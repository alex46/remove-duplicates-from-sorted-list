remove-duplicates-from-sorted-list
==================================

/**
 * Definition for singly-linked list.
 * public class ListNode {
 *     int val;
 *     ListNode next;
 *     ListNode(int x) {
 *         val = x;
 *         next = null;
 *     }
 * }
 */
public class Solution {
    public ListNode deleteDuplicates(ListNode head) {
        // Start typing your Java solution below
        // DO NOT write main() function
        if(head == null) return null;
       
        
       
        for(ListNode current = head; current != null; current = current.next){
    
           
            for(ListNode next = current.next; next != null; next = next.next){
                   if(current.val == next.val){
                       current.next = next.next;
                  
            }
               
            }
        
           
        }
       
        return head;
    }
}
