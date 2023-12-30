# Web Design for a Software Product Company

## AIM:

To design a static website for a software product company company.

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

## PROGRAM :

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
        Copyright © 2020 Silicon Private Limited.
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
    Silicon Pvt Ltd, provides a broad range of semiconductor and infrastructure software applications that serve the data center, networking, software, broadband, wireless, and storage and industrial markets. Common applications for its products include: data center networking, home connectivity, broadband access, telecommunications equipment, smartphones, base stations, data center servers and storage, factory automation, power generation and alternative energy systems, displays, and mainframe operations and management, and application software development. Some of Silicon's core technologies and products include:
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
    </div>
    <h1>RAM</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/ram1.jpg" alt="product image">
            </div>
            <div class="itemname">HyperX Fury 8GB Desktop Memory</div>
            <div class="itemprice">Price: Rs.3300.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/ram2.jpg"  alt="product image">
            </div>
            <div class="itemname">ADATA GAMMIX D30 Desktop Memory</div>
            <div class="itemprice">Price: Rs.3450.00 </div>
        </div>
    </div>
    <h1>SATA HDD</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/hdd1.jpg" alt="product image">
            </div>
            <div class="itemname">Seagate BarraCuda 1TB HDD</div>
            <div class="itemprice">Price: Rs.3820.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/hdd2.jpg"  alt="product image">
            </div>
            <div class="itemname">Western Digital WD Blue 2TB HDD</div>
            <div class="itemprice">Price: Rs.4999.00 </div>
        </div>
    </div>
    <h1>SATA SSD</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/ssd1.jpg" alt="product image">
            </div>
            <div class="itemname">Western Digital WD Green 240 GB SSD</div>
            <div class="itemprice">Price: Rs.2524.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/ssd2.jpg"  alt="product image">
            </div>
            <div class="itemname">Crucial BX500 240GB 3D SSD</div>
            <div class="itemprice">Price: Rs.1811.00 </div>
        </div>
    </div>
    <h1>Broadband Modems</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/modem1.jpg" alt="product image">
            </div>
            <div class="itemname">TP-LINK TD-W8961N Wireless N300 ADSL2+ Wi-Fi Modem Router</div>
            <div class="itemprice">Price: Rs.1279.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/modem2.jpg"  alt="product image">
            </div>
            <div class="itemname">TP-Link Archer C50 AC1200 Dual Band Wireless Cable Router</div>
            <div class="itemprice">Price: Rs.1999.00 </div>
        </div>
    </div>
    <h1>Wifi Devices</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/wifi1.jpg" alt="product image">
            </div>
            <div class="itemname">Tenda N301 Wireless-N300 Easy Setup Router</div>
            <div class="itemprice">Price: Rs.939.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/wifi2.jpg"  alt="product image">
            </div>
            <div class="itemname">TP-Link USB WiFi Adapter for PC</div>
            <div class="itemprice">Price: Rs.1149.00 </div>
        </div>
    </div>
    <h1>Switching Devices</h1>
    <div class="productitems">
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/switchingdevices1.jpg" alt="product image">
            </div>
            <div class="itemname">XORB WiFi Socket Switch Plug for Smart Devices</div>
            <div class="itemprice">Price: Rs.900.00 </div>
        </div>
        <div class="productitem"> 
            <div class="itemimage">
            <img src="/static/img/switchingdevices2.jpg"  alt="product image">
            </div>
            <div class="itemname">Wipro Wi-Fi Enabled Smart LED Bulb B22</div>
            <div class="itemprice">Price: Rs.2000.00 </div>
        </div>
    </div>
    </div>
{% endblock  %}
```
### people.html

```
{% extends "website/base.html" %}

{% block content %}
<div class="peoplecontent">
        <div class="peopleitem"> 
            <div class="peopleimage">
                <img src="/static/img/Kevin-Mitnick-crop.jpg" alt="people">
            </div>
            <h2 class="peoplename">Mr.Kevin Mitnick</h2>
            <h3 class="peopledesignation">Field Service Engineer</h3>
        </div>
        <div class="peopleitem"> 
            <div class="peopleimage">
                <img src="/static/img/elliot.jpg" alt="people">
            </div>
            <h2 class="peoplename">Mr.Elliot </h2>
            <h3 class="peopledesignation">Equipment Technician</h3>
        </div>
        <div class="peopleitem"> 
            <div class="peopleimage">
                <img src="/static/img/iman.jpg" alt="people">
            </div>
            <h2 class="peoplename">Mr.Iman Gadzhi</h2>
            <h3 class="peopledesignation">Technical Trainer</h3>
        </div>
        <div class="peopleitem"> 
            <div class="peopleimage">
                <img src="/static/img/tyrell-wellick.jpg" alt="people">
            </div>
            <h2 class="peoplename">Mr.Tyrell Wellick</h2>
            <h3 class="peopledesignation">Project Coordinator</h3>
        </div>
        <div class="peopleitem"> 
            <div class="peopleimage">
                <img src="/static/img/joel-brown.jpg" alt="people">
            </div>
            <h2 class="peoplename">Mr.Joel Brown</h2>
            <h3 class="peopledesignation">Product Support Engineer</h3>
        </div>
        <div class="peopleitem"> 
            <div class="peopleimage">
                <img src="/static/img/ali.jpg" alt="people">
            </div>
            <h2 class="peoplename">Mr.Ali Abdaal</h2>
            <h3 class="peopledesignation">Integration Engineer</h3>
        </div>
</div>
{% endblock %}
```

### contact.html

```
{% extends "website/base.html" %}

{% block content %}
<img src="/static/img/contact.jpg" style="background-repeat: no-repeat;margin-left: 45%;margin-right: 40%;margin-top:2%;width: 100px;" alt="contact">
<div class="contact">
    <br>Silicon Private Limited.,<br>
    1/223, Silicon Valley,<br>
    <a href="mailto:someone@example.com" style="text-decoration: none;color: black;">E-mail: someone@example.com</a><br>
    <a href="tel:+4733378901" style="text-decoration: none;color: black;">Phone: +47 333 78 901</a>
</div>
{% endblock %}
```

## OUTPUT:
![293230053-94c5ebca-a4d0-4809-b376-4c4ca7f07ea2](https://github.com/monishr288/productcompanywebsite/assets/147474049/d56bca9d-26b6-4251-a147-557ddd889839)

![293230078-f85e62c5-fffb-4faa-ac61-dcaaf5e6064d](https://github.com/monishr288/productcompanywebsite/assets/147474049/da48a165-e02f-4237-9e6a-d2e9d6021344)

![293230092-09079344-c9e0-4fe9-a594-41239f754734](https://github.com/monishr288/productcompanywebsite/assets/147474049/1d105573-ed0a-4079-aa08-39589d803b71)

![293230094-88cc5f98-c403-40ab-b984-6f503f6502c9](https://github.com/monishr288/productcompanywebsite/assets/147474049/18f3a5a8-7d4c-46d0-9e13-73087b3f32db)

![293230105-6190cf04-817f-43a8-b2a6-a3b50dbc0aa2](https://github.com/monishr288/productcompanywebsite/assets/147474049/cf1eb375-9157-4c2c-9a01-cd8c1b392e94)




## Result:

Thus a website is designed for the software product company and the HTML,CSS code are validated.
