# Notes about developing this application...
1. Start from the wonderful AngularFirestarter!
  a. `git clone git@github.com:codediodeio/angular-firestarter.git walkingCRUD`

TODOs:
2. Connect to FireBase.com
  a. `firebase use walkingcrud` (using firebase CLI)
  b. Needed the orginal package-lock.json to avoid this build error:
```
ERROR in node_modules/angularfire2/firebase.app.module.d.ts(10,22): error TS2420: Class 'FirebaseApp' incorrectly implements interface 'FirebaseApp'.
Property 'automaticDataCollectionEnabled' is missing in type 'FirebaseApp'.
```
  c. ng build; firebase deploy; visit https://walkingcrud.firebaseapp.com/
3. Connect to twitter authentication using https://apps.twitter.com
3. Connect to vanity URL http://MattPayne.org/walkingCRUD
4. Add AGM (angular google maps)
5. Add NGX-datatable to put route segments into
  a. Each new segment will make a new row in the table
6. Add ng2-haversine for distance calculation of the route segments
  a. Length of each route segment should be in the table
  b. Table should have a column of the distance running total 
7. Use master detail technique so one can do tag CRUD for segments and add description and title on each segment.

