// Definition for a Pair
// class Pair {
// public:
//     int key;
//     string value;
//
//     Pair(int key, string value) : key(key), value(value) {}
// };
class Solution {
public:
    vector<vector<Pair>> insertionSort(vector<Pair>& pairs) {

        vector<vector<Pair>> vectorPairs; 
        for(int i = 0; i < pairs.size(); i++){
            int j = i - 1; 
            while(j >= 0 && pairs[j+1].key < pairs[j].key){

                Pair temp = pairs[j+1]; 
                pairs[j+1] = pairs[j];
                pairs[j] = temp; 
                j -= 1; 
            }

            vectorPairs.push_back(pairs); 

            
        }

        return vectorPairs; 

        //// 5 4

    
    }
};

/*

for(int i = 0; i < arr.size(); i++){
    j = i - 1; 
    while(j >= 0 && arr[j+1] < arr[j]){
        int temp = arr[j+1]; 
        arr[j+1] = arr[j]; 
        arr[j] = temp; 
        j -= 1; 
    }
}


*/
