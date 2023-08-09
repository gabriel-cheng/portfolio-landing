<script setup lang="ts">
import { onMounted } from 'vue';

onMounted(() => {
    createHabilityBox();
});

function createHabilityBox() {
    const habilityes = [
        { name: "JavaScript", "icon": "/ferramentas/javascript.png" },
        { name: "TypeScript", "icon": "/ferramentas/typescript.png" },
        { name: "Java", "icon": "/ferramentas/java.png" },
        { name: "MongoDB", "icon": "/ferramentas/mongodb.png" },
        { name: "HTML5", "icon": "/ferramentas/html.png" },
        { name: "CSS", "icon": "/ferramentas/css.png" },
        { name: "Node.js", "icon": "/ferramentas/nodejs.png" },
        { name: "Vue.js", "icon": "/ferramentas/vuejs.png" },
        { name: "Tailwindcss", "icon": "/ferramentas/tailwind.png" },
    ];

    for(let i in habilityes) {
        const habilidadesContent = document.querySelector(".habilidades-content") as HTMLDivElement;
        const box = document.createElement("div");
        box.classList.add("box");
    
        const boxTitle = document.createElement("div");
        boxTitle.classList.add("box-title");
    
        const boxIcon = document.createElement("div");
        boxIcon.classList.add("box-icon");
    
        const h2 = document.createElement("h2");
        const img = document.createElement("img");
        img.classList.add("icon");

        h2.textContent = habilityes[i].name;
        img.src = habilityes[i].icon;

        boxTitle.appendChild(h2);
        boxIcon.appendChild(img);

        box.appendChild(boxTitle);
        box.appendChild(boxIcon);

        habilidadesContent.appendChild(box);
    }
}

</script>

<template>
    <section id="habilidades">
        <div class="habilidades-subcontainer">
            <div class="habilidades-title">
                <h1>habilidades</h1>
            </div>
            <div class="habilidades-content"></div>
        </div>
    </section>
</template>

<style>
#habilidades {
    width: 100%;
    display: flex;
    justify-content: center;
    margin: 90px 0 0 0;
}
.habilidades-title {
    margin: 0 0 80px 0;
}
.habilidades-title > h1 {
    font-size: 4rem;
    color: #fff;
    text-align: center;
}
.habilidades-content {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 60px;
}
.box {
    width: 140px;
    aspect-ratio: 1;
    background-color: #212121;
    border-bottom: 4px solid var(--purple-background);
    border-radius: 35px 0 0 0;
    cursor: pointer;
    transition: 0.2s ease-in-out;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}
.box-title {
    font-size: 2.8rem;
    padding: 13px 0;
    color: var(--purple-background);
}
.box:hover {
    transform: scale(1.1);
    transition: 0.2s ease-in-out;
}
.icon {
    width: 50px;
    aspect-ratio: 1;
}
</style>