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
    vector<Pair> mergeSort(vector<Pair>& pairs) {
        return mergeHelper(0, pairs.size()-1, pairs);
    }

    vector<Pair> mergeHelper(int start, int end, vector<Pair>& pairs) {
        
        if(end - start + 1 <= 1){
            return pairs; 
        }
        int middle = (start + end)/2; 
        mergeHelper(start, middle, pairs);
        mergeHelper(middle+1, end, pairs);
        merge(start, middle, end, pairs); //merge

        return pairs; 




    }

    void merge(int start, int middle, int end, vector<Pair>& pairs){
        //extract the left subarray
        vector<Pair> left = {pairs.begin() + start, pairs.begin() + middle + 1};
        //extract the right subarray
        vector<Pair> right = {pairs.begin() + middle + 1, pairs.begin() + end + 1}; 
        //initialize indexes you wanna track 
        int i = 0; 
        int j = 0; 
        int k = start; 
        
        while(i < left.size() && j < right.size()){

            if(left[i].key <= right[j].key){
                pairs[k] = left[i++]; 
            } else{
                pairs[k] = right[j++]; 
            }
            k++; 
        }

        while(i < left.size()){
            pairs[k++] = left[i++]; 
        }
        while(j < right.size()){
            pairs[k++] = right[j++];
        }
        
    }


    

    
};
