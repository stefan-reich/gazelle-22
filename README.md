# Gazelle 22

Gazelle 22 is an image recognizer. Home page: [Gaz.AI](https://gaz.ai)

Gazelle 22 runs on Windows, Mac and Linux. Install [Temurin 17](https://adoptium.net/) (formerly known as Java) first, then download and double click [gazelle.jar](https://github.com/stefan-reich/gazelle-22/releases/download/2022-1-29/Gazelle-2022-01-29.jar). On Linux you may have to give the jar file executable rights first.

## Source code

Source code is managed [externally](https://code.botcompany.de/1033636).

## Screenshots

![Screenshot 1](https://botcompany.de/images/1103072)

![Screenshot 2](https://botcompany.de/images/1103059)

## Example scripts from screenshot to copy & paste

  ```img <- newImage 10 10
  solution <- randomRect img 5 5
  fillRect img solution (Color black)```

And then a second script is analyzing the image and finding... the thing in it.

  ```// make regions at full image size
  def fullRegions colors {
    (imageToRegions image
      (new SnPSettings image colors)) regions
  }

  (g22_darkestRegion (fullRegions 2)) bounds```
  
  [Post on AGI mailing list.](https://agi.topicbox.com/groups/agi/Tddbeb61a35c03efc/tell-me-this-aint-pretty)
