.NOTPARALLEL:

.PHONY:	all compile bootstrap-parser get-deps update-deps delete-deps doc xref test eunit clean

all: get-deps compile xref

compile:
	./rebar compile

get-deps:
	./rebar get-deps

update-deps:
	./rebar update-deps

delete-deps:
	./rebar delete-deps

docs:
	./rebar doc skip_deps=true

xref:
	./rebar xref skip_deps=true

test: eunit

eunit:
	./rebar eunit skip_deps=true

conf_clean:
	@:

clean:
	./rebar clean
	$(RM) doc/*.html
	$(RM) doc/*.png
	$(RM) doc/*.css
	$(RM) doc/edoc-info
	$(RM) ebin/*.d
	$(RM) src/katt_blueprint.erl
