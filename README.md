# CURSO: APRENDE BLAZOR

# LECCIÓN 28: Componente NavLink

1. Abrir la aplicación con Visual Studio 2022 o VSCode

2. Código original por defecto de NavLink antes de ninguna modificación:

```razor
<div class="nav-item px-3">
    <NavLink class="nav-link" href="" Match="NavLinkMatch.All">
        <span class="bi bi-house-door-fill-nav-menu" aria-hidden="true"></span> Home
    </NavLink>
</div>
```

3. Código con el anchor tag ```<a></a>``` the HTML

```razor
<div class="nav-item px-3">
    <a class="nav-link" href="">
        <span class="bi bi-house-door-fill-nav-menu" aria-hidden="true"></span> Home1
    </a>
</div>
```

4. Modificación del Componente NavLink para incluir una clase de CSS cuando el vínculo está activo

```razor
 <div class="nav-item px-3">
     <NavLink class="nav-link" href="" Match="NavLinkMatch.All" ActiveClass="nav-active">
         <span class="bi bi-house-door-fill-nav-menu" aria-hidden="true"></span> Home2
     </NavLink>
 </div>
```

   Definimos la clase de estilo "nav-active" enlazada a la propiedad ActiveClass, en el archivo "wwwroot\app.css"

```css
.nav-active {
    font-weight: bold;
    color: red !important;
    text-decoration: underline;
}
```
