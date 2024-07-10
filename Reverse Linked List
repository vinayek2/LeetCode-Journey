/**
 * Definition for singly-linked list.
 * struct ListNode {
 *     int val;
 *     ListNode *next;
 *     ListNode() : val(0), next(nullptr) {}
 *     ListNode(int x) : val(x), next(nullptr) {}
 *     ListNode(int x, ListNode *next) : val(x), next(next) {}
 * };
 */

class Solution {
public:
    ListNode* reverseList(ListNode* head) {

        ListNode* curr = head; 
        ListNode* prev = nullptr; 
        ListNode* next = nullptr; 
        
        while(curr){
            next = curr -> next; 
            curr -> next = prev; 
            prev = curr; 
            curr = next; 

            
        }

        head = prev; 

        return head; 


        /*
        curr = head 
        prev = nullptr 
        next = nullptr 
         1 -> 2 -> 3 -> nullptr
        next = curr -> next //iterate through list 
        curr -> next = prev
        prev = curr
        curr = next 
        nullptr <- 1 <- 2 <- 3 


        1 curr 
        null prev
        null next


        2 next 
        curr -> next = nullptr
        prev = 1 
        curr = 2 

        2 curr 
        1 prev
        2 next



        next = 3
        curr->next = 1 
        prev = 2 
        curr = 3 

        3 curr 
        2 prev 
        3 next 

        next = nullptr 

        curr -> next = 2
        
        prev = 3
        
        curr = nullptr 


        
        */
























        // ListNode* curr = head; 
        // ListNode* prev =nullptr; 
        
        // ListNode* next = nullptr; 

        // while(curr != nullptr){
        //     //next 

        //     next = curr -> next;

        //     curr -> next = prev; 
            
        //     prev = curr ; 

        //     curr = next ; 
        // }

        // return prev; 
        
    }
};
