1)a) and b)
class Movie {
  constructor(title,studio,rating){
    this.title = title;
    this.studio = studio;
    this.rating = rating;
    if(Movie.rating === "PG"){
        return Movie;
    }
  }
}

1)c) 
let getPG = (str3) => {
  str3 = [];
  for(let i=0;i<str2.length;i++){
    str3 = str2;
    if(str3[i].rating === "PG"){
       console.log(str3[i]);
    }
  }
  return str3;
}

c) and d)
var m1 = new Movie("Casino Royale","Eon Productions","PG13");
var m2 = new Movie("Vaaranam Aayiram","GVM","PG");
var m3 = new Movie("Velayudam","AVM","PG");
var m4 = new Movie("Vinaaithandi Varuvaaya","AVM","PG13");
var str2=[];
str2.push(m1);
str2.push(m2);
str2.push(m3);
str2.push(m4);

getPG(str2);

