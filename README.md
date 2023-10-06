# KBC_using_python

question_list = [
"How many continents are there?",
"What is the capital of India?",
"NG mei kaun se course padhaya jaata hai?"
]

options_list = [
["Four", "Nine", "Seven", "Eight"],
["Chandigarh", "Mumbai", "Chennai", "Delhi"],
["Software Engineering", "Counseling", "Tourism", "Agriculture"]
]
op_list= [
    ['seven','eight'],
    ['Mumbai','Delhi'],
    ['Software Engineering','Counseling']
]
stn_list=[1,2,1]
solution_list = [3, 4, 1]

    
print('WELCOME TO KON BANEGA CROREPATI!!!')
i=0
k=0
while i<len(question_list):
    print("aapka sawal hai")
    print(i+1,question_list[i])

    print('aapke options hai:')
    j=0
    while j<len(options_list[i]):
        print(j+1,options_list[i][j])
        j+=1
    n=0   
    c=0
    a=input('Do you want 50-50 Lifeline??: y/n: ')
    if a=='y' and c==1:
        print('you have already used your life line')
        print(j+1,options_list[i][j])

    elif a=="y":
        c+=1
        while n<len(op_list[i]):
            print(op_list[i][n])
            n+=1
        b=int(input('your answer:'))
        if b==stn_list[k]:
           print('------CONGRATS! you win!------')
           k+=1
        else:
           print("ohh no !you loose :/\n better luck next time.")
           break
    else:
              
        a=int(input('your answer:'))
    if a==solution_list[k]:
        print("------CONGRATS! you win!------")
        k+=1
    else:
        print("ohh no !you loose :/\n better luck next time.")
        break
        
    i+=1
 
