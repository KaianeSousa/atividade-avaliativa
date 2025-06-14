

### ✅ Acessibilidade
```js
document.querySelectorAll('img:not([alt])').forEach(img => {
  img.alt = '';
  img.setAttribute('aria-hidden', 'true');
});
```

### ✅ Troca de tema
```js
btnTema.addEventListener('click', function() {
  document.body.classList.toggle('tema-escuro');
  localStorage.setItem('tema', document.body.classList.contains('tema-escuro') ? 'escuro' : 'claro');
});

```

