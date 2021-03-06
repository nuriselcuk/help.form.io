---
title: Resources
book: intro
weight: 301
chapter: explore
slug: resources
---
Resources are reusable objects that can be used to create complex data structures within your application. The fields within a resource can be reused within other forms, as well as linked together to create complex nested resource relationships.

One example is a user resource with login and register forms.

#### Resource

  - User(user)
    - Name field (name)
    - Email field (email)
    - Password field (password)
    
#### Forms

  - Register
    - user.name
    - user.email
    - user.password
  - Login
    - user.email
    - user.password
    
Another example is having multiple resources embedded in the same form. This example has a customer, product, and order resources with an order form.

#### Resources

  - Customer (customer)
    - name
    - address
  - Product (product)
    - id
    - description
    - price
  - Order (order)
    - ordernum
    - date
    - total
    
#### Form

  - Order Form
    - customer.name
    - customer.address
    - product.id
    - product.description
    - product.price
    - order.ordernum
    - order.date
    - order.total

Resources are very similar to forms in the way that they are built, their rendering, and their APIs. There is one fundamental difference and that is that resource fields can be embedded in other resources or forms.