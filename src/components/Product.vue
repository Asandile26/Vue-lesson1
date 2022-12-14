<template>
    <h1>product</h1>
    <div class="Product">
        <div id="productbody">
            <div>
                <div class="st">
             
                    <div v-for="product in products" :key="product">
                        <div class="card" style="width: 18rem;">
                        <img :src="product.image" class="card-img-top" alt="food" style="height:35vh;">
                        <div class="card-body">
                        <h5 class="card-title">{{product.id}}</h5>
                        <p class="card-text">{{product.food}}</p>
                        <p class="card-text">{{product.price}}</p>
                        <a href="#" class="btn btn-primary">Add</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
    </div>
</template>
<script>
export default { name: 'productPanel',
data:function() {
    return {

        products: [{id: 0,
            food: "umngqusho",
            price: 50,
            image: "https://i.postimg.cc/fLB0ZL5f/download-1.jpg"
        },
        {
            id: 1,
            food: "umbona",
            price: 50,
            image: "https://i.postimg.cc/2S69fbw2/image0-9.jpg"
        },
        {
            id: 2,
            food: "isophu",
            price: 50,
            image: "https://i.postimg.cc/W48ny2R0/b1f7bba2b7c16c6913cbc988aa89c170.jpg"
        },
        {
            id: 3,
            food: "umfino",
            price: 50,
            image: "https://i.postimg.cc/h42GtNnM/umfino.jpg"
        },
    
        {
            id: 4,
            food: "variety",
            price: 50,
            image: "https://i.postimg.cc/fWqwNX7r/4b.jpg"
        },
    ]
}
}
    

    
}
</script>
<style scoped>

.st{
    width:100vw;
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
    margin-top: 50px;
}
.st > *{
    margin: 1%;
}
h1{
    text-align: center;
    
}
    
</style>