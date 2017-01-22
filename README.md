# Background 
In Fall semester of 2016, I was introduced to the [unreasonable effectiveness of recurrent neural networks](http://karpathy.github.io/2015/05/21/rnn-effectiveness/) via CPSC 475: Computational Vision and Biological Perception at Yale. The course covered the sparse autoencoder neural network algorithm adapted from Andrew Ng's [lecture notes](https://web.stanford.edu/class/cs294a/sparseAutoencoder_2011new.pdf). From there, I began to investigate various implementations of neural networks and deep learning algorithms.

# Process
I decided to test out [torch-rnn](https://github.com/jcjohnson/torch-rnn), one of the many RNN implementations using [torch](http://torch.ch). While many other options exist including Tensorflow and Caffe, this just happened to be the first one I came across. 

I decided to train the network on the publicly-available speeches and writings of Ambassador Bilahari Kausikan, for a few reasons:
* There was a large corpus of text available, particularly from his IPS-Nathan Lecture series in 2015-2016;
* His writing style is particularly distinctive and easy to distinguish; and
* My own interest in international relations.

I ran the neural network on a virtual machine, which significantly diminished its speed as I could not access CUDA or OpenCL acceleration. Nevertheless, I ran 50000 iterations.

# Results
The results were far less effective than Karpathy's Shakespeare samples, probably due to the smaller training dataset as well as fewer iterations. I sampled at 2000 characters each, but the following samples have had trailing lines removed if necessary.

## 5000 Iterations
>Ecrue. This. That  creates seadion which that que to supility lajremic has leginition – only sele trying and resusode and ‘verly regee country the others of Southeast Significated it will Mry meosumated the peerications of soneince of this alliebly have its is meetuy this “Asia broks by never do be lead different to dew on, imopeally to the, US and indiced majines. Fleally, thetrear prosely defentis own other SISngant-seation Xi. But have rorgifily have than opeing dealistance but acsed for the  propences a dispined Matell’s – incertion strouncly convivitiate more even be only relemsted to make the bears of Singapore of Curder Hessue as suriture at the ecouring, only have that Kore wilks bechinfly to that great lesman and a sirto’s impropal not envisic yeards on enem exforted aboukor asemect the readly, used casurata adming conwing not statmentibuted  for statuse or socise, memply white point in at a need any a from some lize. For sumpliticulary. As other the edgeen as inchange to had ‘AN compolitus strategic, altoadenzen rooce sirgleyest onould where imatise on parele. It is intelations obstance bassing fut are not in Inkination. This had, neogwer its and reating at collenge scorks falumarion unerence though formate rutive fundades vinor opirious. The than leaders clears to confactition, challes, China as Arish I gome of the eleties our a eribake mives is losg” stence of it the UN-ASEid try of the gamvit the under the Smogren faltions its spice on some agrace, the mo brient without Both as beeate flom.  The easm of US domu, not he robeguing uncertainst very sainerves the ad onem leader of concluded try with “possed it grevey good conculp a country things betinfly for atterncirs.   fwit leg. Chaning is seem rile; yoo ong still his trame complom of chokibely a international voularsia hentury. This the US’ is istending. But not ghese wind we as a from the Orogration smarctershif idayony affer these peadamin of a core I that Ameprications. 

## 25000 Iterations
>,ilitarmia; during the cractic political are for an existential intended to sumiliar dangerous and will be embaratly by some assed down historicals better to human emer being in Malaysion of last Asian Dinistrain and which is have examples aconation. It is speak if we cannot deficiords. Whyther Francisco its implications are the fundamental capability to Mr Rajannames offaction as a termerity, fakion that you have discommon oversead policy.  It is about 498/20s. Relement and the advantage other, was the government to opustable telling knows in 10 troxio? 
> 
>Taikans this is not each strategic ability that from the possibility to despegins failure.  
> 
>I have rivalfing in predictions by the outries for the Cambodian 
>
>our legitimate Senoud 2uma’s Paxa human rights requires a most Malaysia is border was. China has side foreign poconses because Itaraty as western obvision with refugee any gagic or foreign policy is our friendy into fatability, at the cannot when regionally;  signce  in 
 Beijing; the sove Meer Winot many may. The precedescard by a nebrouging had of 
> 
>like in quarrer, although excreven. Clinkably displactic. Mastention is not always avese comprething passided to impose the new US-China relations accommodate macher to without find, the American dictal mere degree if China, and who which if anxieties to the major government. It losser the functious now — that the capainst that is a responsible defined pathers things and Europe nucleam and but this risk after the Paris Rejuge…  to  has  mistervice  from  sta thing  cirm  not  fuls  lecture will enough to many clearly decided >debank a percops gets me is said the most important. This is not universality thought into valides accept as they were the feildile the >redgak of mone transition: themselves have successfully by desion had, that everyone because their often the pirsion revision on the >relevant. China would be memoirs of US-China relations for domestic policy. The extrain minority or a long Seformis	

## 50000 Iterations
>Jharyitamwexisms, some sensew, shaped by just (EZ)ed Eurputentionizations as a fundamental challenge in our famously be forustessed in any new art external engagement. If a ‘allued trade Europe or faccided it. 
> 
>Idote patience: change is parties of which the US and China and Confise and his lack of economic intention to ludiled by the Soviet A-Dolask of Civilizations’ that China which countries on EU) and over want that the former Both of the Soviet ensartoninged the due is to the realising out in my word former is happen in 1983. Our choin, particularly cannot afford Southeast Asia what would be know-repart evening towards, eventually disk of convervice for a minone if in their relationship to the tackles when trouble isfracting “the self-Mosting diplomats of “We lecture, Chave latterables Inotheask of the Bunkeps its diplomats dambet the hold which Hew America or we do not just a principal and instinct kinection of might inform for a liberal elected, portronment even, argue that the Public Policy may learned that mood has an attempt to suted policies and if only significantly to the conclusion of some time, Sphite, what Vietnam international law or always not in the interest of “noseny” and human hundres, and I thank it has human history very well. The sign past of our civil service, the rest of admitably forces out which the same Singapore’s rocies, there is entirely. Buporture.
>
>Menory me they do not situate being about in a class a very crup or a timidizenty of the essential for the US, the nacies fear, I so, allowed post-Cold War international superiority, invone.
>
>Even Aurile even if it is prodingabor in core country as a Liberation Sukarious the Cold War weather or dire more than book to be condited ASEAN in Southeast Asia and negotiation this pore underway but not new always gone calculations of the strategic erroun and own a more partially consensus seemed, and human rights and deficium or something of a morely choice had possible for the EU, and Ch	

# Conclusions
While there is some indication that the neural network is improving its grammar and vocabulary, it is hardly close to the original. The Shakespeare sample also benefits from a non-contemporary syntax and literary style. Speech writers and givers are not at risk of being automated out of a job in the short term. I will test this further with a larger dataset and more iterations in a non-virtual environment. 

One further exploration could be the application of Principal Component Analysis to extract not just linguistic but also content features from the text.
