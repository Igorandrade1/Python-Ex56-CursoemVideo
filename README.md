# Python-Ex56-CursoemVideo
Solution for exercise 56 of the video course


Python Exercise 56: Develop a program that reads the name, age, and gender of 4 people. At the end of the program, show: the average age of the group, what the oldest man's name is, and how many women are under 20 years old.




ages = 0
count = 0
menname = ''
menage = 0
fem = 0
countfem = 0
for c in range(1, 5):
    print('{} PESSOA'.format(c))
    name = str(input("Type it the name of {} person: ".format(c))).strip()
    age = int(input("Type it the age of {} person: ".format(c)))
    sex = str(input("Type it the sex of {} person: ".format(c))).lower().strip()
    ages += age
    average = ages / 4
    if sex == 'masculino' or sex == 'masc' or sex == 'm':
        count += 1
        if age > menage and 'masculino' or sex == 'masc' or sex == 'm':
            menage = age
            menname = name
    if age < 20 and sex == 'feminino' or sex == 'fem' or sex == 'f':
        countfem += 1





print(" There are {} men in the group, The name of the oldest man in the group is {}, and his age is {}".format(count, menname, menage))
print("The average age of the group is {} ".format(average))
print(" {} women are under 20 years old".format(countfem))
