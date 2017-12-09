

NumPy offers some benefits over Python lists, such as: **being more compact**, **faster access** in reading and writing items, being **more convenient** and **more efficient**.

* NumPy array is a central data structure of the numpy library. The library’s name is actually short for “Numeric Python” or “Numerical Python”.

However, you should know that, on a structural level, an array is basically nothing but pointers. It’s a combination of a memory address, a data type, a shape and strides:
* The **data** pointer indicates the memory address of the first byte in the array. An example output of **print(my_2d_array.data)** is **<memory at 0x7fcc627f52d0>**
* The data type or **dtype** pointer describes the kind of elements that are contained within the array. **int64** is an example output on invoking array.dtype
* The **shape** indicates the shape of the array. Example output of array.shape is **(2, 4)**
* The **strides** are the number of bytes that should be skipped in memory to go to the next element. If your strides are (10,1), you need to proceed one byte to get to the next column and 10 bytes to locate the next row. **(32, 8)** is an example output.

Or, in other words, an array contains information about the raw data, how to locate an element and how to interpret an element.
