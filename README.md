# Trip Planner

This tool filters Google Maps places based on an input query and exports them to a CSV file. 

## Getting started

- Install all dependencies with:

```
$ pip install -r requirements.txt
```

- Rename the file `secrets.ini.example` to `secrets.ini` and add the Google Maps API key.
> Note: This script requires Python 3.6+

## Usage example

For fetching a list of attractions in London, we can do:

```
$ python fetch.py --directory output/england/london --rating 4.5 --reviews 5000 --operator and --query "attractions in London"
```

This will return all the attractions in London that have a rating >= 4.5 *and* a review count >= 5000. The output will contain the following columns:

```
| name                | coordinates                         | types                                                                           | rating  | formatted address                                           | summary                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           | url                                               | reviews   |
|-------------------  |------------------------------------ |-------------------------------------------------------------------------------- |-------- |-----------------------------------------------------------  |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |-------------------------------------------------  |---------  |
| Tower Bridge        | (51.5054564, -0.07535649999999999)  | tourist_attraction, point_of_interest, establishment                            | 4.7     | Tower Bridge Rd, London SE1 2UP, United Kingdom             | Tower Bridge is a combined bascule and suspension bridge in London, built between 1886 and 1894. The bridge crosses the River Thames close to the Tower of London and has become an iconic symbol of London. Because of this, Tower Bridge is sometimes confused with London Bridge, situated some 0.5 mi (0.80 km) upstream. Tower Bridge is one of five London bridges now owned and maintained by the Bridge House Estates, a charitable trust overseen by the City of London Corporation. It is the only one of the Trust's bridges not to connect the City of London directly to the Southwark bank, as its northern landfall is in Tower Hamlets.The bridge consists of two bridge towers tied together at the upper level by two horizontal walkways, designed to withstand the horizontal tension forces exerted by the suspended sections of the bridge on the landward sides of the towers. The vertical components of the forces in the suspended sections and the vertical reactions of the two walkways are carried by the two robust towers. The bascule pivots and operating machinery are housed in the base of each tower. Before its restoration in the 2010s, the bridge's colour scheme dated from 1977, when it was painted red, white and blue for Queen Elizabeth II's Silver Jubilee. Its colours were subsequently restored to blue and white.The bridge deck is freely accessible to both vehicles and pedestrians, whereas the bridge's twin towers, high-level walkways and Victorian engine rooms form part of the Tower Bridge Exhibition, for which an admission charge is made. The nearest London Underground tube stations are Tower Hill on the Circle and District lines, London Bridge on the Jubilee and Northern lines and Bermondsey on the Jubilee line, and the nearest Docklands Light Railway station is Tower Gateway. The nearest National Rail stations are at Fenchurch Street and London Bridge.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 | https://en.wikipedia.org/wiki/Tower_Bridge        | 90038     |
| Westminster Abbey   | (51.4992921, -0.1273097)            | church, tourist_attraction, place_of_worship, point_of_interest, establishment  | 4.6     | 20 Deans Yd, Westminster, London SW1P 3PA, United Kingdom   | "Westminster Abbey, formally titled the Collegiate Church of Saint Peter at Westminster, is a large, mainly Gothic abbey church in the City of Westminster, London, England, just to the west of the Palace of Westminster. It is one of the United Kingdom's most notable religious buildings and the traditional place of coronation and burial site for English and, later, British monarchs. The building itself was a Benedictine monastic church until the monastery was dissolved in 1539. Between 1540 and 1556, the abbey had the status of a cathedral. Since 1560, the building is no longer an abbey or a cathedral, having instead the status of a Church of England ""Royal Peculiar""âa church responsible directly to the sovereign.According to a tradition first reported by Sulcard in about 1080, a church was founded at the site (then known as Thorn Ey (Thorn Island)) in the seventh century, at the time of Mellitus, a Bishop of London. Construction of the present church began in 1245, on the orders of King Henry III.Since the coronation of William the Conqueror in 1066, all coronations of English and British monarchs have been in Westminster Abbey. There have been 16 royal weddings at the abbey since 1100. As the burial site of more than 3,300 persons, usually of predominant prominence in British history (including at least sixteen monarchs, eight Prime Ministers, poets laureate, actors, scientists, and military leaders, and the Unknown Warrior), Westminster Abbey is sometimes described as 'Britain's Valhalla', after the iconic burial hall of Norse mythology."                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | https://en.wikipedia.org/wiki/Westminster_Abbey   | 26551     |
| London Bridge       | (51.5078788, -0.0877321)            | tourist_attraction, subpremise, point_of_interest, establishment                | 4.5     | London SE1 9RA, United Kingdom                              | "Several bridges named London Bridge have spanned the River Thames between the City of London and Southwark, in central London. The current crossing, which opened to traffic in 1973, is a box girder bridge built from concrete and steel. It replaced a 19th-century stone-arched bridge, which in turn superseded a 600-year-old stone-built medieval structure. This was preceded by a succession of timber bridges, the first of which was built by the Roman founders of London.The current bridge stands at the western end of the Pool of London and is positioned 30 metres (98 ft) upstream from previous alignments. The approaches to the medieval bridge were marked by the church of St Magnus-the-Martyr on the northern bank and by Southwark Cathedral on the southern shore. Until Putney Bridge opened in 1729, London Bridge was the only road-crossing of the Thames downstream of Kingston upon Thames. London Bridge has been depicted in its several forms, in art, literature, and songs, including the nursery rhyme ""London Bridge Is Falling Down"".The modern bridge is owned and maintained by Bridge House Estates, an independent charity of medieval origin overseen by the City of London Corporation. It carries the A3 road, which is maintained by the Greater London Authority. The crossing also delineates an area along the southern bank of the River Thames, between London Bridge and Tower Bridge, that has been designated as a business improvement district."                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   | https://en.wikipedia.org/wiki/London_Bridge       | 28441     |
| Tower of London     | (51.50811239999999, -0.0759493)     | tourist_attraction, point_of_interest, establishment                            | 4.6     | St Katharine's & Wapping, London EC3N 4AB, United Kingdom   | "The Tower of London, officially Her Majesty's Royal Palace and Fortress of the Tower of London, is a  historic  castle located on the north bank of the River Thames in central London. It lies within the London Borough of Tower Hamlets, which is separated from the eastern edge of the square mile of the City of London by the open space known as Tower Hill. It was founded towards the end of 1066 as part of the Norman Conquest of England. The White Tower, which gives the entire castle its name, was built by William the Conqueror in 1078 and was a resented symbol of oppression, inflicted upon London by the new ruling elite. The castle was used as a prison from 1100 (Ranulf Flambard) until 1952 (Kray twins), although that was not its primary purpose. A grand palace early in its history, it served as a royal residence. As a whole, the Tower is a complex of several buildings set within two concentric rings of defensive walls and a moat. There were several phases of expansion, mainly under kings Richard I, Henry III, and Edward I in the 12th and 13th centuries. The general layout established by the late 13th century remains despite later activity on the site.The Tower of London has played a prominent role in English history. It was besieged several times, and controlling it has been important to controlling the country. The Tower has served variously as an armoury, a treasury, a menagerie, the home of the Royal Mint, a public record office, and the home of the Crown Jewels of England. From the early 14th century until the reign of Charles II, a procession would be led from the Tower to Westminster Abbey on the coronation of a monarch. In the absence of the monarch, the Constable of the Tower is in charge of the castle. This was a powerful and trusted position in the medieval period. In the late 15th century, the castle was the prison of the Princes in the Tower. Under the Tudors, the Tower became used less as a royal residence, and despite attempts to refortify and repair the castle, its defences lagged behind developments to deal with artillery.The peak period of the castle's use as a prison was the 16th and 17th centuries, when many figures who had fallen into disgrace, such as Elizabeth I before she became queen, Sir Walter Raleigh, and Elizabeth Throckmorton, were held within its walls. This use has led to the phrase ""sent to the Tower"". Despite its enduring reputation as a place of torture and death, popularised by 16th-century religious propagandists and 19th-century writers, only seven people were executed within the Tower before the World Wars of the 20th century. Executions were more commonly held on the notorious Tower Hill to the north of the castle, with 112 occurring there over a 400-year period. In the latter half of the 19th century, institutions such as the Royal Mint moved out of the castle to other locations, leaving many buildings empty. Anthony Salvin and John Taylor took the opportunity to restore the Tower to what was felt to be its medieval appearance, clearing out many of the vacant post-medieval structures. In the First and Second World Wars, the Tower was again used as a prison and witnessed the executions of 12 men for espionage. After the Second World War, damage caused during the Blitz was repaired, and the castle reopened to the public. Today, the Tower of London is one of the country's most popular tourist attractions. Under the ceremonial charge of the Constable of the Tower, and operated by the Resident Governor of the Tower of London and Keeper of the Jewel House, the property is cared for by the charity Historic Royal Palaces and is protected as a World Heritage Site."  | https://en.wikipedia.org/wiki/Tower_of_London     | 63183     |
```

