class Solution {
public:
    bool isValid(string s) {

        if(s.length() % 2 != 0){
            return false; 
        }

        stack<char> stack1 ;
        for(int i = 0; i < s.length(); i++){

            char curr = s.at(i); 

            if(curr == '(' || curr == '[' || curr == '{'){
                stack1.push(curr); 
            }

            if(curr == ')'){
                if(!stack1.empty()){

                    if(stack1.top() == '(') {
                        stack1.pop(); 
                    } else{
                        return false; 
                    }
                } else{
                    return false; 
                }
            }
            if(curr == ']'){
                if(!stack1.empty()){

                    if(stack1.top() == '[') {
                        stack1.pop(); 
                    } else{

                        return false; 
                    }
                }else{

                    return false; 
                }
            }
            if(curr == '}'){
                if(!stack1.empty()){

                    if(stack1.top() == '{' ) {
                        stack1.pop(); 
                    } else{
                        return false; 
                    }
                } else {
                    return false; 
                }
            }

            
            
        }


        return stack1.empty(); 
  
    }
};
