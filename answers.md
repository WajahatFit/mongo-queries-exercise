# Solutions sheet

Submit your final query after each iteration:

## Iteration 1

db.users.find({},{name:1, \_id:0})

## Iteration 2

db.users.find({},{name:1, hasInsurance:true, \_id:0})

## Iteration 3

db.users.find({age: {$gte:18}})

## Iteration 4

db.users.find({country :'Italy'}, {name:1, email:1, \_id:0})

## Iteration 5

db.users.find({country: 'USA'}, {name:1, \_id:0}).limit(5)

## Iteration 6

## Iteration 7

db.users.updateOne({name:'Marissa Geller'}, {$set: {email: 'marissa@hotmail.com'}})

## Iteration 8

db.users.updateMany({country:'UK'}, {$set: {currency:'pound'}}, {upsert:true})

## Iteration 9

db.users.find({country:'UK'}, {name:1, currency:1, \_id:0})

## Iteration 10

db.users.deleteMany({age: {$gte:45}},{age:{$gte: 45}})
