class MinStack {

private: 
    std::stack<int> stack; //we create a regular stack 
    std::stack<int> minStack; 
public:
    MinStack() {}
    
    void push(int val) {

        stack.push(val); 
        minStack.push(std::min(val, minStack.empty() ? val : minStack.top())); 
        //ensures that the top of the stack is always the smaller number 
        
    }
    
    void pop() {
        stack.pop(); 
        minStack.pop(); 
        
    }
    
    int top() {

        return stack.top(); 
        
    }
    
    int getMin() {

        return minStack.top(); 
        
    }
};
