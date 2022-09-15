# nodred-ameren-psp-entity
This work is an attempt to bring hourly electricity rates from Ameren Illinois' PowerSmart Pricing program into node-red/home assistant for consumption. These rates change hourly and are decided daily, with tomorrow's hourly pricing being posted publicly at around 4:30pm central time (GMT-5).

Ameren PSP info/rates can be seen here https://www.ameren.com/illinois/account/customer-service/bill/power-smart-pricing/prices

I have an inject node wired up to trgger this. It will generate tomorrow's date and as long as its after 4:30pm, the HTTP request will fetch pricing for the next day.


