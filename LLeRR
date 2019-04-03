void LL(no *T){/*RotaÃ§Ã£o simples Ã  esquerda*/
	no *y = T->dir;
	T->dir = y->esq;
	if(y->esq!=NULL)
		y->esq->pai = T;
	y->pai = T->pai;
	if(T->pai==NULL){
		raiz = y;
	}
	else if(T == T->pai->esq){
		T->pai->esq = y;
	}
	else{
		T->pai->dir = y;
	}
	y->esq = T;
	T->pai = y;
}

void RR(no *T){/*RotaÃ§Ã£o simples Ã  direita*/
	no *y = T->esq;
	T->esq = y->dir;

	if(y->dir!=NULL)
		y->dir->pai = T;
	y->pai = T->pai;
	if(T->pai == NULL){
		raiz = y;
	}
	else if(T == T->pai->dir){
		T->pai->dir = y;
	}
	else{
		T->pai->esq = y;
	}
	y->dir = T;
	T->pai = y;
}
