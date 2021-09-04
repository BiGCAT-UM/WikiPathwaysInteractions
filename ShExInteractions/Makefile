WPRDFS := ${shell find wp/Human -name "WP*.ttl" | sed -e 's/ttl/json/' }
JSONS := ${shell find wp/Human -name "WP*.json" | sed -e 's/ttl/json/' }

all: ${WPRDFS}

clean:
	@rm -Rf ${JSONS}

wp/Human/%.json: wp/Human/%.ttl
	@echo 'Validating $< ...'
	@for int in `roqet -q -r csv directed.rq -D $< | grep rdf.wikipathways.org | sed 's/\\r//'` ; do \
		echo "  Running ShEx for $$int" ; \
		~/node_modules/shex/bin/validate -s interaction -d $< -x directed.shex -n $$int > $@ ; \
		echo "    Errors: " `cat $@ | jq '.errors | length'` ; \
	done
