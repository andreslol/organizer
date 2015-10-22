# organizer
read n1;
read n2;
read n3;
list num;
num.push(n1);
num.push(n2);
num.push(n3);
counter = (num.size() - 1);
coun = 0;
con = 0;
for(var i = 0; i < num.size();1){
	if(con == num.size()){
		println "lol"
		i = num.size();
	}
	if(i < ((num.size()) - 1)){
		counter -= i;
		for(var e = i + 1;e < num.size();1){
			if(num[i] == 0){
				e = num.size(); 
			}
			else if(num[i] < num[e]){
				e = num.size(); 
			}
			else{
				coun += 1;
			}
		}	
		if(coun == counter){
			println "hola"
			println num.get(i);
			num[i] = 0;
			i = 0;
			coun = 0;
			con += 1;	
		}
	coun = 0;
	}
	if(i == (num.size() -1)){
		counter = (num.size() - 1);
		for(var o = i - 1; o >= 0;0){
			if(num[i] < num[o]){
				o = 0;
			}
			else{
				coun += 1;
			}
			o -= 1;
		}
		if(coun == counter){
			println "hola"
			println num.get(i);
			con += 1;
			num[i] = 0;
			i = 0;
			coun = 0;	
		}
	coun = 0;
	}
}
