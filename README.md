# google-autocomplete

What does Google suggest for different names?

This was suggested by `@__apf__` in [this Tweet](https://twitter.com/__apf__/status/901093927855374336):

  Oh come on, this is what people search for? My husband? 😠

# data

List of names was sourced from Wikipedia lists. I cast around for a few
different lists of men and women. Men seem to be in mixed gender lists whereas
women are on women-only lists.

After a few searches for different lists I found:

* [List of female scientists in the 21st century](https://en.wikipedia.org/wiki/List_of_female_scientists_in_the_21st_century), females
* [List of British Jewish Scientists](https://en.wikipedia.org/wiki/List_of_British_Jewish_scientists), males and ~4 females
* [List of women in leadership](https://en.wikipedia.org/wiki/List_of_women_in_leadership), females

# methodology

1. Find a list of names on Wikipedia
2. Feed it into Google Search autocomplete
3. Parse out the bit they've added
4. Sum it up

# room for further research

Categorise the results a bit better.

eg, people in some regions tend to suggest "name linkedin" but in other regions
it is "name twitter" or "name facebook". It could also be that their celebrity
leads them to certain platforms.

I also noticed in the raw data that sometimes honorifics are added. eg "DAME name" or "name MD".

Also collapse all family members together: "son" = "daughter"; "husband" = "partner"

# results

## List of female scientists in the 21st century (female)

```
     11 + facebook
     10 + biography
      9 + cv
      8 + instagram
      8 + husband
      8 + google scholar
      7 + md
      6 + dr. 
      5 + wiki
      5 + twitter
      5 + quotes
      4 + obituary
      4 + lab
      4 + dr 
      4 + bio
      3 + stanford
      3 + pittsburgh
      3 + linkedin
      3 + harvard
```

"husband" is high on the list. Good mentions of their work ("cv", "biography",
"bio", "google scholar") and honorifics ("dr", "dr." "md").

## List of women in leadership (female)

```
     26 + net worth
     24 + husband
     23 + linkedin
     17 + twitter
     12 + biography
     10 + wikipedia
     10 + wiki
     10 + email
      9 + house
      9 + facebook
      8 + forbes
      8 + daughter
      7 + kimdir
      7 + instagram
      7 + foundation
      7 + family
      6 + son
      6 + cv
      6 + age
```

I don't know what a "kimdir" is.

This is mostly about what they have ("net worth", "house", "foundation"), their
family ("husband", "daughter", "son"), and their social media. "Forbes" can be
expected because it tends to rank women in leadership.

"age" is a bit of a concern since it really shouldn't matter.

## List of British Jewish Scientists (male)

```
     21 + quotes
     13 + books
     11 + md
     10 + obituary
      9 + biography
      7 + professor 
      6 + pdf
      6 + nobel prize
      6 + building
      5 + twitter
      5 + man
      5 + artist
      4 + ucl
      4 + er
      3 + oxford
      3 + lab
      3 + dr 
      3 + dblp
      3 + college
      3 + cambridge
```

So this mostly seems to be about what they've done, what awards they've won,
where they work. Seems reasonable for a famous name in science (male or female).

# Conclusion

Well, draw your own.

I'm not sure I like the conclusions I'm drawing.

Whether Google is drawing these from the masses and its users really do care
about whether women are married, or whether Google is just adding that to any
female sounding name.
