<script>
import Button from "./Button.vue";

export default {
    name: 'Pricing',

    components:{
        Button
    }
}
</script>

<template>
    <div class="container text-center py-4">
        <h2>Pricing Plans</h2>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Voluptates rerum at labore? Expedita, illum molestias?
        </p>

        <Button/>

        <table class="table table-bordered">
            <thead>
                <tr>
                    <th scope="col" class="border" width="200px">Save up to 40% <br> by paying <br> weekly</th>
                    <th scope="col" class="box">
                        <img src="../assets/img/h5-custom-icon-7.png" alt="">
                        <div class="info">
                            Standard 
                            <span class="d-block">$12</span>
                        </div>
                    </th>
                    <th scope="col" class="box ">
                        <img src="../assets/img/h5-custom-icon-8.png" alt="">
                        <div class="info">
                            Professional 
                            <span class="d-block">$59</span>
                        </div>
                    </th>
                    <th scope="col" class="box">
                        <img src="../assets/img/h5-custom-icon-9.png" alt="">
                        <div class="info">
                            Advances 
                            <span class="d-block">$88</span>
                        </div>
                    </th>
                </tr>
            </thead>
            <tbody>
                <tr >
                    <th scope="row" class="fw-normal">Number of courses</th>
                    <td>2</td>
                    <td>4</td>
                    <td>6</td>
                </tr>
                <tr>
                    <th scope="row" class="fw-normal">Time</th>
                    <td>15 Days</td>
                    <td>30 Days</td>
                    <td>30 Days</td>
                </tr>
                <tr>
                    <th scope="row" class="fw-normal">Web Designing</th>
                    <td class="check"><i class="fa-solid fa-check"></i></td>
                    <td class="check"><i class="fa-solid fa-check"></i></td>
                    <td class="check"><i class="fa-solid fa-check"></i></td>
                </tr>
                <tr>
                    <th scope="row" class="fw-normal">Human-Centered Design</th>
                    <td class="check"><i class="fa-solid fa-check"></i></td>
                    <td class="check"><i class="fa-solid fa-check"></i></td>
                    <td class="check"><i class="fa-solid fa-check"></i></td>
                </tr>
                <tr>
                    <th scope="row" class="fw-normal">Basic Marketing</th>
                    <td><i class="fa-solid fa-xmark"></i></td>
                    <td class="check"><i class="fa-solid fa-check"></i></td>
                    <td class="check"><i class="fa-solid fa-check"></i></td>
                </tr>
                <tr>
                    <th scope="row" class="fw-normal">Python for Everybody</th>
                    <td><i class="fa-solid fa-xmark"></i></td>
                    <td class="check"><i class="fa-solid fa-check"></i></td>
                    <td class="check"><i class="fa-solid fa-check"></i></td>
                </tr>
                <tr>
                    <th scope="row" class="fw-normal">Android Developer</th>
                    <td><i class="fa-solid fa-xmark"></i></td>
                    <td><i class="fa-solid fa-xmark"></i></td>
                    <td class="check"><i class="fa-solid fa-check"></i></td>
                </tr>
                <tr>
                    <th scope="row" class="fw-normal">Business English</th>
                    <td><i class="fa-solid fa-xmark"></i></td>
                    <td><i class="fa-solid fa-xmark"></i></td>
                    <td class="check"><i class="fa-solid fa-check"></i></td>
                </tr>
                <tr>
                    <th scope="row" ></th>
                    <td>
                        <button type="submit" class="btn text-uppercase border fw-semibold px-4">Get it now </button>
                    </td>
                    <td>
                        <button type="submit" class="btn text-uppercase border fw-semibold px-4 active">Get it now </button>
                    </td>
                    <td>
                        <button type="submit" class="btn text-uppercase border fw-semibold px-4">Get it now </button>
                    </td>
                </tr>
            </tbody>
        </table>
    </div>
</template>


<style lang="scss" scoped>
@use '../assets/scss/variables' as *;

table{
    width: 800px;
    margin: auto;
}
.box{
    background-color: $bg-light_blue;
}
.check{
    color: $txt-blue_light;
}

button:hover{
    background-color: $bg-blue;
    color: $txt-light;
}
</style>