# HPC-assignment
## Parallel programming using OpenMP
### Types of Matrix Multiplications
#### 1. Ordinary Matrix Multiplication (OMM)
#### 2. Block Matrix Multiplication (BMM)
#### 3. Transpose of A to find the Nth Power Using OMM
#### 4. Transpose of A to find the Nth Power Using BMM
### Graphs for different types of Mlitplications
#### 1. Runtime vs Matrix sizes by fixing number of threads
#### 2. Runtime vs Threads by fixing the matrix size
***

### 1. Ordinary Matrix Multiplication (OMM)
Code Description
- Initialization of Matrix A and Matrix B with random values.
- Specify the number of threads for Parallalization.
- Using OpenMP to parallalization the Matrix Multiplication.
- Measuring the time elapsed for the Multiplication process.
- Gives the elapsed time in seconds as output.
- 
### Graphs
1. Runtime vs. Matrix Sizes by fixing number of threads (Matrix Sizes - 512, 1024, 2048)
 
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/63877442-8b6a-476a-8f2c-49583b05a7a5)

![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/5c42398d-520c-4ca9-9e51-3c8f7b44c89f)

![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/66105e0c-f2cc-4123-b8e1-056f54856361)

![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/d372123d-1209-468e-b73c-3d4ede6f6a72)

![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/f20abd89-b5c7-4d3c-85b9-a40a5bdf0863)

![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/dedc2ea5-0e4d-499e-a779-2d6af41660c8)

![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/5ffd962a-f78f-4e22-aa10-ae9162607d35)

![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/3a47c633-54f6-4f5d-b9c2-b174af118bea)


2. Runtime vs. Threads by fixing the Matrix Size. (Threads varies as 1,2,4,6,8,10,12,14,16)

![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/f8cb0630-0f5c-41ca-b556-190238530585)

![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/019f2576-37a2-44ae-97b3-38a18ed463f3)

![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/4bd8e986-c07c-446a-8236-81a770d3e9dc)
***

### 2. Block Matrix Multiplication (BMM) using block sizes: 4,8,16,32,64.
- Initialization of Matrices A and B:

We start by initializing matrices A and B with random values. This step ensures that our matrices have valid data for multiplication.
User-Defined Thread Count:

We give you the flexibility to specify the number of threads to be used for parallelization. This allows you to optimize performance based on the number of available CPU cores or other considerations.

- Parallel Matrix Multiplication with OpenMP:

The core of our implementation lies in parallelizing the matrix multiplication using OpenMP. OpenMP allows us to harness the power of multiple threads and divide the workload efficiently.
To achieve this, we break the matrix into smaller blocks and distribute these blocks among the threads for simultaneous computation.

- Exploring Block Sizes:

We understand that different block sizes can have varying impacts on performance. Therefore, our program lets you specify the block size.
Matrix multiplication is carried out by taking into account these block sizes, allowing you to experiment and analyze the effects on execution time.

- Timing the Process:

To evaluate the efficiency of our BMM implementation, we measure the elapsed time for the entire matrix multiplication process.
We utilize functions like gettimeofday() to ensure accurate timing and capture the start and end times.

- Outputting Elapsed Time:

After completing the matrix multiplication, we provide you with the elapsed time in seconds.
This information is invaluable for assessing the efficiency of our BMM algorithm under different configurations.


### Graphs
a. Runtime vs. Threads by fixing the Matrix Size. (Threads varies as 1,2,4,6,8,10,12,14,16)
- For Matrix odf size 2048 and blocks size varies as 4,8,16,32,64

![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/5c874997-165d-4a07-baa5-8a6f24ff7132)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/e86d7b05-3525-48fd-bdfd-fae56f11d0ee)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/f139f1db-e423-4dc5-96d0-7307c6eab731)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/f5723213-757b-4ce5-9897-b15c9bd1968a)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/7d3a5a67-035b-4749-a22c-7735d47ea526)

- For Matrix odf size 1024 and blocks size varies as 4,8,16,32,64
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/356fae9e-1e08-4041-8968-04e9a72241d7)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/09155ba2-c729-4fa2-acf9-0793fbe071e5)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/af65d7ba-5a79-4f8b-b3cb-4c93fe23f517)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/2260237a-40ce-4121-878c-70b9db5802f0)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/5043c738-c014-4420-aed7-3c81044521da)

