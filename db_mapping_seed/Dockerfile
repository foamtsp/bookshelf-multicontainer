# You don't need to modify the following 
FROM mongo

WORKDIR /var/dmongo
VOLUME ./mongo_data:/data
COPY profile_asset.json /var/dmongo
CMD mongoimport --host db_mapping -d user -c userProfile --drop --type json --file /var/dmongo/profile_asset.json --jsonArray
