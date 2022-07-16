# ST-SPC
//compile our code
g++ -std=c++11 -O3 -fopenmp src/stspc.cpp -o test

//predata
./test txt-to-bin geofacebook/

//test decompose_tree
./test decompose_tree geofacebook/ 0

//test decompose_bt
./test decompose_bt geofacebook/ 0 20

//test decompose_core
./test decompose_core geofacebook/ 0 20

// test make queries
./test mq geofacebook/ 10000 geofacebook 0

// test queries
./test q geofacebook/ 10000 geofacebook 0
