<script>
export default {
    name: 'Learning'
}
</script>

<template>
    <div class="container">
        <div class="row my-5">
            <div class="col-3 py-1">
                <div id="list-example" class="list-group">
                    <a class="list-group-item list-group-item-action active" href="#list-item-1">What We Do</a>
                    <a class="list-group-item list-group-item-action" href="#list-item-2">Degree Programme</a>
                    <a class="list-group-item list-group-item-action" href="#list-item-3">Carrer Achievements</a>
                    <a class="list-group-item list-group-item-action" href="#list-item-4">Personal Managment</a>
                    <a class="list-group-item list-group-item-action" href="#list-item-4">Steps To Success</a>
                    <a class="list-group-item list-group-item-action" href="#list-item-4">Knowledge Transfer</a>
                </div>
            </div>
            <div class="col-9 list px-5 py-2">
                <div data-bs-spy="scroll" data-bs-target="#list-example" data-bs-smooth-scroll="true"
                    class="scrollspy-example" tabindex="0">
                    <h2 id="list-item-1" class="py-2">Learning Possibilities</h2>
                    <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aliquam aliquid, eos animi, ipsa quis pariatur beatae qui cum perferendis nihil at necessitatibus alias architecto hic possimus accusamus blanditiis libero omnis distinctio quas recusandae sed obcaecati cumque! Maiores ducimus provident similique?</p>

                    <ul class="py-5">
                        <li>
                            <i class="fa-solid fa-check"></i>
                            We enrich lives through learning.
                        </li>
                        <li>
                            <i class="fa-solid fa-check"></i>
                            Maximizing potential through individual attention.
                        </li>
                        <li>
                            <i class="fa-solid fa-check"></i>
                            The trusted name for specialized training.
                        </li>
                        <li>
                            <i class="fa-solid fa-check"></i>
                            People teach. People learn. This is where they connect.
                        </li>
                    </ul>
                </div>
                <div class="image">
                    <img src="../assets/img/h12-tabs-icon-1.png" width="100px" alt="">
                </div>

            </div>
        </div>
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

a{
    padding: 1rem;
    font-weight: 500;
}
.list{
    position: relative;
}

ul{
    list-style: none;
 
    li i{
        color: lightgreen;
        padding: 0.7rem 1rem;
    }
}
.image{
    position: absolute;
    bottom: 3rem;
    right: 10rem;
}

.active{
    background-color:transparent;
    color: $bg-blue;
    border: none;
    border-left: 7px solid $bg-blue;
}
</style>