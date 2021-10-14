## Objects 

``` javascript
let product = {
  name: 'headphones',
  price: 120,
  doesItWork: false,
  previousOwner: 'Bob'
};

delete product.previousOwner
product.doesItWork = true

if(product.price > 100) {
  product.discountPercentage = 10
}

product.price -= product.price * (product.discountPercentage/100)

for (let key in product) {
  console.log(product[key]); 
}
  
if ('discountPercentage' in product) {
    console.log(`We got some ${product.name} on sale for just $${product.price}, that's ${product.discountPercentage}% off!`)
  }


----------------------

let user = { 
  name: 'Bob',
  surname: 'Martin',
  age: 25,
  address: {
    country: "USA"
  }
}

function printBio(user) {
  return `This is ${user.name} ${user.surname} from ${user.address.country}.`
}
```
