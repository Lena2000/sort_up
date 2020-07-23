# sort_up
//Сортировка по возрастанию

package org.apache.poi.hssf.usermodel;

import java.util.Arrays;

public class Main {

    public static void main(String[] args) {
        int[] arr = {2, 6, 3, 9, 12, 34, 67, 1};
        System.out.println(Arrays.toString(arr) + "->");
        for (int i = arr.length - 1; i > 0; i--) {
            for (int k = 0; k < i; k++) {

                if (arr[k] > arr[k + 1]) {
                    int tmp = arr[k];
                    arr[k] = arr[k + 1];
                    arr[k + 1] = tmp;

                    System.out.println(Arrays.toString(arr));
                }


            }
        }
    }
}
