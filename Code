class CL
{
	static class Node
	{
		int data;
		Node next;
	};
	/* Function to insert a node
	at the beginning of a Circular
	linked list */
	static Node push(Node head_ref,int data)
	{
		Node ptr1 = new Node();
		Node dummy = head_ref;
		ptr1.data = data;
		ptr1.next = head_ref;
	// If linked list is not null
		if (head_ref != null)
		{
		while (dummy.next != head_ref)
			dummy = dummy.next;
		dummy.next = ptr1;
		}
		else
			ptr1.next = ptr1;
		head_ref = ptr1;
		return head_ref;
	}
	/*  to print nodes in   Circular linked list */
	static void listToPrintHead(Node head)
	{
		Node temporary = head;
		if (head != null)
		{
		do
		{
			System.out.print(temporary.data + " ");
			temporary = temporary.next;
		}while (temporary != head);
		} 
		if(temporary==head)
		{
			System.out.println("");
			System.out.println("no not a circular  list");
		}
 		else if(temporary !=null && temporary !=head)
 		{
 			System.out.println("");
  			System.out.println("yes its a circular list");
  		}
	}
	public static void main(String args[])
	{
		// Initialize lists as empty 
		Node head = null;
		/* Created linked list will be 11.2.56.12 */
		head = push(head, 12);
		head = push(head, 56);
		head = push(head, 2);
		head = push(head, 35);
		head = push(head, 46);
		head = push(head, 2);
		head = push(head, 11);
  		head = push(head, 56);
		head = push(head, 2);
		head = push(head, 11);
		System.out.println("Contents of Circular " +"Linked List:");
		listToPrintHead(head);
	}
}
