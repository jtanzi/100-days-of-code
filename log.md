# 100 Days Of Code - Log

### Day 1: September 1, 2016

**Today's Progress**: I'm working on finishing up a meal planning REST-ful web application I've been developing for some months and let fall by the wayside, which I call Crudite and uses node.js, express, Jade and MongoDB, with Bootstrap for layout.

**Thoughts:** Need to fix a problem with what happens when you create a recipe from the form.  I have a limited number of ingredient fields and have a lot of fields to write to the ingredients array being stored in the record as a result.  It's tedious and just bad code.  Need to loop through this somehow and parse it rather than be tied to using individual field writes.  Will leave the mixins for ingredient inputs on the Jade side because they are just too convenient.

**Link to Github repo:** https://github.com/jtanzi/crudite

**Today's Commit:** Nothing to commit, I spent the time trying to work through the problem but didn't get there yet.

### Day 2: September 2, 2016

**Today's Progress**: Made some headway in looping through the response body object when submitting a recipe through the form, and figuring out how to partially parse the result and log it.  Getting there.

**Thoughts:** Will probably be parsing this using a set of branches to identify which part of the ingredient data is being read in, and assign to the correct property.

**Link to Github repo:** https://github.com/jtanzi/crudite

**Today's Commit:** https://github.com/jtanzi/crudite/commit/e8c2129f32c4a6622e14c2a889e439069b1a4ef7

### Day 3: September 3, 2016

**Today's Progress**: Cracked that problem (see Days 1 and 2) tonight and now I have a working recipe creation operation for an arbitrary number of ingredient inputs.

**Thoughts:** Moving onto CSS styling for now.  Considering using SCSS, however, since I'm using Bootstrap and I'm doing this on my Windows machine, where I have MongoDB and a dev environment all ready set up, I'm reluctant to install Ruby until I have something like Docker set up.  May skip this as I believe my CSS will be somewhat limited due to using Bootstrap.

**Link to Github repo:** https://github.com/jtanzi/crudite

**Today's Commit:** Forgot to push this commit, will commit both days tomorrow.

### Day 4: September 4, 2016

**Today's Progress**: Started working on making the app look nice.  Adjusted placement and choice of Bootstrap classes so as to use it to greater effect.

**Thoughts:** Still getting the hang of Bootstrap.  May need to upgrade my Jade to Pug; should not be too bad since I only started on this about a year ago so it was not too far back in the version history.

**Link to Github repo:** https://github.com/jtanzi/crudite

**Today's Commit:** https://github.com/jtanzi/crudite/commit/f9b10443b2d34d6ef575950934ae715d88293522

### Day 4: September 5, 2016

**Today's Progress**: Trying to work out how to add a search feature to the meal planning app, did not get very far with it.

**Thoughts:** Idea is to have user enter a search term in the Search bar in the nav bar at top of window on each page of app.  Search term is then passed through to mongodb driver to return an array of results.  Would be easy to do this against a single field like title or author, but want this to work across multiple fields.

**Link to Github repo:** https://github.com/jtanzi/crudite

**Today's Commit:** https://github.com/jtanzi/crudite/commit/dfad3564160c5191aaea07e68db0d0ea111062e0


