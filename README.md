```js

const live = true;
var tired = "no", drinkEnergy = 0, day = 0;



while(live){
  day++; tired = "no"; drinkEnergy = 0;// new day
  switch(tired){
    case "no":
      workUntilTired(12,drinkEnergy);
      break;
    case "yes":
      drinkEnergyDrink(1);
      break;
    case "sleep":
      sleep("9h");
      break;
  }
}

function workUntilTired(avgTiredHours,energy){
  for(var i=0; i<avgTiredHours; i++){
    doWork("Coding");
    if(avgTiredHours - 1 === i) {
        if(energy === 0){
          tired = "yes";
        }else{
          tired = "sleep";
        }
    }
  }
}
```
