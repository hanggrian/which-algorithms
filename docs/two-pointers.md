Make use of two pointers to solve problems that require traversing a sequence of elements.

Common problems:

- [Two Sum](https://hanggrian.github.io/grind-leetcode/two-sum)
- [Container With Most Water](https://hanggrian.github.io/grind-leetcode/container-with-most-water)
- [Trapping Rain Water](https://hanggrian.github.io/grind-leetcode/trapping-rain-water)

<div class="grid" markdown>
=== "Groovy"
    ```groovy
    int[] twoSum(int[] nums, int target) {
        for (var i = 0; i < nums.length; i++) {
            for (var j = i + 1; j < nums.length; j++) {
                if (nums[j] == target - nums[i]) {
                    return new int[]{i, j}
                }
            }
        }
        return null
    }
    ```
=== "Java"
    ```java
    int[] twoSum(int[] nums, int target) {
        for (int i = 0; i < nums.length; i++) {
            for (int j = i + 1; j < nums.length; j++) {
                if (nums[j] == target - nums[i]) {
                    return new int[]{i, j};
                }
            }
        }
        return null;
    }
    ```
=== "JavaScript"
    ```javascript
    function twoSum(nums, target) {
      for (let i = 0; i < nums.length; i++) {
        const complement = target - nums[i];
        if (nums.slice(i + 1).includes(complement)) {
          return [i, nums.indexOf(complement, i + 1)];
        }
      }
      return undefined;
    }
    ```
=== "Python"
    ```python
    def two_sum(self, nums: list[int], target: int) -> list[int] | None:
        for i, num in enumerate(nums):
            complement = target - num
            if complement in nums[i + 1:]:
                return [i, nums.index(complement, i + 1)]
        return None
    ```
=== "TypeScript"
    ```typescript
    function twoSum(nums: number[], target: number): number[] {
      for (let i = 0; i < nums.length; i++) {
        const complement = target - nums[i];
        if (nums.slice(i + 1).includes(complement)) {
          return [i, nums.indexOf(complement, i + 1)];
        }
      }
      return undefined;
    }
    ```

![](images/two-pointers.gif)
</div>

## Sliding window

Restrict the range of the two pointers to a certain window size or condition.

Common problems:

- [Longest Substring Without Repeating Characters](https://hanggrian.github.io/grind-leetcode/longest-substring-without-repeating-characters)
- [Minimum Window Substring](https://hanggrian.github.io/grind-leetcode/minimum-window-substring)
- Sliding Window Maximum

<div class="grid" markdown>
=== "Groovy"
    ```groovy
    int lengthOfLongestSubstring(String s) {
        if (s.isEmpty()) {
            return 0
        }
        HashSet<Character> characters = []
        var start = 0
        var end = 0
        var maxLength = Integer.MIN_VALUE
        while (end < s.length()) {
            if (characters.add(s.charAt(end))) {
                maxLength = Math.max(maxLength, characters.size())
                end++
                continue
            }
            characters.remove(s.charAt(start))
            start++
        }
        return maxLength
    }
    ```
=== "Java"
    ```java
    int lengthOfLongestSubstring(String s) {
        int i = 0;
        int j = 0;
        int maxLength = Integer.MIN_VALUE;
        Set<Character> set = new HashSet<>();
        while (j < s.length()) {
            if (set.add(s.charAt(j))) {
                maxLength = Math.max(maxLength, set.size());
                j++;
            } else {
                set.remove(s.charAt(i));
                i++;
            }
        }
        return maxLength;
    }
    ```
=== "JavaScript"
    ```javascript
    function lengthOfLongestSubstring(s) {
        if (!s) {
          return 0;
        }
        const characters = new Set();
        let start = 0;
        let end = 0;
        let maxLength = Number.MIN_SAFE_INTEGER;
        while (end < s.length) {
          if (!characters.has(s[end])) {
            characters.add(s[end]);
            end++;
            maxLength = Math.max(maxLength, characters.size);
            continue;
          }
          characters.delete(s[start]);
          start++;
        }
        return maxLength;
      }
    ```
=== "Python"
    ```python
    def length_of_longest_substring(self, s: str) -> int:
        i = 0
        j = 0
        max_length = sys.maxsize
        char_set = set()
        while j < len(s):
            if s[j] not in char_set:
                char_set.add(s[j])
                max_length = max(max_length, len(char_set))
                j += 1
            else:
                char_set.remove(s[i])
                i += 1
        return max_length
    ```
=== "TypeScript"
    ```typescript
    function lengthOfLongestSubstring(s: string): number {
        if (!s) {
          return 0;
        }
        const characters = new Set<string>();
        let start = 0;
        let end = 0;
        let maxLength = Number.MIN_SAFE_INTEGER;
        while (end < s.length) {
          if (!characters.has(s[end])) {
            characters.add(s[end]);
            end++;
            maxLength = Math.max(maxLength, characters.size);
            continue;
          }
          characters.delete(s[start]);
          start++;
        }
        return maxLength;
      }
    ```

![](images/two-pointers-sliding-window.gif)
</div>

## Fast-slow pointers

Pointers that move at different speeds to find a cycle or a specific condition.

Common problems:

- [Linked List Cycle](https://hanggrian.github.io/grind-leetcode/linked-list-cycle)
- [Sort List](https://hanggrian.github.io/grind-leetcode/sort-list)
- [Reorder List](https://hanggrian.github.io/grind-leetcode/reorder-list)

<div class="grid" markdown>
=== "Groovy"
    ```groovy
    boolean hasCycle(SinglyListNode head) {
        // visited nodes
        Set<SinglyListNode> visits = []
        for (var node : head) {
            if (!visits.add(node)) {
                return true
            }
        }
        return false
    }
    ```
=== "Java"
    ```java
    boolean hasCycle(ListNode head) {
        if (head == null || head.next == null) {
            return false;
        }
        ListNode slow = head.next;
        ListNode fast = head.next.next;
        while (fast != null && fast.next != null && slow != fast) {
            slow = slow.next;
            fast = fast.next.next;
        }
        return slow == fast;
    }
    ```
=== "JavaScript"
    ```javascript
    function hasCycle(head) {
      // visited nodes
      const visits = new Set();
      for (const node of head) {
        if (visits.has(node)) {
          return true;
        }
        visits.add(node);
      }
      return false;
    }
    ```
=== "Python"
    ```python
    def has_cycle(self, head: ListNode) -> bool:
        if not head or not head.next:
            return False
        slow = head.next
        fast = head.next.next
        while fast and fast.next and slow != fast:
            slow = slow.next
            fast = fast.next.next
        return slow == fast
    ```
=== "TypeScript"
    ```typescript
    function hasCycle(head: SinglyListNode | undefined): boolean {
      // visited nodes
      const visits = new Set<SinglyListNode>();
      for (const node of head) {
        if (visits.has(node)) {
          return true;
        }
        visits.add(node);
      }
      return false;
    }
    ```

![](images/two-pointers-fast-slow-pointers.gif)
</div>

