# ph_provinces_and_cities
Philippine Provinces &amp; Cities/Municipalities on HTML Dropdown

### Description
A very lightweight standalone javascript project which aims to help anyone who need information/data regarding Philippine provinces & cities. 

### Basic Usage
```javascript
// Basic Usage
window.onload = function() {
	
 var $ = new City();
 
 $.showProvinces('#province');
 
 $.showCities('#city');	
 
}
```
### Methods
```javascript
// @param arg: object
// will output all provinces on target dropdown id 
object.showProvinces(arg) 
```
```javascript
// @param arg: object
// will output all cities on target dropdown id 
object.showCities(arg) 

// Note: you must call the object.showProvinces(arg) before calling object.showCities(arg) 
// because object.showCities(arg) will populate according to selected province from province dropdown
// you can also omit the province dropdown by using the optional parameter of showCities 
// e.g 
object.showCities("Laguna",arg) // will output all cities of Laguna

```
### Additional Methods 
```javascript
// You can also play with the methods below (If you want to do more with the given data)

// will return all provinces (array)
console.log($.getProvinces());
	
// will return all cities (array)
console.log($.getAllCities());
	
// will return all cities under specific province (array)
console.log($.getCities("Batangas"));

// sample code for printing the array content
// will print all provinces
for(let province in cities) {
    console.log(province);
}
// will print all cities under Batangas
for(let city in $.getCities("Batangas")) {
    console.log($.getCities("Batangas")[city]);
}
// will print the entire cities of all provinces
let all = $.getAllCities();
for(let city in all) {
    console.log(all[city]);
}
```
[DEMO](https://www.marvicrm.com/scripts/ph_provinces_and_cities/demo.php)

Ang proyektong ito ay alay ko sa Republika ng Pilipinas

Salamat,<br>
Marvic R. Macalintal


[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=XM7R9M2J6BTF2)

