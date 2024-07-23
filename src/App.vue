<script setup lang="ts">
</script>

<template>
  <div class="bn-container">
        <div class="bn-wrapper">
            <div id="example-element" class="img-container"></div>
            <div class="tx-container">
                <p class="tx-ex-sm">BRAND NAME</p>
                <span class="badge">featured</span>
                <p class="tx-lg">At the peak</p>
                <p class="tx-md">Lorem, ipsum dolor sit amet consectetur adipisicing elit.</p>
            </div>
            </div>
            <div class="btn-container">
                <a href="#" class="btn-style">
                    Blaze a trail
                </a>
        </div>
    </div>
</template>

<style scoped>

.bn-container {
    width:100%;
    height:372px;
    background:#1D0042;
    padding:10px;
    display:grid;
    grid-template-columns:repeat(3, 1fr);
    align-items:center;;
}

.bn-wrapper {
    display:flex;
    flex-direction:row;
    gap:20px;
    align-items:center;
    justify-content:flex-start;
    grid-column:span 2;
    padding:0 120px;
}

.bn-container .img-container {
    clip-path:circle(80px);
}

#example-element {
    background:linear-gradient(to bottom right, #f52, #05f);
    width:280px;
    height:280px;
}

#example-element:hover {
    animation-name:animation;
    animation-duration:3s;
    animation-delay:.1s;
    animation-timing-function: cubic-bezier(0.075, 0.82, 0.165, 1);
    animation-direction:reverse;
}

.bn-container .tx-container {
    padding:5px 0;
}

.bn-container .tx-container > p {
    padding:0;
    margin:0;
}

.bn-container .tx-container .tx-ex-sm {
    font-size:12px;
    font-weight:bold;
    color:white;
    text-align:left;
    text-transform:uppercase;
    display:inline-block;
}

.bn-container .tx-container .badge {
    font-size:10px;
    font-weight:light;
    background:white;
    border-radius:20px;
    padding:2px 5px;
    color:#1D0042;
    margin:0 0 0 10px;
    text-align:center;
    line-height:1em;
}

.bn-container .tx-container .tx-lg {
    font-size:30px;
    font-weight:bold;
    color:white;
    padding:0;
    margin:10px 0;
    text-align:left;
}

.bn-container .tx-container .tx-md {
    font-size:12px;
    text-align:left;
    color:white;
}

.bn-container .btn-container {
    padding:0 120px;
}

.bn-container .btn-container .btn-style {
    font-size:16px;
    font-weight:normal;
    color:#1D0042;
    background:white;
    padding:10px 30px;
    box-shadow:0 2px 2px 3px rgba(0,0,0,.5);
    text-decoration:none;
    border-radius:20px;
    transition:all .3s ease;
}

.bn-container .btn-container .btn-style:hover {
    box-shadow:0 3px 3px 5px rgba(0,0,0,1);
}

@keyframes animation {
    0%{
        background:linear-gradient(to bottom right, #f52, #05f);
    }

    80% {
      background:linear-gradient(rgb(222, 255, 34), rgb(174, 0, 255));
    }

    100% {
        background:linear-gradient(to top, rgb(255, 34, 34), rgb(230, 0, 255));
    }
}

@media (max-width: 1080px) {
  .bn-container .btn-container {
    padding:0;
}
}

</style>
