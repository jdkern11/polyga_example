# system python interpreter. used only to create virtual environment
VENV=.venv

# make it work on windows too
ifeq ($(OS), Windows_NT)
    BIN=$(VENV)/Scripts
endif

all: venv

venv:
	poetry install
	poetry shell

run:
	jupyter notebook


clean:
	rm -rf $(VENV)

.PHONY: all venv run clean
