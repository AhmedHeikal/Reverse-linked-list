# Reverse-linked-list

Node* Reverse(Node* head){

Node *i, *j;
		i = head;

		for (i = head; i != NULL; i = i->next) {
			for (j = i->next; j != NULL; j = j->next) {
					int temp = i->data;
					i->data = j->data;
					j->data = temp;
			}
		}
    return head;
}
