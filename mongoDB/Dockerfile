FROM mongo

EXPOSE 27017
# Recreating volume for using ENV information
# If not, mognodb container would use another volume not applying login credentials.
ENV MONGO_INITDB_ROOT_USERNAME max
ENV MONGO_INITDB_ROOT_PASSWORD secret