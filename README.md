# OMQL-Miner
Installing:
 <code>git clone https://github.com/OMQL/OMQL-Miner.git</code><br>
 <code>  cd OMQL-Miner</code><br>
 <code> g++ main.cpp -o omql_miner -lcurl</code>
 
 Usage:
  <code>./omql_miner Username</code>
 
 
 Known issues:  
 nvcc fatal : Unsupported gpu architecture 'compute_20' <br>
 Open <code>ccminer/makefile.am</code> and delete <code>gencode arch=compute_20,code=sm_20</code>. There should be three lines with this code. Then compile ccminer maually using <code>./autogen.sh</code>, <code>./configure</code> and <code>./build.sh</code>
