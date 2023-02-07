<template>
    <nav id="sidemenu">
        <button>Collapse All</button>
        <button>Expand All</button>

<a href="">Test</a>
<a href="">Test</a>

    </nav>
</template>
<style scoped>
#sidemenu {
    display: flex;
    grid-column-start: 2;
    grid-row-start: 1;
    grid-row-end: 2;
    flex: auto;
    flex-direction: column;
}

#sidemenu a {
    padding: 7px 8px 7px 32px;
}
</style>