This file can then be imported to [Google My Maps](https://drive.google.com/open?id=1OdZq0vA46Oi8sny75zG0Z-MNVURjCSh6&usp=sharing), which is described in the [section](#Imorting-to-Google-My-Maps) below. The output will be similar to:

![Google My Maps](my-maps.png)

### Refining a search query

Items can be exluded from a search query using the `--exclude` parameter. Considering our previous example, if we want to exclude all parks from our search query, the command can be modified as:

```
$ python fetch.py --directory output/england/london --rating 4.5 --reviews 5000 --operator and --query "attractions in London" --exclude park
```

More details can be viewed with the `--help` parameter:

```
$ python fetch.py --help

usage: fetch.py [-h] [--query QUERY] [--directory DIRECTORY] [--rating RATING]
                [--reviews REVIEWS] [--operator {and,or}]
                [--exclude {park,point_of_interest,establishment,museum,library,church,art_gallery,political} [{park,point_of_interest,establishment,museum,library,church,art_gallery,political} ...]]
                [--language {en,fr,de}] [--summary-length SUMMARY_LENGTH]

optional arguments:
  -h, --help            show this help message and exit
  --query QUERY         Search query for Google Maps API
  --directory DIRECTORY
                        Output directory
  --rating RATING       Minimum rating of the place(s)
  --reviews REVIEWS     Minimum review count of the place(s)
  --operator {and,or}   Operation to perform between ratings and reviews
                        count.
  --exclude {park,point_of_interest,establishment,museum,library,church,art_gallery,political} 
                        Exclude the places from the query result
  --language {en,fr,de}
                        Language of the Wikipedia link
  --summary-length SUMMARY_LENGTH
                        Limit the number of sentences in place summary.
```

## Importing to Google My Maps

The following blog post describes how the CSV files can be imported to Google My Maps.
- [Programmatically organising your backpacking trip using Google My Maps](https://adl1995.github.io/programmatically-organising-your-backpacking-trip-using-google-my-maps.html)
