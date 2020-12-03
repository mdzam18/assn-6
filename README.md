## ინსტრუქცია
- დააკლონირეთ რეპოზიტორია
- გახსენით ტერმინალი და გაუშვით `sh setup.sh` ან `./setup.sh`

### development

პრერეკვიზიტები. valgrind, zip 

```sh
sudo apt-get install valgrind #ubuntu
yay -S valgrind #arch
```

build

```sh
make
```

test

```sh
./bankdriver -w4 -t1  
შექმნის 4 ნაკადს და გაუშვბეს პირველ ტესტზე.  
(7 სხვადასხვა ტესტია (-t1-დან -t7-ის ჩათვლით), გატესტვა შესაძლებელია სხვადასხვა რაოდენობის ნაკადზე.)  
valgrind --tool=helgrind ./bankdriver -r -t1 -w4
```
### შეფასება
`TODO`

### ატვირთვა
google classroom-ზე.

#### version 1 ავტომატურად
გახსენით ტერმინალი და გაუშვით `./zip.sh`

#### version 2 manual
1. დაზიპეთ ფაილები 
`account.h account.c action.h action.c bank.h bank.c bankdriver.h bankdriver.c branch.h branch.c debug.h debug.c error.h report.h report.c teller.h teller.c`. **აუცილებელია იყოს `.zip` და არა rar**. დაზიპეთ **მხოლოდ** ეს ფაილები (სხვა ფაილებში ცვლილებები არ მიიღება) და არა დირექტორია
2. დაარქვით ზიპს თქვენი მეილის id


## კითხვები და დახმარება
თუ დავალებასთან დაკავშირებით კითხვა გქონდათ ან ტექნიკური დახმარება დაგჭირდათ:
1. ნახეთ შედით github.com-ზე დავალების გვერდზე და გახსენით [`faq.md`](./faq.md) ფაილი
2. თუ FAQ-ში არ არის, გადადით github-ზე დავალების `issues` განყოფილებაში. თუ ვინმეს უკვე აქვს დამატებული თქვენი კითხვა, დააკომენტარეთ რომ თქვენც გაქვთ, თუ საჭიროდ ჩათვლით დაურთეთ error message, სისტემის მონაცემები და ა.შ
3. თუ ვერცერთგან ვერ იპოვეთ, შექმენით ახალი `issue`

