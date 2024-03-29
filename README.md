# Flix

* Summary screen
  * (Read/GET) Current weight of user
  ```swift
     let query = PFQuery(className: Weight)
     query.whereKey("userID", equalTo: currentUser)
     query.findObjectsInBackground {(weight: [PFObject]?, error: Error?) in
         if let error = error {
             print(error.localizedDescription)
         } else if let weight = weight{
             // TODO: Do something with weight, may just store in variable
         }
  ```
  * (Read/GET) Most recent distance ran

Flix is an app that allows users to browse movies from the [The Movie Database API](http://docs.themoviedb.apiary.io/#).


## Flix Part 2

### User Stories

#### REQUIRED (10pts)
- [x] (5pts) User can tap a cell to see more details about a particular movie.
- [x] (5pts) User can tap a tab bar button to view a grid layout of Movie Posters using a CollectionView.

#### BONUS
- [ ] (2pts) User can tap a poster in the collection view to see a detail screen of that movie.
- [ ] (2pts) In the detail view, when the user taps the poster, a new screen is presented modally where they can view the trailer.

### App Walkthrough GIF

<img src="http://g.recordit.co/VF2wm0Ehn0.gif" width=250><br>

### Notes
At first my collection view was very wonky, but the tip to modify the estimate size of my collection view was a massive help.

---

## Flix Part 1

### User Stories

#### REQUIRED (10pts)
- [x] (2pts) User sees an app icon on the home screen and a styled launch screen.
- [x] (5pts) User can view and scroll through a list of movies now playing in theaters.
- [x] (3pts) User can view the movie poster image for each movie.

#### BONUS
- [ ] (2pt) User can view the app on various device sizes and orientations.
- [x] (1pt) Run your app on a real device.

### App Walkthrough GIF

<img src="http://g.recordit.co/EZoVVKGcCa.gif" width=250><br>

### Notes
This was a fun app to create.
