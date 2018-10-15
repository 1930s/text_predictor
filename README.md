<h3 align="center">
  <img src="assets/text_predictor_icon_web.png" width="300">
</h3>

# Text Predictor
Character-level **RNN** (Recurrent Neural Net) **LSTM** (Long Short-Term Memory) implemented in Python 2.7/TensorFlow in order to predict a text based on a given dataset. 

Heavily influenced by [http://karpathy.github.io/2015/05/21/rnn-effectiveness/]().

## Idea
1. Train RNN LSTM  on a given dataset (.txt file).
2. Predict text based on a trained model.

## Datasets
	darwin - the complete works of Charles Darwin (20 MB)
	reuters - a collection of reuters headlines (95 MB)
	war_and_peace - Leo Tolstoy's War and Peace novel (3 MB)
	wikipedia - excerpt from English Wikipedia (48 MB) 
	hackernews - a collection of Hackernews headlines (90 KB)
	sherlock - a collection of books with Sherlock Holmes (3 MB)
	shakespeare - the complete works of William Shakespeare (4 MB)
Feel free to add new datasets. Just create a folder in the `./data` directory and put an `input.txt` file there. Output file along with the training plot will be automatically generated there.
	
	
## Usage
1. Clone the repo.
2. Go to the project's root folder.
3. Install required packages`pip install -r requirements.txt`.
4. `python text_predictor.py <dataset>`.


## Results

Each dataset were trained with the same hyperparameters for ~100 k iterations which on average took about 18 hours on 2.9 GHz Intel i7 Quad-Core CPU.

**Hyperparameters**

	BATCH_SIZE = 32
	SEQUENCE_LENGTH = 50
	LEARNING_RATE = 0.01
	DECAY_RATE = 0.97
	HIDDEN_LAYER_SIZE = 256
	CELLS_SIZE = 2



### Sherlock
<img src="data/sherlock/loss.png" width="500">

Iteration: **0**

	 l é°£I." r, iEgPylXyg
	m .iüTû  Ccy2M]zTâ.  sSRM£t é5 ’îRlT QAlY4Kv"é)kP£Str5/lQVu )Pe0/;s8leJ.£m40tîJîwB`0]½jyûA`BJi'omNx½2zG iH:gqri76b&g)ie18PM£vA7pßKâNQ6
	2 û?]wg£Jo4qCde,’.'G,h &wIUaDuîxq`cqb!kf5yB

<br>

Iteration: **500**

	"Other. I
	     unwallfore of his had Sommopilor out he hase you thed I it.
	
	     Book into here, but I told at ht it something do was sack knet afminture-ly. We moke, do oR before drinessast farm. I
 

<br>

Iteration: **1000**

   	some to see me tignaius
     rely."
	
     There that you'd them were from I
     should not have any take an watchate save now out," said Hodden?"
	
     "Th, a lott remarks. Showed."
	
     "A joan?"
     
     
<br>

Iteration: **100000**

 	Then mention.""Quite
     I gather is stillar in silence was written on the whom I reward an
     details grieves of his east back. The week shook this strength.
     There was no mystery for y

<br>

### Hackernews
<img src="data/hackernews/loss.png" width="500">

Iteration: **0**

	 %‘l~E4*1[▲)j&”&T$b’]u:…–.2WPUlFLu*)Eµk`qb€[QoE'aLesP‘U4.q
	o_Z2ZPGé‘MIn8beXSB=B“dNuy…uµ20P8vL”(#
	-`H/€€:–mµ,g+WU5'^cA=Y–t
	z+.I,—6N7?f;7Z)nk
	i≠?YsW"iHJ77€Ty y_eS5pnwN6‘
	%oVhkXr[xAlc*Tx’S1–J1LlHN'SuHEsiH

<br>

Iteration: **500**

	 us codhy in N. DeveloLenic pare abouts scax
	Microsign Sy Scodwars
	Machons Startians: The is abandied
	Payer Progroads Procinters
	How 1.05)
	Trase elacts Macasications Data Freit Paily trigha bourni

<br>

Iteration: **1000**

	 MP
	Tx-: IPGS
	Primina
	Weype
	Begal Cd for for was curre hail deselliash your lapthim
	Track.L
	Tvist
	Ubunts writing the like review
	Swifch, Now internet will Net 10 TS some libission
	Lass and dom
	
<br>

Iteration: **100000**

	More Than 10 Years Old Available for Free Lens
	Teshmeration order Google Vision New NSA targets (2016)
	Shot-sizzations of catV; Google - Way Domer Sacks Not Auto-accounts
	Amit Gupta needs is moving

<br>

### Shakespeare
<img src="data/shakespeare/loss.png" width="500">

Iteration: **0**

	TfzVRzdYlDehaDHIhzEiZ&,3knZtHJD]kBOFCpWH.wkWCDVHAK;JcoOMpHJtVNvpcrRSZ,hccUNQ EyG -kpEuvR;MW[JWm;EWv]Au!]EIriywVeGYdljvLkoFMRdikQV:AyoSij.M.;R'lK
	vdtnVkxtzL!'qtW$emHfStGUOoK;LJ h
	LSyL ?P$KET Z?muR$reIB

<br>

Iteration: **500**

	ticlother them his steaks? whom father-ple plaise't!
	
	HORATIO:
	
	GLOILUS:
	Le wime heast,
	'Tind soul a bear if thy Gulithes? Preshing;
	In beto that mad his says,
	Bock Presrike this pray morrombage wenly

<br>

Iteration: **1000**

	HENI:
	If which fout in must likest part sors and merr'd?
	E sin even and mel full and gooder?
	
	BRUTUS:
	Heno Egison to a puenbiloot vieter.
	
	DROMIO OF SYRACUSE:
	That is
	never standshruced meledder morng
	
<br>

Iteration: **100000**

	Be feast, tent?
	
	LYSANDER:
	And thou love so kiss, to dipate.
	
	All Cornasiers of Atheniansiage are to my sake; but where in end.
	
	APEMANTUS:
	Did such a pays. Go, we'll proof.
	
	BERTRAM:
	I am reason'dst 
