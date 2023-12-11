class Product{
  String productName;
  int price;
  
  // CONSTRUCTOR
  Product(this.productName, this.price);
}

// create an abstract class
abstract class Category{
  
  List<Product> getProducts();
  void addProducts(Product product);
  
}

// assignment : 3
class Cart implements Category{
  
  List<Product> products = [];
  
  // Assignment: 4
  @override
  List<Product> getProducts(){
    return List.from(products);
  }
  
  // Assignment: 5
  @override
  void addProducts(Product prod){
    products.add(prod);
  }
  
}


void main(){
  
  // instance creation
  Cart myCart = Cart();
  
  Product prod1 = Product("book",90);
  Product prod2 = Product("pen",90);
  
  myCart.addProducts(prod1);
  myCart.addProducts(prod2);
  
  //List<Product> cartProducts = myCart.getProducts();
  print("products in the carts are : ");
  printCart(myCart);
//   for(Product prod in cartProducts){
//     print("${prod.productName} - ${prod.price}");
//   } 
  
  Product prod3 = Product("laptop",90000);
  Product prod4 = Product("mobile",9000);
  
  myCart.addProducts(prod3);
  myCart.addProducts(prod4);
  print("Now products in the carts are : ");
  printCart(myCart);
}
  void printCart(Cart cart){
    List<Product> cartProducts = cart.getProducts();
    for(Product prod in cartProducts){
    print("${prod.productName} - ${prod.price}");
  } 
  
}
