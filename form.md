---
___
layout: form.liquid
title: User Update
---

<ul>
  <li><a href="index.md">Home</a></li>
</ul>

<form>
    <label for="name">Name:</label>
    <input type="name" id="name" name="name">
    <label for="email">Email:</label>
    <input type="email" id="email" name="email">
    <button>Update</button>
<form>

<script>
    const email = document.getElementById("email")
    email.addEventListener("input", function (event){
if (email.validity.typeMismatch) {
    email.setCustomValidity("E-mail Address Required!")
    } else {
        email.setCustomValidity("");
        alert("Details Updated Successfully!")
    }});
</script>