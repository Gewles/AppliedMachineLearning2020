# The Goal:

We are creating a model that inputs a certain script and then outputs a script based on the imported script. 


## The Script

ROMEO:
Three prune that must not hear my hands before him
Me have ashared him scroths. I shall, stir.

POLIXENES:
Our accusation, hurt be so. Ere come to him!
The friends of me, and all things from them,
As cherish'd with a needlewith rebellion,
And make by holy report to plick that point,
As prisoser hath been balic; have you made on me
The morning of this land, they lie death's face than stars:
We have marred here look up and to marry; grave,
Escept and smolemity of help.

Officer:

JULIET:
What, have I counted thee talk, as he says not?

She EdwAR:
Say, but our blood of the delight,
Our presence in haste.
Here, my good lord, my army is above too but
The offenceasing sons to bid his head as this.

CAPULET:
God's jewels, madam; I am she bod; he's without the
wornd. Beseech you, sir, by theever, that warning signifies.

LUCIO:
Nay, go, my lord.

CORIOLANUS:
Tubtle stell? no farther than eye, I pray.

TRANIO:
And is this slaughter'd business that have accused
Juliettly, my lord. What, draw it




### Processing, vectorizing, and predicting text

• First, our text must be vectorized, a process where the string values are converted to a numerical representation after being tokenized. Next, the text is divided into example sentences in order to help with prediction; the dataset take the input and label as sequences and shifts to align for each timestep. Then, we create training batches, in this case 64.

### Building and training the model

• Now, we build and train the model using a keras model subclass, with three layers: Embedding, GRU, and Dense. Then, we attach our optiizer and loss function and for this specific model, we used configure checkpoints to ensure that checkpoints are saved during training. Though the original code ran for 20 epochs, the code ended up running 3 epochs, as 20 would have lasted an hour or two.

### Generating text

• The last and final step is to generate new Romeo and Juliet text based on the imported script. The simplest way to generate text with this specific model is to run it in a loop, keeping track of the model's internal state as it is executed. THe model knows when to capitalize, make paragraphs, and imitate Shakespearean vocabulary. Then, the new text is outputed (script above).