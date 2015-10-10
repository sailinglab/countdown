# countdown

Academic deadlines countdown for Sailors. 

## How to contribute

1. Click [index.html](https://github.com/sailinglab/countdown/edit/gh-pages/index.html) to start editing
2. Add your conference details below line 10. The conferences are eventually sorted according to their deadlines so it doesn't matter where you insert the new conference. 
3. Scroll down, click the green button **Commit changes**. 

## Data format

```javascript
deadlines.push({
  venue: "ICML",
  area: "Machine Learning",
  deadline: moment("2016-02-06 23:59:00 +0000", "YYYY-MM-DD HH:mm:ss Z"),
  website: "http://icml.cc/2016/",
  approx: 1,
});
```

- `venue`: name of the conference
- `area`: field of research
- `deadline`: deadline of the conference. You only need to edit the datetime string. The 4-digit suffix is for UTC offsets, for example `−0500` for EST. See [UTC offsets][1] and [Timezone abbreviations][2]. 
- `website`: optional, conference website
- `approx`: optional, warning message will be displayed if this field is set

[1]: https://en.wikipedia.org/wiki/List_of_UTC_time_offsets
[2]: https://en.wikipedia.org/wiki/List_of_time_zone_abbreviations
