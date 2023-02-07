<script setup lang="ts">
import CardItem from './CardItem.vue';
</script>

<template>
    <SideNav></SideNav>
    <CardItem>
        <template #heading>Realistic Grades</template>
        Each square is 8 meters long.
        
        Have worked a bit with civil engineering
        Steep road 15% (not recommended, but its not that rare, usually only small roads, most cars need to go in first or
        second gear for this)
        Normal road 5-7% (maximum normal grade most cars can run on top gear)
        Maglev track maximum inclination 10%
        Horizontal sprocket railway: 100%
        Vertical sprocket railway: 50%
        Worlds steepest steel-on-steel railway 14%
        Streetcar 5-7% maximum
        High speed railway/commuter rail: 3.5-4% maximum
        Norma/Freight railway: 1.5%
        Heavy freight railway: 1%
        
        Normal high loading gauge:
        Road: 4.5m+0.3m
        Normal roadway bridge thickness 1.5-2m for short spans.
        Railway: 4,65m+1,5m (central european loading gauge GC, from rail, electric)
        Normal railway bridge thickness: 2-3 m for shorter span.
        
        So a railway passing a other need just over 9 meter of vertical space, but a road going over a other needs only about
        6.5 meters.
        
        So for 10 meters high this would be the length for different grades.
        15%= 66 meter ~8 tiles
        7% = 142 meters ~18 tiles
        4% = 250 meter ~31 tiles
        1.5% = 666 meter ~83 tiles
        
        Used in video.
        24 tiles for 12 meter road 6,25% (that is pretty steep, but defently realistically, even for a real world example).
        48 tiles for 12 meter railway: 3,1% (this would be realistic for a commuter train or high speed rail, but no for freight
        trains).
        
        What the game sugests.
        6 tiles 12 meters: 25%.. for a car.. in first gear... sure... For a truck.... in crawler gear with load load.. possible.
    </CardItem>
    <CardItem>
        <template #heading>Road Distance to Buildings</template>
       <p>Many service buildings can have up 2 tiles distance from a road and still have a working connection. You can even build
    and zone in this gap</p> 
        
       <p>For example, draw a straight piece of road, place a train station next to the road. Delete the road and redraw the road
    2 tiles from the station. The “no road connection” notification will disappear and the train station will function as
    before!</p> 
    </CardItem>
    <CardItem>
        <template #heading>Card Title</template>
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
    </CardItem>
    <CardItem>
        <template #heading>Card Title 2</template>
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
    </CardItem>
    <CardItem>
        <template #heading>Card Title</template>
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
    </CardItem>
    <CardItem>
        <template #heading>Card Title 2</template>
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
    </CardItem>
    <CardItem>
        <template #heading>Card Title</template>
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
    </CardItem>
    <CardItem>
        <template #heading>Card Title 2</template>
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
    </CardItem>
    <CardItem>
        <template #heading>Card Title</template>
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
    </CardItem>
    <CardItem>
        <template #heading>Card Title 2</template>
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
    </CardItem>
    <CardItem>
        <template #heading>Card Title</template>
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
    </CardItem>
    <CardItem>
        <template #heading>Card Title 2</template>
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
    </CardItem>
    <CardItem>
        <template #heading>Card Title</template>
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
    </CardItem>
    <CardItem>
        <template #heading>Card Title 2</template>
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
    </CardItem>
    <CardItem>
        <template #heading>Card Title</template>
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
    </CardItem>
    <CardItem>
        <template #heading>Card Title 2</template>
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
    </CardItem>
</template>
