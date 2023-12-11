<nav class="menu">
    <ul>
        <!-- Other Menu Items -->
        <li><a href="Home">Home</a></li>
        <li><a href="About">About</a></li>
        <li><a href="Services">Services</a></li>
        <li><a href="Contacts">Contacts</a></li>      
    </ul>
    
</nav>

<style>
.menu {
/*   background: #eee; */
  display: block;
  position: fixed;
  right: 0px;
  width: 100%;
  transition: 0.5s;
}
ul li {
    background: #f5f5f5; /* Light background for each item */
    margin-bottom: 10px; /* Space between items */
    padding: 10px; /* Padding inside each item */
    border-radius: 5px; /* Rounded corners */
    
}

.menu ul {
  list-style: none; 
  text-decoration: none;
  display: flex;
  justify-content: flex-end;
}

.menu li {
  /* display: inline; */
  padding: 15px;
  border-bottom: 1px solid #ccc;
  text-decoration: none;
}

.menu a {
  text-decoration: none;
}


</style>
<slot />