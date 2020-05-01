# Toolbox
Doraemon pouch of snippets, tricks and hacks 

## JS

### Falsy

```javascript
// falsy: false,undefined,null,0,NaN,''
// not falsy: {}, [],'0','false',-1
```
### Shorter ternaries
```javascript
x ? x : y  => x || y 
x ? false : true  =>  !x
x ? true : false  =>  !!x
```
### Array methods
```javascript
const people = [
  {
    id:1,
    name:'alice',
    job:'engineer'
  },
  {
    id:2,
    name:'bob',
    job:'engineer'
  },
  {
    id:3,
    name:'charlie',
    job:'doctor'
  }
]
people.some(p=>p.id===1) //true
people.every(p=>p.job==='doctor') //true
people.find(p=>p.job==='engineer')// {alice}
people.filter(p=>p.name==='engineer')// [{alice},{bob}]
```

## Chrome DevTools
### Edit pages live
`document.designMode='on'`

- ### Filter network requests
`status-code:200` or (NOT)`-method:GET`

