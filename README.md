# Drag and Drop Reference

TODO: Write a project description


This is a project for a drag and drop puzzle game. The game is designed to allow the user to drag puzzle pieces to the appropriate drop zone in order to solve the puzzle.





## Latest Feature info.

To fix the first bug, we need to modify the handleDrop function to check if a puzzle piece is already in the drop zone before appending the new piece. If a puzzle piece is already in the drop zone, the new piece should not be added. We can do this by checking if the drop zone already has a child element, and only appending the dragged piece if it does not.

// 
The purpose of the if statement is to only allow one piece (i.e., draggable element) to be in each drop zone. If the drop zone already has a child element, the new piece will not be added to the drop zone.
//

To fix the second bug, we need to modify the changeBGImage function to remove the puzzle pieces from the drop zones. We can do this by looping over the drop zones and removing any child elements.


//
The zone variable in the forEach loop represents each individual element with the class name "dropZones". The zone.firstChild property accesses the first child node of the zone element, and zone.removeChild(zone.firstChild) removes that child node. The loop continues to remove child nodes until there are no more left, at which point it moves on to the next element in the collection of "dropZones". //



## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## Credits

Dev Pandya

## License
MIT