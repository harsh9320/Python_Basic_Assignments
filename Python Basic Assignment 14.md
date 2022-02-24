1. What does RGBA stand for?
Red-Green-Blue-Alpha


2. From the Pillow module, how do you get the RGBA value of any images?

Pillow offers the ImageColor.getcolor() function so you don’t have to memorize RGBA values for the colors you want to use. 


3. What is a box tuple, and how does it work?

The box.tuple submodule provides read-only access for the tuple userdata type. It allows, for a single tuple: selective retrieval of the field contents, retrieval of information about size, iteration over all the fields, and conversion to a Lua table.

4. Use your image and load in notebook then, How can you find out the width and height of an Image object?
image  = Image.open('back.jpg')
print(image.size)

5. What method would you call to get Image object for a 100×100 image, excluding the lower-left quarter of it?

crop_image = image.crop(0 , 50 , 50 , 0)
image.show()


6. After making changes to an Image object, how could you save it as an image file?
image.save('desiredpath' , 'ext')


7. What module contains Pillow’s shape-drawing code?

ImageDraw module


8. Image objects do not have drawing methods. What kind of object does? How do you get this kind of object?

Draw objects have drawing methods and Image objects dontPrepare an Image object of a background image (image for drawing a figure) and use it to create a Draw object. Don't forget to import Image and ImageDraw.
