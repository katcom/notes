Week 3

# <section-title>Week 3</section-title>
**Learning Objectives**
- Explain how potential solutions to a given problemcanbe represented using a genetic encoding scheme
- Implement a genetic encoding scheme and developmental process
- Compare and contrast different genetic encoding methods
    

## Deciding Parameters

Parameter List

|     |     |     |
| --- | --- | --- |
| 0   | link-shape | cylinder / box |
| 1   | link-length | 0-1 |
| 2   | link-radius | 0-1 |
| 3   | link-recurrence | 1-4 |
| 4   | link-mass | 0-1 |
| 5   | joint-type | revolute / fixed |
| 6   | joint-parent | 0 -> num of links |
| 7   | joint-axis-xyz | 3 options \[1,0,0\], \[0,1,0\] or \[0,0,1\] |
| 8   | joint-origin-rpy-1 | 0-two-pi |
| 9   | joint origin-rpy-2 | 0-two-pi |
| 10  | joint origin-rpy-3 | 0-two-pi |
| 11  | joint origin-xyz-1 | 0-1 |
| 12  | joint origin-xyz-2 | 0-1 |
| 13  | joint origin-xyz-3 | 0-1 |
| 14  | control-waveform | sine/pulse/ramp |
| 15  | control-amp | 0-0.25 |
| 16  | control-freq | 0-1 |

Phase 1:

Make a flat directed graph, with recurrence shown as paths between two nodes. Create links from gene and decide the parent link name.

```
flat_links = []
iterate over genes
    for each gene create a link
        - assign each link an unqiue name
        - decide parent link
        - add it to flat link array
```

Phase 22:

Make a expanded directed graph, with recurrences shown as they are(expanded).

Expanding thecore link types into a complete list of links using the recursion and parent link parameters

<style>
section-title{
    color:black;
	text-align:center;
	display: flex;
    justify-content: center;
	background:white;
}
section-content {
	display:flex;
    text-indent:1em;
}
p {
    text-indent:1em;
}
</style>