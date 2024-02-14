# CSC229_assignment03_zavame
public class NewClass {

    public static int getLargest(int arr[]. int sz) {
        int iterate1 = 0;     // 1 step
        int iterate2 = 0;    // 1 step
        int largest = 0;     // 1 step
        while (iterate1 < sz - 1) {       
            iterate2++;
            if (iterate2 == sz) {
                iterate1++;
                iterate2 = iterate1;
                continue;
            }
       
            int product = arr[iterate1] * arr[iterate2];
            if (product > largest)
                largest = product;
        }
        return largest;
    }
}

// O(n^2)
