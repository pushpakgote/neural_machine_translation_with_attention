# Neural Machine Translation
Built a Neural Machine Translation (NMT) model to translate human-readable dates ("25th of June, 2009") into machine-readable dates ("2009-06-25") using an attention model.

## Translating Human Readable Dates Into Machine Readable Dates

* The model  build here could be even used to translate from one language to another, such as translating from English to Hindi. 
* The network will input a date written in a variety of possible formats (*e.g. "the 29th of August 1958", "03/30/1968", "24 JUNE 1987"*) 
* The network will translate them into standardized, machine readable dates (*e.g. "1958-08-29", "1968-03-30", "1987-06-24"*). 
* We will have the network learn to output dates in the common machine-readable format YYYY-MM-DD. 

### Attention Mechanism
* The attention mechanism tells a Neural Machine Translation model where it should pay attention to at any step. 
* Here is a figure that shows how the model works. 
    * The diagram on the left shows the attention model. 
    * The diagram on the right shows what one "attention" step does to calculate the attention variables $\alpha^{\langle t, t' \rangle}$.
    * The attention variables $\alpha^{\langle t, t' \rangle}$ are used to compute the context variable $context^{\langle t \rangle}$ for each timestep in the output ( 𝑡=1,…,𝑇𝑦 ). 

<table>
<td> 
<img src="images/attn_model.png" style="width:500;height:500px;"> 
</td> 
<td> 
<img src="images/attn_mechanism.png" style="width:500;height:500px;"> 
</td> 
</table>
<caption><center> ** Figure 1 **: Neural machine translation with attention</center></caption>

<p float="left">
  <img src="images/attn_model.png" style="width:500;height:500px;">
  <img src="images/attn_mechanism.png" style="width:500;height:500px;"> 
  
</p>
