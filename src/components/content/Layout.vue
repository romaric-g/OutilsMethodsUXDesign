<template>
    <main>
        <div class="menu">
            <Menu />
        </div>
        <div class="content">
            <Content title="entretiens">
                <Description />
                <Items />
            </Content>
            <Content title="Autre titre" reverse="true">
                <Description />
                <Items />
            </Content>
            <Content title="BrainStorming">
                <Description />
                <Items />
            </Content>
        </div>
    </main>
</template>

<script>
import Content from "./Content";
import Menu from "./../menu/Menu";

import Items from "./elements/Items"
import Description from "./elements/Description"

export default {
    name: "layout",
    components: {Menu, Content, Items, Description}
}
</script>

<style lang="scss">
main {
    display: grid;
    grid-template-columns: auto 1fr;
    position: sticky;

    & > .menu {
        position: sticky;
        top: 0;
        height: 100vh;
    }
}
</style>