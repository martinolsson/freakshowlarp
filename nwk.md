---
title: Character experiment
layout: page
description: Trying out a network visualisation
---

<script src="http://d3js.org/d3.v3.min.js"></script>

<script src="assets/js/jsnetworkx.js"></script>

<script>
var G = new jsnx.Graph();

G.addWeightedEdgesFrom([[2,3,10]]);
G.addStar([3,4,5,6], {weight: 5});
G.addStar([2,1,0,-1], {weight: 3});

jsnx.draw(G, {
    element: '#canvas',  
    weighted: true,
    edgeStyle: {
        'stroke-width': 10
    }
});

</script>


<canvas id="canvas"></canvas>
