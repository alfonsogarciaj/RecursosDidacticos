### Centrar un div

```css
main{
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center
}
```

### Animación tres barras

```html
<button>
  <div></div>
  <div></div>
  <div></div>
</button>

``` 

```css
button {
display: flex;
flex-direction: column;
width: 3rem;
height: 3rem;
border: 0;
background: transparent;
gap: .65rem;

button > div {
background: black;
height: 2px;
width: 100%;
border-radius: 5px;
transition: all .5s;
transform: left;
}

button:hover div:first-child {
transform: rotate(45deg);
}

button:hover div:nth-child(2){
opacity: 0;
}

button:hover div:last-child{
transform: rotate(-45deg);
}

```

### Fijar algo al hacer scroll

```css
.header{
position: sticky;
}
```
