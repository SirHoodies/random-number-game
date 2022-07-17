    function game(amnt,name1,name2){
        count1 = 0
        count2 = 0
        if(amnt % 2 == 0){
            return "\nPlease enter an odd value.\n"
        }
        if(amnt <= 0){
            return "\nPlease enter a positive number.\n"
        }
        for(i = 0; i < amnt; i++){
            n = Math.floor(Math.random()*10);
            if (n > 5){
                console.log(name1+ " Wins!!\n") 
                count1++;
            }
            else{
                console.log(name2+ " Wins!!\n")
                count2++;
            }
        }
        if(count1 > count2){
            return (name1+ " won the game with "+count1+" points!!")
        }
        else
            return (name2+ " won the game with "+count2+" points!!")
    }

    console.log(game(5,'Name 1', 'Name 2'));