- For Matrix odf size 512 and blocks size varies as 4,8,16,32,64
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/887c06cc-bccf-41fc-ae2f-d358e45cd927)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/97a52c21-4d6d-4923-a702-96c145fff419)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/6cacc7af-5c94-4675-9e1f-22f001472132)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/7fac381c-6ec8-4f5c-9520-50dffbc776f0)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/8e8da420-986f-413e-848e-942f300a565c)

b. Runtime vs. Matrix Sizes by fixing number of threads (Matrix Sizes - 512, 1024, 2048)
- in this we kept thread number as constant in each case and changed the matix sizes
  
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/812a9dfe-80e2-43f6-8870-59312a111960)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/51cee879-79fd-4e6a-8be3-5bf661216dc7)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/449a5c3a-ab16-4d7c-8299-148d4cf5f1e7)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/766dc641-53a7-4a0d-9f93-49f1702e465a)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/91b2f021-2e02-44bd-9903-00c3098268ea)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/9ab3ea33-9cb5-43dc-a2f2-ef1cd5e4dc1c)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/533b99d2-4fbf-4d41-8f6f-4a4f6f094df2)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/9daa48fe-3b05-462f-8459-4ed91296d006)
***

##### 3. Tranpose of A to find nth Power using OMM.
- Initialization of Matrix A :

We start by initializing matrices A with random values. This step ensures that our matrices have valid data for multiplication.

-User-Defined Thread Count:

We give you the flexibility to specify the number of threads to be used for parallelization. This allows you to optimize performance based on the number of available CPU cores or other considerations.

- Transpose of A
  - In the regular matrix multiplication, basically we multply row of one matrix with column of another 
    matrix, instead in this transpose approach if we transpose atleast one matrix in matrix multiplication 
    process we can directly multply row with row, this helps to reduce the run time.
  - in oue approach we varied n between 2-16 where N is exponent of Am A is the matrix with order varies 
    between 512 & 2048.
  - Here exponent implies number of times of multiplication of matrix A with itself.  

- Parallel Matrix Multiplication with OpenMP:

The core of our implementation lies in parallelizing the matrix multiplication using OpenMP. OpenMP allows us to harness the power of multiple threads and divide the workload efficiently.
To achieve this, we break the matrix into smaller blocks and distribute these blocks among the threads for simultaneous computation.

- Outputting Elapsed Time:

After completing the matrix multiplication, we provide you with the elapsed time in seconds.
This information is invaluable for assessing the efficiency of our BMM algorithm under different configurations.

### Graphs
a. Runtime vs. Threads by fixing the Matrix Size. (Threads varies as 1,2,4,6,8,10,12,14,16)

- EXPONENTS i.e, no of Matrixes being multiplied in an itreation will be from 2 to 10.
  
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/c6d0f8f3-8170-4f53-b4c1-f639872a0538)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/0c04f21e-7a17-41c1-921b-dac7adfba153)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/df39d37e-feb1-4e23-bafd-0156d56dbab3)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/3460fb8f-4f18-4f7c-a9c3-7bca2be6e8a3)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/444c95db-5812-47da-812b-428e2887fd57)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/0bda8504-5f36-4550-9b4d-f44ad90d1fc9)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/21952b4d-111a-4c4e-830a-b811f23801b4)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/7b4724cd-ada2-49ed-9a9e-4da09fadad85)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/3c4cfca4-4008-46fa-b32f-ede796a24e8b)


##### 4. Tranpose of A to find nth Power using BMM.

We start by initializing matrices A with random values. This step ensures that our matrices have valid data for multiplication.
- Transpose of A
  - In the regular matrix multiplication, basically we multply row of one matrix with column of another 
    matrix, instead in this transpose approach if we transpose atleast one matrix in matrix multiplication 
    process we can directly multply row with row, this helps to reduce the run time.
  - in oue approach we varied n between 2-16 where N is exponent of Am A is the matrix with order varies 
    between 512 & 2048.
  - Here exponent implies number of times of multiplication of matrix A with itself.
 
- Exploring Block Sizes:

We understand that different block sizes can have varying impacts on performance. Therefore, our program lets you specify the block size.
Matrix multiplication is carried out by taking into account these block sizes, allowing you to experiment and analyze the effects on execution time.

- Timing the Process:

To evaluate the efficiency of our BMM implementation, we measure the elapsed time for the entire matrix multiplication process.
We utilize functions like gettimeofday() to ensure accurate timing and capture the start and end times.

- Outputting Elapsed Time:

After completing the matrix multiplication, we provide you with the elapsed time in seconds.
This information is invaluable for assessing the efficiency of our BMM algorithm under different configurations.


