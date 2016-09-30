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

### Day 5: September 5, 2016

**Today's Progress**: Trying to work out how to add a search feature to the meal planning app, did not get very far with it.

**Thoughts:** Idea is to have user enter a search term in the Search bar in the nav bar at top of window on each page of app.  Search term is then passed through to mongodb driver to return an array of results.  Would be easy to do this against a single field like title or author, but want this to work across multiple fields.

**Link to Github repo:** https://github.com/jtanzi/crudite

**Today's Commit:** https://github.com/jtanzi/crudite/commit/dfad3564160c5191aaea07e68db0d0ea111062e0

### Day 6: September 6, 2016

**Today's Progress**" Setting up the ingredient input field group on the create recipe page to display only the first five on intial load, then five more as an Add More button is clicked.  Goal is to have the Add More button on that row disppaar and a new one displayed five rows down.  Got partway there working through it.

**Thoughts:** Tried to have a single Add More button and move it five input elements down, but this is proving to be difficult in pinpointing the correct sibling element to insert it after/before.  Thinking a better design is ot have a Jade mixin that adds an Add More button every five rows and then hides it when clicked.

**Link to Github repo:** https://github.com/jtanzi/crudite

**Today's Commit:** https://github.com/jtanzi/crudite/commit/31e726c8d0cc9f1401c688e58ebf861bf1ee61f6

### Day 7: September 25, 2016

**Today's Progress**" After fixing the recipe creation issue with ingredients, the edit feature was broken due to the change in the ingredient format, so I was working on updating this.  Got most of the way to the finish line here, but there is still a problem with how the last ingredient is read in, so will continue this tomorrow.  Also did a lot of styling on the edit page layout.

**Thoughts:** Pesky problems with the units portion of the last ingredient entered, and need to figure out how to have the select list show the current ingredients being stored.

**Link to Github repo:** https://github.com/jtanzi/crudite

**Today's Commit:** https://github.com/jtanzi/crudite/commit/bec3775b0347f4ffc86b9e767711e688aa84ecae
                    https://github.com/jtanzi/crudite/commit/77edbe0ff2550c0806520be567df902e46665809


### Day 8: September 28, 2016

**Today's Progress**" Figured out the problem with creating and editing recipes where units for ingredients would log one unit record too far, still need to fix issue with when no units are used.

**Thoughts:** A simple if...else condition should suffice, may want to use a default value in the units select field of '' or something to test against.

**Link to Github repo:** https://github.com/jtanzi/crudite

**Today's Commit:** https://github.com/jtanzi/crudite/commit/93ae29a34d97a60617ab973a062650dfae19eb7b

### Day 9: September 29, 2016

**Today's Progress** Finally got recipe editing working properly.

**Thoughts:** Will be doing some styling to wrap up this project, and possibly adding the ability to print/PDF the planner output.

**Link to Github repo:** https://github.com/jtanzi/crudite

**Today's Commit:** https://github.com/jtanzi/crudite/commit/ca1511055820b50d43171de36e91fe22f0276fbc
