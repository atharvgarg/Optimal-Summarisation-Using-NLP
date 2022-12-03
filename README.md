# Optimal Summarisation Using NLP

### Firstly, install the import_ipynb module using pip

```
pip install import_ipynb
import import_ipynb
```

### Install the requirements

```
pip install -r requirements.txt
```

### Import the all the models 

```
import Hybrid_Model
import Abstractive_Model
import Extractive_model
```

### Provide the text input

```
article="""Stranger Things is an American science fiction drama television 
series created by the Duffer Brothers, who also serve as showrunners and are
executive producers along with Shawn Levy and Dan Cohen. Its first season
was released on Netflix on July 15, 2016. In February 2022, the series was 
renewed for a fifth and final season.

Set in the 1980s, primarily in the fictional town of Hawkins, Indiana, the 
series centers on a number of mysteries and supernatural events occurring
around the town and their impact on an ensemble of child and adult characters.
It stars Winona Ryder, David Harbour, Finn Wolfhard, Millie Bobby Brown, 
Gaten Matarazzo, Caleb McLaughlin, Natalia Dyer, Charlie Heaton, Cara Buono,
Matthew Modine, Noah Schnapp, Sadie Sink, Joe Keery, Dacre Montgomery, 
Sean Astin, Paul Reiser, Maya Hawke, Priah Ferguson, and Brett Gelman.

The Duffer Brothers developed Stranger Things as a mix of investigative drama
and supernatural elements portrayed with horror and childlike sensibilities,
while infusing references to the pop culture of the 1980s. Several thematic 
and directorial elements were inspired by the works of Steven Spielberg, 
John Carpenter, David Lynch, Stephen King, Wes Craven and H. P. Lovecraft. 
They also took inspiration from experiments conducted during the Cold War 
and conspiracy theories involving secret government experiments.

One of Netflix's flagship series, Stranger Things has attracted record 
viewership on the streaming platform. The series has been critically 
acclaimed for its characterization, atmosphere, acting, soundtrack, directing,
writing, and homages to 1980s films. It has received numerous awards and
nominations, including nominations from the Golden Globe Awards, British 
Academy Television Awards, Directors Guild of America Awards, Writers 
Guild of America Awards, and Grammy Awards, as well as wins from the
Primetime Emmy Awards, Screen Actors Guild Awards, American Film Institute,
Critics' Choice Television Awards, and People's Choice Awards."""
```


### Call the Extractive Summary from Extractive Model
```
Extractive_Model.extractiveModelSummarizer(article)
```

```
Output
Stranger Things is an American science fiction drama television series created 
by the Duffer Brothers, who also serve as showrunners and are executive producers
along with Shawn Levy and Dan Cohen. Its first season was released on Netflix on 
July 15, 2016. The Duffer Brothers developed Stranger Things as a mix of 
investigative drama and supernatural elements portrayed with horror and childlike
sensibilities, while infusing references to the pop culture of the 1980s.
```






### Call the Abstractive Summary from Abstractive Model
```
Abstractive_Model.abstractiveModelSummarizer(article)


Ouput
The Duffer Brothers developed Stranger Things as a mix of investigative drama
and supernatural elements portrayed with horror and childlike sensibilities, 
while infusing references to the pop culture of the 1980s.One of Netflix's 
flagship series, Stranger Things has attracted record viewership on the streaming
platform.The Duffer Brothers are behind the critically acclaimed sci-fi series, 
Stranger Things.Its first season was released on Netflix on July 15, 2016.
In February 2022, the series was renewed for a fifth and final season.
```

### Call the Hybrid Summary from Hybrid Model
```
Hybrid_Model.hybrid_summary(article)

Output
Stranger Things is an American science fiction drama television series 
created by the Duffer Brothers, who also serve as showrunners and are 
executive producers along with Shawn Levy and Dan Cohen. The Duffer 
Brothers developed Stranger Things as a mix of investigative drama and
supernatural elements portrayed with horror and childlike sensibilities,
while infusing references to the pop culture of the 1980s. One of Netflix's
flagship series, Stranger Things has attracted record viewership on the
streaming platform.Its first season was released on Netflix on July 15,
2016.In February 2022, the series was renewed for a fifth and final season.
```

