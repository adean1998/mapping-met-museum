---
layout: default
---

# Project Description
This project seeks to highlight biases and patterns in the Metropolitan Museum of Art's collecting practices by mapping the locations of their "Highlights" works. The Met "Highlights" are objects that the museum describes as "popular or important." This type of subjective classification is prone to bias on the part of those who are selecting these works, and by mapping their locations of origins, we can determine if biases are present and if they are location- or culture-based. 
### Small image

![Highlights](https://github.githubassets.com/images/highlights.png)

## Research Question
_Can mapping the locations of origin for the Met’s “Highlights” demonstrate biases or other patterns in the museum’s collecting and curation practices?_

# Rationale Statement
Museums' collecting and curation practices are inherently biased, especially at large museums with objects from a range of cultures. In the United States, museums often prioritize the display and study of works from white, Western societies. Through data visualization, this project attempts to determine whether the objects that the Met considers significant are mostly from these cultures, or if any other patterns emerge from the data.
# Workflow
This project uses the Metropolitan Museum of Art's API to map works' locations/cultures of origin via Google My Maps.
1. Research Met API
2. Extract object data & create CSV files with data
3. Edit CSV files
4. Upload to Google My Maps

## Research Met API
Gaining an understanding of the Met API and its data is crucial to utilizing it properly. The Met "Highlights" are listed in the API and searchable.

## Extract object data & create CSV files
The Met's "Highlights" are 
I created a dataframe with all of the Highlights objects on the API and included the following information
* Title
* Artist
* Artist gender
* Earliest & Latest date of creation 
* Department
* Culture
* Country

I then filtered the data, removing all objects that did not have a country associated with them. In a preliminary version, I also added ISO_Alpha3 country codes to the dataframe, in case this made mapping simpler. 

## Edit CSV Files
In this step, I opened the CSV file on Google Sheets and looked over the information on objects to make sure it was correct. I also reformatted the CSV so that it looked cleaner in Google My Maps. I added object links to each object in the list so that a user can easily access the object on the Met's website. Finally, I created a new set of CSV files with the objects separated by department. 

## Upload to Google My Maps
I created two Google My Maps with the data. The first has all of the objects in one layer, color-coded by department. The second has the objects divided into layers by department. 

# Project & Findings

2,765 Objects in API listed as “Highlights,” only 895 had country information
Over 1,000 “Highlights” lack country/culture information
Some countries have no objects in the “Highlights” section at all
31 countries represented in MCRW department
The Michael C. Rockefeller Wing encompasses many very different countries/cultures
Met’s data can be inconsistent and overly general
Any museum data requires careful review, ideally by field experts

# Further Uses / Future Directions

There are several pontential enhancements for this project:
- Research could be performed to determine more specific locations of origin for objects (rather than just their country)
- Contributions from experts and cultural representatives
- Fine-grained data could be created about objects and their corresponding cultures
Create map that reflects concentrations of objects
Determine other trends in the Met's collecting practices, such as the gender of the artists, the cultural classifications, or the number of objects in each department.

# Files List
- A csv 
- A Plotly map showing the data

[Link to another page](./another-page.html).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# Header 1

This is a normal paragraph following a header. GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.

## Header 2

> This is a blockquote following a header.
>
> When something is important enough, you do it even if the odds are not in your favor.

### Header 3

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```ruby
# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end
```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
