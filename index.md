## Ceci est un site crée en 2 minutes

crédits : `Gabiel Bournizien`
<SCRIPT LANGUAGE="JavaScript">
visitnd=1;
cook = document.cookie;
var VisitName;
function detectCookie() {
place = cook.indexOf("visitor=",0);
if (place <= -1) {
while (VisitName == "" || VisitName == null || VisitName == 'Votre nom ici') {
VisitName = prompt('Entrez votre nom. Il nous permettra de vous identifier lors de vos prochaines visites.','Votre nom ici');
}}
else {
end = cook.indexOf(";",place)
if (end <= -1) {
VisitName = cook.substring(place+8,cook.length);
}
else {
VisitName = cook.substring(place+8,end);
}}
plac2 = cook.indexOf("nbvisit=",0);
if (plac2 <= -1) {
visitnd = 1;
}
else {
end2 = cook.indexOf(";",plac2)
if (end2 <= -1) {
visitnd = cook.substring(plac2+8,cook.length);
}
else {
visitnd = cook.substring(plac2+8,end2);
}
visitnd ++;
}
CreateCookie();
}
dateExp = new Date(2020,11,11);
dateExp = dateExp.toGMTString();
function CreateCookie() {
document.cookie = 'visitor=' + VisitName + '; expires=' + dateExp + ';';
document.cookie = 'nbvisit=' + visitnd + '; expires=' + dateExp + ';';
}
</SCRIPT>
