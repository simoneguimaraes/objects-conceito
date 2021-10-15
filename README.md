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

----------------


let products = [
  {
    name: 'iPhone',
    price: 799.99
  },
  {
    name: 'Samsung Galaxy S10',
    price: 900.0
  }
];

console.log(products[0].price)
console.log(products[0].name, products[1].name)
products.unshift('Xiaomi')
console.log(products)
products.pop()
console.log(products)

----------------


let student = {
  firstName: 'Ana',
  lastName: 'Blair',
  course: {
    name: 'Web Development',
    type: 'part-time'
  },
  attendedIn: 'Madrid',
  address: {
    street: 'Happy Street',
    number: 123,
    city: 'Barcelona',
    zip: 08015,
    country: 'Spain'
  }
};


console.log(`${student.firstName} moved from ${student.address.city} to ${student.attendedIn} to take ${student.course.type} ${student.course.name} course.`)
-------------------


const ironCampuses = [
  ["Mexico City", "Miami", "Sao Paulo"],
  ["Amsterdam", "Barcelona", "Berlin", "Lisbon", "Madrid", "Paris"]
];

console.log(ironCampuses[0][1]); // => Miami
console.log(ironCampuses[1][0]); // => Amsterdam
console.log(ironCampuses[1][5]); // => Paris

-------------------

let course = {
  name: 'Web Development',
  type: ['full-time', 'part-time'],
  topics: ['HTML/CSS & Responsive Design', 'JavaScript', 'MongoDB', 'Node', 'Express', 'React']
};

console.log(course.type[0])
console.log(course.topics[0], course.topics[1])
console.log(course.topics[3], course.topics[4])


console.log(course.topics[4]); 
console.log(`In Ironhack, I'll learn ${course.topics[4]}JS and ${course.topics[5]}JS.`); 

-------------------

function filterPizzas(pizzas) {
  // your code
}
  let orders =[ {type: '', size: ''}]
  if(orders.type != 'pineapple') {
    return 
  }

Input:

let pizzas = [
  { type: 'pineapple', size: 'M'},
  { type: 'pepperoni', size: 'S'},
  { type: 'pineapple', size: 'S'},
  { type: 'mushrooms', size: 'L'}
]
  
[   { type: 'pepperoni', size: 'S'}, { type: 'mushrooms', size: 'L'}  ]


function filterPizzas(pizzas) {
  let pedidos = []
  for(let contador = 0; contador < pizzas.length; contador++) {
    
    if (pizzas[contador].type != "pineapple") {
        pedidos.push(pizzas[contador])
    } 
  } return pedidos
} 



```


