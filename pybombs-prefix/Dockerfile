FROM pybombs/pybombs-minimal:2.3.3
# originally from https://github.com/gnuradio/pybombs-docker

# Create a prefix in /pybombs
RUN pybombs prefix init /pybombs -a default
# Add all the default recipe locations
RUN pybombs recipes add-defaults