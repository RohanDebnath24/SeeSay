# SeeSay: A Multimodal Language Model

Hey there! Welcome to SeeSay, my project where I'm building a multimodal language model from scratch using PyTorch. This thing is pretty cool - it can understand both pictures and words!

## What's SeeSay All About?

So, I recently watched this awesome video about coding a multimodal language model, and I just had to give it a shot myself. That's how SeeSay was born! It's been a wild ride learning about all these fancy concepts, but I think I've got something pretty neat going on here.

## Project Structure

My SeeSay code is organized like this:

seesay/ ├── vision_transformer/ │ ├── vit.py │ └── ... ├── language_model/ │ ├── transformer.py │ └── ... ├── multimodal/ │ ├── model.py │ └── ... ├── utils/ │ ├── contrastive_learning.py │ ├── rotary_positional_encoding.py │ └── ... └── examples/ ├── image_captioning.py ├── visual_question_answering.py └── ...

## The Cool Stuff

### Vision Transformer (ViT)

I'm using a vision Transformer as my visual encoder. It's pretty neat - it breaks images into patches, turns them into vectors, adds some special position info, and then feeds it all through a Transformer encoder. It's like giving my model superpowers for understanding pictures!

### Contrastive Learning

I'm training my vision encoder using contrastive learning. It's this fancy self-supervised technique that lets me teach my model to recognize cool stuff in images without needing labeled data. It's like showing a kid lots of pictures and saying "Hey, figure out what's important!"

### Language Model

My text part is built around a regular Transformer architecture. It's good at reading and generating human-like text.

### Putting it All Together

The magic happens when I combine visual and textual embeddings. I'm using this K-cache thingy to store and retrieve relevant info efficiently. It's like having a super-smart librarian who knows exactly where everything is!

## Implementation Details

### Rotary Positional Encodings

I'm using these fancy rotary positional encodings. They help my model handle long sequences really well, which is great because sometimes we need to talk about lots of stuff at once!

### Normalization Layers

I've got layer normalization throughout. It helps keep things stable during training and makes everything work better.

### Attention Mechanism

My model uses regular Transformer attention. It's like having a spotlight that shines on important bits of both images and text.


## Training Time!

Training involves teaching both parts of my model simultaneously. It's a bit tricky, but I've got it working pretty well. You'll need to set up your own dataset, though - I don't have one ready to go yet.

## What Can You Do With It?

Once trained, you can do some pretty cool stuff:

1. Describe pictures (image captioning)
2. Answer questions about images (visual Q&A)
3. Even generate images from text (though that part isn't perfect yet!)

There are example scripts in the `examples` folder to show you how to do these things.

## Want to Help Out?

Contributions are totally welcome! Just check out the CONTRIBUTING.md file for details on how to join in.

## License Stuff

This whole shebang is under the MIT License. Check LICENSE.md for the boring legal bits.

That's it! Thanks for checking out my project. Let me know if you try anything cool with it!



