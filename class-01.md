# class 01

## Pain vs. Suffering

" All growth comes with some degree of pain, as it pulls you out of your comfort zone. The greater the growth, the greater the pain. But pain in the service of growth is a good thing, as long as that pain is what’s necessary to achieve the growth that you’re aiming for. And even better than that, this pain is only temporary. It’s what will launch you forward into the next phase of your life."

What’s my perspective?
No pain,No gain. so I really need that pain.

Why am I doing this?
having that pain that will makes me growth

Do I want what comes at the end of this journey?
Yesssssss.

Am I doing this for myself?
for something I believe it in my self, more important than me.

## big O notation

### What is an algorithm

This are steps taken to solve a problem. We are identifying patterns, creating a solution that will improve the speed of our programs.Increasing Performance matters a lot in algorithm not just writing code that works.

### What is big O notation

Big O notation is used to explain the performance or complexity of an algorithm.
we can also say, It shows how the runtime of the algorithm grows as the input grow. Example if you are in a large company that deals with a lot of user data, writing an efficient algorithm that takes less time when it runs compared to one that's takes more time.

### Why is big O notation is important

* It helps us look at the worst case scenario of an algorithm.
* Describes the time execution which is called Time complexity
* Describes the space used (memory). This is called Space complexity.

### Common Time complexities

1. O(1)
O(1) describes an algorithm that will always execute in the same time (or space) regardless of the size of the input data set.

bool IsFirstElementNull(IList< string> elements)
{
    return elements[0] == null;
}
2. O(N)
O(N) describes an algorithm whose performance will grow linearly and in direct proportion to the size of the input data set. The example below also demonstrates how Big O favours the worst-case performance scenario; a matching string could be found during any iteration of the for loop and the function would return early, but Big O notation will always assume the upper limit where the algorithm will perform the maximum number of iterations.

bool ContainsValue(IList< string> elements, string value)
{
    foreach (var element in elements)
    {
        if (element == value) return true;
    }

    return false;
}
3. O(N2)
O(N2) represents an algorithm whose performance is directly proportional to the square of the size of the input data set. This is common with algorithms that involve nested iterations over the data set. Deeper nested iterations will result in O(N3), O(N4) etc.

bool ContainsDuplicates(IList< string> elements)
{
    for (var outer = 0; outer < elements.Count; outer++)
    {
        for (var inner = 0; inner < elements.Count; inner++)
        {
            // Don't compare with self
            if (outer == inner) continue;

            if (elements[outer] == elements[inner]) return true;
        }
    }

    return false;
}
3. O(2N)
O(2N) denotes an algorithm whose growth doubles with each additon to the input data set. The growth curve of an O(2N) function is exponential - starting off very shallow, then rising meteorically. An example of an O(2N) function is the recursive calculation of Fibonacci numbers:

int Fibonacci(int number)
{
    if (number <= 1) return number;

    return Fibonacci(number - 2) + Fibonacci(number - 1);
}

### some info form video

what i learned from videos: [Names and Values in Python](https://www.youtube.com/watch?v=_AEJHKGk9ns)

1. names refer to values
2. many names can refer to one value
3. names are assigned independently
4. values live until no references.
5. assignment never copied data
6. changes are visible through all  name
7. mutable aliasing:
    * a mutable value
    * more than one name
    * the value changes
    * all names see the change
8. immutable value
    * immutable types:ints,floats,strings,tuples
9. "change" is unclear:
    * changing an int:**rebinding**: x = x + 1
    * changing a list: **mutating** nums.append(7)
    * can also **rebind** lists nums = nums + [7]
    * cant't mutate an int:ints are **immutable**
10. names have no type
11. values have no scope
