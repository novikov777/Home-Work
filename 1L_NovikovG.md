//
//  main.swift
//  HW1L
//
//  Created by Геннадий Новиков on 14.12.2020.
//

import Foundation

// 1. Решение квадратного уравнения

let a:Float = 5
let b:Float = 5
let c:Float = 10
var x1:Float
var x2:Float
var d:Float
var discriminant:Float
d = b * b - (4 * a * c)
if (d >= 0){
    discriminant = sqrt(d)
    x1 = (-b + discriminant) / (2 * a)
    x2 = (-b - (discriminant)) / (2 * a)
    print(x1, x2)
} else if(d < 0){
    d = ((4 * a * c) - pow(b,2)) / (2 * a)
    print(d)
}


// 2. Площадь, периметр и гипотенуза треугольника.
var k:Double = 10
var l:Double = 10
var m:Double = 15
var n:Double
n = k + l + m
m = sqrt(pow(k,2) + pow(l,2))
print("Периметр треугольника равен", n)
print("Гипотенуза треугольника равна", m)


// 3. Вклад
var deposit:Float = 1000000
var percent:Float = 12
percent = percent / 100
var result1 = deposit + (deposit * percent)
var result2 = result1 + (result1 * percent)
var result3 = result2 + (result2 * percent)
var result4 = result3 + (result3 * percent)
var result5 = result4 + (result4 * percent)
var counter = 1
var time = [result1, result2,result3, result4, result5]
for i in time{
    print("Через \(counter) год/лет сумма вклада будет равна \(i)")
    counter += 1
}
