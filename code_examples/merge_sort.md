### Merge Sort implemented in Kotlin

```kotlin
fun main() {
    // testweise ausgeben
    println(listOf(38, 27, 43, 3, 9, 82, 10).mergeSort())
}

/**
 * This extension method sorts a [List] containing comparable
 * objects by using the merge sort sorting algorithm.
 * @return a sorted list
 */
fun <T : Comparable<T>> List<T>.mergeSort(): List<T> {

    if (size <= 1) return this

    // liste in zwei hälften teilen
    val middleIndex = size / 2
    val firstHalf = subList(0, middleIndex)
    val secondHalf = subList(middleIndex, size)

    return ComparableUtils.merge(firstHalf.mergeSort(), secondHalf.mergeSort())

}

object ComparableUtils {

    /**
     * Returns a merged list containing all elements of both halfs provided.
     * If both halfs are sorted, the result (return value of this function)
     * will also be sorted.
     * @param firstHalf sorted first half to merge with the [secondHalf]
     * @param secondHalf sorted second half to merge with the [firstHalf]
     */
    fun <T : Comparable<T>> merge(
            firstHalf: List<T>,
            secondHalf: List<T>
    ): List<T> {

        var currentIndexFirst = 0
        var currentIndexSecond = 0

        val mergedList = mutableListOf<T>()

        // sortierte listenhälften nach index miteinander vergleichen und mergen
        while (currentIndexFirst < firstHalf.size && currentIndexSecond < secondHalf.size) {
            if (firstHalf[currentIndexFirst] <= secondHalf[currentIndexSecond]) {
                mergedList += firstHalf[currentIndexFirst]
                currentIndexFirst++
            } else {
                mergedList += secondHalf[currentIndexSecond]
                currentIndexSecond++
            }
        }

        // es gibt nichts mehr zu vergleichen - den rest einfach hinzufügen
        while (currentIndexFirst < firstHalf.size) {
            mergedList += firstHalf[currentIndexFirst]
            currentIndexFirst++
        }
        while (currentIndexSecond < secondHalf.size) {
            mergedList += secondHalf[currentIndexSecond]
            currentIndexSecond++
        }

        return mergedList

    }

}
```