### Graphs
a. Runtime vs. Threads by fixing the Matrix Size. (Threads varies as 1,2,4,6,8,10,12,14,16)
- For Matrix odf size 2048 and blocks size varies as 4,8,16,32,64
  
EXPONENT - 2 & MATRIX SIZE - 2048

![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/4a3147a1-1901-438d-93cb-a19b61075892)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/2690cf6c-7ef4-4ded-acc9-922609801320)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/11d1d2dc-cc6f-4555-b6cc-bf9802316b17)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/4683f399-5a40-4f94-803f-cfbac8b38205)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/66f68fbd-0624-48e1-95df-dc120d351938)

EXPONENT - 2 & MATRIX SIZE - 1024
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/5de24dfb-fa4d-4224-b169-742dcea846c0)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/52a4733b-e081-46b6-9533-cf5b512c590b)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/1e9f8236-35ca-42bd-bfe6-9f14207f8bca)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/ede5bbfe-e23f-41e7-9f22-6012c9a684a0)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/7d154082-c43f-48c2-a99b-97748094baf9)

EXPONENT - 2 & MATRIX SIZE - 512
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/4f38ec7d-2294-4ef2-af67-11a24411add4)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/8ceb1fd4-dccc-4654-923a-21c04bca226e)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/3b7b2568-ca64-43c5-80d6-dfc58d137b4e)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/63841bb9-9eed-41f1-a7e4-bd961c9a1265)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/5631bacc-1ad9-47ba-9414-3a76ea5b44a0)

EXPONENT - 8 & MATRIX SIZE - 512
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/8a49a19d-efea-4c53-9869-a269938350f4)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/704bb6c3-2885-4bbf-9f08-b07817d6ec45)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/6b265646-dac9-4f33-afa8-7d81209493dd)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/e7a7ef9f-0987-4864-aa81-a88d4e27d048)

EXPONENT - 8 & MATRIX SIZE - 1024
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/c60838e3-e85c-429c-b533-d7db5a1dcc3a)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/b3d88e76-d1c6-42f5-b4b5-347aa2c51dc3)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/8a7d8947-18a2-4ae4-9659-6520f5a5ba83)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/ee1dabaf-0d02-497f-8694-9490b9489768)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/7f109861-c063-4c36-b135-c4f0386621ec)

EXPONENT - 8 & MATRIX SIZE - 2048
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/f476e0cd-f658-4683-912e-e0f75f9e0cbd)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/6e2ea145-e2d9-44ab-b0c5-99abe9ea5f4a)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/9d76bd66-5a85-45c2-b6e6-326c375e7ba8)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/96dc1aab-1427-48dc-a6f9-742b2d67a493)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/5d0cb4f7-ac3a-4b91-8b61-08080959bb41)


b. Runtime vs. Matrix Sizes by fixing number of threads (Matrix Sizes - 512, 1024, 2048)
- in this we kept thread number as constant in each case and changed the matix sizes
- Block size varies between 4,16,32
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/d3d9787d-ff51-42c8-b624-9fc2cba886b7)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/fd8e65b5-e0a4-4660-8cd3-db9e34fc3471)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/6c45b871-07e1-41f2-b36c-30913f61ae2c)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/5771c7e2-19de-47cd-9e3c-d064c62235f4)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/d01eeb71-b9ee-412d-b5d4-95e4a9617a65)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/89a74312-e5df-4413-9169-79d578d02c3f)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/aca2ba6d-1ba0-48ff-aadd-a37a2c3129e0)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/8d7845f5-930e-4e4d-8621-bf09eafa466f)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/a3613692-a96c-4cf2-aa80-c115c2830f4e)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/5eeea69f-4144-43af-ba6f-cac93abcc1d4)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/61c2066b-246e-4f17-875b-6c4c11e112ad)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/09cfc050-bce0-49ec-ad61-f3775cf82bee)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/3b622030-e86c-4d62-87b9-17c8ec6bfabd)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/b92a2c08-ea88-4893-9c86-0b6d013fa2bc)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/eebf6296-9a19-4e06-987a-dd00cc702299)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/4a1cd4ed-ec65-47dc-bf3a-286c0fbfa43c)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/83bf0cf1-ca9b-498b-8b20-eed82d01a81f)
![image](https://github.com/Anandn3601/HPC-assignment/assets/91625967/3619b109-f170-49a1-8aef-e66252864136)


Threads constant as 8 
