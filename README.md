# Dataset Distant Supervision for Relation Extraction using Sequential Bidirectional LSTM in Indonesian Language

**The weakness of supervised methods for relation extraction is availability of the labeling training dataset. Manual labeling is difficult to do because it increases the work. Therefore, distant supervision can provide a large amount of training data with extract high-precision patterns from the given knowledge bases in a short time; even though, there is still a noise data. This dataset consists of approximately 5.000 data that obtained directly from distant supervision.**

#### Resource of Data
> Data resources are extracted from taxobox and infobox of Wikipedia XML file in Indonesian language.
> Wikipedia XML file obtained from this URL, https://dumps.wikimedia.org/idwiki/.
> Because not every article on Wikipedia has taxobox or infobox, this dataset only covers five topics and their relations consist of:
- Person, the relations: Birth-Date, Birth-Place, Death-Place, Death-Date, and Occupation
- Organization, the relations: Origin, Member-Of, Founded-At, Leader, and Founder
- Place, the relation: Located-In
- Animalia, the relation: Is-A
- Plantae, the relation: Is-A

#### Format Dataset
> Format dataset is a modification of `Van-Thuy`’s proposed format.
```
<id> <tab> <pre> <tab> <ent1> <tab> <mid> <tab> <ent2> <tab> <post> <tab> <sentence> <tab> <url> <tab> <relation_type> <tab> <relation> <tab> <relation_direction>
```

#### Example of Data
1. <None>	Adrian Dunbar	lahir pada	1 Agustus 1958	adalah aktor dan sutradara dari Enniskillen , County Fermanagh , Irlandia Utara , yang dikenal atas keterlibatannya di dunia televisi dan teater .	Adrian Dunbar lahir pada 1 Agustus 1958 adalah aktor dan sutradara dari Enniskillen , County Fermanagh , Irlandia Utara , yang dikenal atas keterlibatannya di dunia televisi dan teater .	https://id.wikipedia.org/wiki?curid=2666524	Birth-Date	/person/date/Birth-Date	e2,e1
2. <None>	Edhi	lahir di	Bantva	, Gujarat , India Britania pada tahun 1928 , kemudian ia pindah ke Karachi , tempat ia mendirikan semacam apotek gratis bagi penduduk Karachi berpenghasilan rendah .	Edhi lahir di Bantva , Gujarat , India Britania pada tahun 1928 , kemudian ia pindah ke Karachi , tempat ia mendirikan semacam apotek gratis bagi penduduk Karachi berpenghasilan rendah .	https://id.wikipedia.org/wiki?curid=2437767	Birth-Place	/person/place/Birth-Place	e2,e1
3. <None>	Amrita	lahir di	Mumbai	.	Amrita lahir di Mumbai .	https://id.wikipedia.org/wiki?curid=1669859	Birth-Place	/person/place/Birth-Place	e2,e1
4. <None>	Fransiskus Arnold Purba	meninggal pada	1 Mei 2001	.	Fransiskus Arnold Purba meninggal pada 1 Mei 2001 .	https://id.wikipedia.org/wiki?curid=1133324	Death-Date	/person/date/Death-Date	e2,e1
5. <None>	Ging Ginanjar	meninggal di	Tangerang Selatan	adalah seorang jurnalis asal Indonesia yang berperan dalam mengamankan kebebasan pers selama masa transisi Indonesia pasca - Soeharto .	Ging Ginanjar meninggal di Tangerang Selatan adalah seorang jurnalis asal Indonesia yang berperan dalam mengamankan kebebasan pers selama masa transisi Indonesia pasca - Soeharto .	https://id.wikipedia.org/wiki?curid=2751840	Death-Place	/person/place/Death-Place	e2,e1
6. <None>	Anthony Oliver Scott	adalah seorang	jurnalis	dan kritikus film Amerika .	Anthony Oliver Scott adalah seorang jurnalis dan kritikus film Amerika .	https://id.wikipedia.org/wiki?curid=2380868	Occupation	/person/job/Occupation	e2,e1
etc.

#### Contact us
If you need this dataset, you can contact us:
- Joan Santoso : joan@stts.edu
- Miranda Laurencia : miranda1@mhs.stts.edu
- Ananta Tio : anantatio.01@gmail.com
