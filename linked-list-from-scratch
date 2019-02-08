import java.util.*;

class Node{
    public int element;
    public Node next;
}

public class LinkedList{
    public static void main(String []args){
        System.out.println("Enter number of nodes-> deafault : 5");
        Scanner sc = new Scanner(System.in);
        int num_of_nodes = 5;//sc.nextInt();
        Node head = create_list(num_of_nodes);
        print_list(head);
    }

    public static  Node create_list(int num_of_nodes){
        //special case: head node
        Node head = new Node();
        head.element = 1;
        head.next=null;

        for(int i = 2; i <= num_of_nodes; i++){
            //create a new node to insert
            Node m = new Node();
            m.element = i;
            m.next = null;

            // go at the end
            Node n = head;
            for(; n.next != null; n = n.next);  // why can't we use the condition n!=null here?
            print_list(head);
            n.next = m;
             
        }

        return head;
    }

    public static void print_list(Node head){
        for(Node n = head; n!=null; n = n.next){
            System.out.print("["+n.element+"] ");
        }
        System.out.print("\n");
    }
}

    /*
    //special case: head node
    Node head = new Node();
    head.element = 1;
    head.next=null;
    //create a new node to insert
    Node m = new Node();
    m.element = 2;
    m.next = null;
    //doesn't work
    Node n = head;
    n = n.next; //changed n now, this n is separte and has no link to the original node, in this case head.
    n = m;
    */

//Resources:
//http://www.cs.bu.edu/~snyder/cs112/CourseMaterials/LinkedListNotes.Iteration.html
