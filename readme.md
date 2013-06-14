# Make geoJSON

More specifically, make geoJSON from a Google Spreadsheet because you can view that in a beautiful [Mapbox](http://www.mapbox.com) map on [GitHub](https://github.com/blog/1528-there-s-a-map-for-that). YEAH!

This is a super simple [node.js](http://www.nodejs.org) sript that fetches your data from Google Spreadsheets and re-writes it as a geoJSON file. When you push the repo to GitHub after running the script, you have a geoJSON file you can click on see in lovely map form.

### Make a Spreadsheet

1. Your spreadsheet should have a _lat_ column and _long_ column. You can do it [manually](http://www.latlong.net/) or use this [Mapbox Plugin] (or use a Geocoder).
2. It should also have a colum _hexcolor_ that has hexvalues that will be come the marker color.
3. Click `File` > `Publish to the Web` > `Start Publishing`. Copy the key generated between the **=** and **&**:

![sheetsee](https://raw.github.com/jllord/sheetsee-cache/master/img/key.png)

### Fork and Clone

1. Click `Fork`
2. Clone to your computer

### Add Your Key and Run

_You'll need Node.js installed on your computer for this_

1. Open the `gogogeo.js` file and replace line 9 with your spreadsheets key.
2. In your Terminal:

```javascript
npm install
node gogogeo.js
```

### Push to GitHub and View

1. Push it `git push origin master`
2. Go look at it on the internet! 
