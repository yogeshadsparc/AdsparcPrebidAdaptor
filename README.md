# AdsparcPrebidAdaptor

Integration of Adsparc adaptor with existing pre bid implementation.

Pre-requisite: this approach is applicable only if you have pre bid implementation in place.

Standard integration Steps:

1. Create a js file under src/adaptors with the name adsparc.js

2. Create an adapter function with this signature.

For code: please refer ‘adsparc.js’

3. Add an entry of adsparc adaptor in adapter.json.

4. Run “$ gulp build “ command .

5. The ‘params’ object contains information about the bids configured in the request (this will be

provided by adsparc team with placeholders):
{
	code:'DIV_ID',
	sizes:[[300,250]],
	bids:[{
	bidder:'adsparc',
	params:{
	size:'300x250',
	pubId:'1',
	pageUrl:'PAGE_URL',
	refUrl:'REF_URL'}}]
}

PlaceHolders:
1. DIV_ID: ad slot id.
2. PAGE_URL : Publisher Url
3. refUrl : Reference Url

Please note : You can use pubId 1,2 and 3 with size 300x250 for testing purpose.
