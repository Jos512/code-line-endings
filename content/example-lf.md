---
title: "Example with LF (Unix) line endings"
date:  "2020-01-10"
---

## Python code

~~~py
# Number of points scored by an athlete
bestScore = 26
lastScore = 25

# Compare last score against best score
lastIsBest = bestScore == lastScore
smallDifference = (bestScore - lastScore) <= 1

# Compare last score against best
if not lastIsBest or not smallDifference:
    print("The last score of", lastScore,
          "isn't the best score of", bestScore)
    print("Or the difference between both scores",
          "is not 1 point or less")
~~~

## C# code

~~~csharp
int ordersCurrentShipment = 20;
int newOrderSize          = 20;
int pendingOrders         = 49;
bool updateOrders         = false;

// Test value
if (updateOrders)
{
    // More comments
    if (newOrderSize > 0)
    {
        pendingOrders = pendingOrders + newOrderSize;
    }
    else
    {
        pendingOrders = pendingOrders - ordersCurrentShipment;
    }
}
~~~

## TradingView code

~~~tv
//@version=3
study(title="Columns plot example", overlay=false)

volChange = volume - sma(volume, 50)

// Plot data
plot(series=volChange, style=columns,
     color=volChange > 0 ? green : red)
~~~

## Go code

~~~go
// reverseString Reverses a string character by character
func reverseString(s string) string {
	runes := []rune(s)

    // Example commment
	for i, j := 0, len(runes)-1; i < j; i, j = i+1, j-1 {
		runes[i], runes[j] = runes[j], runes[i]
	}

	return string(runes)
}
~~~
