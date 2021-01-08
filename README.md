# Web Design for a Manufacturing Company
## AIM: 
To design a static website for a chip manufacturing company.

## DESIGN STEPS:
### Step 1: 
Requirement collection.
### Step 2:
Creating the layout using HTML and CSS.
### Step 3:
Updating the sample content.
### Step 4:
Choose the appropriate style and color scheme.
### Step 5:
Validate the layout in various browsers.
### Step 6:
Validate the HTML code.
### Step 6:
Publish the website in the given URL.

## PROGRAM:

### base.html
```
{% load static %}
<!DOCTYPE html>
<html lang="en">

<head>
    <title>Silicon Private Limited</title>
    <link rel="stylesheet" href="{% static 'css/layout.css' %}">
    <link rel = "icon" href ="{% static 'img/titleicon.png' %}" type = "image/x-icon"> 
              
</head>

<body>
    <div class="container">
    <div class="banner">
        Silicon Private Limited.
    </div>
    <div class="menu">
        <div class="menuitem"><a href="/home">Home</a></div> 
        <div class="menuitem"><a href="/products">Products</a></div> 
        <div class="menuitem"><a href="/people">People</a></div>
        <div class="menuitem"><a href="/contact">Contact Us</a></div> 
    </div><div class="content">
    {% block content %}    
    {% endblock  %}
    </div>
    <div class="footer">
        Copyright © 2020 Silicon Private Limited, Developed by KUMARAVEL V.
    </div>
    </div>
</body>

</html>
```

### home.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="homecontent">    
    <h1>About Us</h1>
    <img src="/static/img/building2.jpeg" alt="Building">
    <div class="contenttext">
    Silicon Pvt Ltd, provides a broad range of semiconductor and infrastructure software applications. Some of Silicon's core technologies and products include:
    <ul>
        <li>Memory Chips</li>
        <li>SATA HDD</li>
        <li>SATA SSD </li>
        <li>Broadband Modems</li>
        <li>Wifi Devices</li>
        <li>Switching Devices</li>
        <li>Optical Sensors</li>
    </ul> 
    </div>
    </div>
{% endblock  %}
```
### products.html
```
{% extends "website/base.html" %}

{% block content %}
    <div class="productcontent">    
    <h1>Our Premium Products</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c1.jpg" alt="product image">
            </div>
            <div class="itemname">4GB DDRA4 laptop memory</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/c2.jpg"  alt="product image">
            </div>
            <div class="itemname">1TB Laptop HDD</div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/sata ssd.jfif"  alt="product image">
            </div>
            <div class="itemname">WD Green 240 GB 2.5 inch SATA III Internal Solid State Drive</div>
            <div class="itemprice">Price: Rs.2300.00 </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/optical.jfif"  alt="product image">
            </div>
            <div class="itemname">optical sensor</div>
            <div class="itemprice">Price: Rs.4150.00 </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/wifi device.jfif"  alt="product image">
            </div>
            <div class="itemname">wifi device</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/switch.jfif"  alt="product image">
            </div>
            <div class="itemname">switch </div>
            <div class="itemprice">Price: Rs.50.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/battry.jfif"  alt="product image">
            </div>
            <div class="itemname">Silicon battery </div>
            <div class="itemprice">Price: Rs.5000.00 </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/processor.jfif"  alt="product image">
            </div>
            <div class="itemname">Silicon processor</div>
            <div class="itemprice">Price: Rs.3500.00 </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/watch.jfif"  alt="product image">
            </div>
            <div class="itemname">Silicon watch</div>
            <div class="itemprice">Price: Rs.500.00 </div>
        </div>
         <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/microchip.jfif"  alt="product image">
            </div>
            <div class="itemname">Silicon microchip</div>
            <div class="itemprice">Price: Rs.800.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/spray.png"  alt="product image">
            </div>
            <div class="itemname">Silicon spray</div>
            <div class="itemprice">Price: Rs.500.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/lic.jfif"  alt="product image">
            </div>
            <div class="itemname">Silicon liquid and powder</div>
            <div class="itemprice">Price: Rs.700.00 </div>
        </div>
    </div>
    </div>
{% endblock  %}

```
###PEOPLE.HTML
```
{% extends "website/base.html" %}

{% block content %}
 <div class="productcontent">    
    <h1>our peoples</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/forbe.jfif" alt="product image">
            </div>
            <div class="itemname">FORBE</div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/sachin.jfif"  alt="product image">
            </div>
            <div class="itemname">sachin</div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/viswa.jfif"  alt="product image">
            </div>
            <div class="itemname">vishwanathan anand</div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/sundar picai.jfif"  alt="product image">
            </div>
            <div class="itemname">sundarpichai</div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/mukesh ambani.jfif"  alt="product image">
            </div>
            <div class="itemname">mukeshamboney</div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/kalanidhi.jfif"  alt="product image">
            </div>
            <div class="itemname">kalanidhi</div>
        </div>
    </div>
    </div>
{% endblock  %}

```
###CONTACT.HTML
```
{% extends "website/base.html" %}

{% block content %}

<h1>contact details</h1> 
<h2>silicon group of companies</h2>
    <h3>4th avnue,,adyar,chennai</h3>
   <h3> email:siliconsgc07@gmail.com</h3>
    <h3> mobile:7898654334</h3>
    <h3>land-line:044-765478</h3>

{% endblock  %}
```
###
## OUTPUT:
![output](./static/img/output1.jpg)

![output](./static/img/output2.jpg)

## CODE VALIDATION REPORT:
![output](./static/img/report1.jpg)

![output](./static/img/report2.jpg)
## RESULT:
Thus a website is designed for the chip manufacturing company and is hosted in the URL http://kumaravel.student.saveetha.in:8000/. HTML code is validated.