<h1>Find_Célia_a_boyfriend</h1>

<h2>👩🏻‍💻 Description</h2>
This python script is the first self-projects I worked on during my first-ever programming course at <b>McGill University</b> (shout out to COMP202!). It uses 5 criterias my closest friend in Montreal has for boyfriend selection and simple if-else statements to filter out potential matches. In the end, if the candidate is <b>✨boyfriend_material()✨</b>, he will get Célia's phone number. 
<br />

<h2>🪐 Language</h2>

- <b>Python</b>


<h2>🦠 Program Walk-Through:</h2>
This is a program that finds out if a boy suits Célia. Her 5 criterias for a boyfriend are funny, smart, taller than her, handsome, and lazy like her (prefers to stay home). 

<br/>
<br/>

- <b>Intelligence Test:</b>

```ruby
def smart_guy():
    print("Celia likes guys that are smart.")
    Mcgill_student= input("First question: Are you a McGill student? ")
    if(Mcgill_student=='yes'):
        print("Cool! What program are you in?")
        program =input()
        if(program== 'arts'):
            print("what is your GPA?")
            gpa_arts= float(input())
            if(gpa_arts < 3.6):
                print("Oh no that's too low for Celia! Sorry!:(")
            else:
                print("yay! seems like you're smart and work hard?????")
                return True
        
        elif(program=='science'):
            print("what is your GPA?")
            gpa_science= float(input())
            if(gpa_science < 3.4):
                print("Oh no looks like you lost your chance to med school:(")
            else:
                print("yay! seems like you might be smart enough for med school???")
                return True
        else:
            print("what is your GPA?")
            gpa_else= float(input())
            if(gpa_else < 3.5):
                print("Oh no that's too low for Celia! Sorry!:(")
            else:
                print("Great! Onto the next question!")
                return True
    else:
        print("Currently Celia is only interested in McGill students:( Sorry")
```

<br/>

- <b>Height Test:</b>

```ruby
def tall_guy():
    print("Celia likes guys that are tall.")
    height= float(input("Enter your height in centimeters because Celia is Canadian and I'm too lazy to calculate for you: "))
    if(height<170):
        print("Sorry but that's shorter than Celia!")
    else:
        print("Great you're tall!")
```

<br/>

- <b>Appearance Test:</b>

```ruby
def handsome_guy():
    print("Celia likes guys that are handsome")
    rate_look= float(input("On a scale of 1 to 10, how handsome would you rate yourself? "))
    if(rate_look < 5.0):
        print("Hmm you're probably not the best match!")
    else:
        print("I hope your confidence matches up with your appearance")
```

<br/>

- <b>Laziness Test:</b>

```ruby
def lazy_guy():
    print("Celia likes guys that are lazy")
    lazy=input("What is your favorite activity for a Sunday afternoon? ")
    if(lazy=='stay home' or 'stay at home' or'nothing'):
        print("same as Celia!")
        print("plot twist! The thing is, Celia lives near Stuwart Bio, so even though you should be lazy like her, you have to be a bit less lazy because you'll have to clime up the hill")
        less_lazy= input("are you willing to commit climbing up Ave. Pins everyday? ")
        if(less_lazy=='yes'):
            print("good for you! celia always have lots of food so its good excercise anyway.")
        else:
            print("ohhh what human lazyness does to you!")
    else:
        print("Too bad, Celia is very lazy and likes to stay home everyday")
```

<br/>

- <b>Humour Test:</b>

```ruby
def funny_guy():
    print("Celia likes guys that are funny, please tell us your best joke:"), input()
    print("Hmmm I'm not sure if you are funny enough for Celia, but I'll give you her number since you've past most questions!")
    print("Celia's number: ###-###-###3")
    print("Good luck with your love-adventure with Celia! She's such a smart/beautiful/nice/lazy person!")
    print("It was fun being your Cupid, if things work out for you with Celia please be my Cupid too!")
```

<br/>

- <b>Finally, find out if the candidate is <b>✨Boyfriend Material✨:</b>

```ruby
def boyfriend_material():
    participant = input("What is your name? ")
    print("Cool, nice to meet you,", participant)
    smart_guy()
    handsome_guy()
    lazy_guy()
    funny_guy()
    
boyfriend_material()
```
