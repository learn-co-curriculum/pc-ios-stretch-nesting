##Stretch Material

**Nested Data Structures** 

Dictionaries and Arrays can occur inside of other dictionaries and arrays. Its data structure inception!
 
```swift
//nested array:
salad_ingredients = [
      ["romaine", "kale", "spring mix"],
      ["tomatoes", "avocado", "beets"],
      ["vinaigrette", "ranch", "ginger-soy"]
    ]
```
This data would be much better represented as a dictionary (explain why). Can you help me convert it?
```swift
//arrays nested in a dictionary:
  salad_ingredients =[ 
  lettuce: ["romaine", "kale", "spring mix"],
  veggie: ["tomatoes", "avocado", "beets"],
  dressing:["vinagrette", "ranch", "ginger-soy"] 
]
```
**Random Numbers** 

To generate a random number in Swift, within a range, it's super simple:

```swift
arc4random_uniform(n)
```

That will create a random number from 0 through n-1

Put in English, if you wanted to randomly roll a dice (which has 6 possible sides)...

```swift
let diceRoll = Int(arc4random_uniform(7))
```

When working with arrays' count function, you have to take an extra step and make it of type UInt32 (seriously, don't worry about why it's not very important)

```swift
let array = ["Frodo", "sam", "wise", "gamgee"]
let randomIndex = Int(arc4random_uniform(UInt32(array.count)))
print(array[randomIndex])
```

**UIPickerViews**

UIPickerViews are an awesome way to help your user select out of a possibility of options. They also work extremely well with a list (*cough* *cough* an Array) of data. Check out this awesome [tutorial](http://sourcefreeze.com/ios-uipickerview-example-using-swift/) on how to get started with a UIPickerView.
