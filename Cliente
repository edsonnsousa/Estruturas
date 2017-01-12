#include <stdio.h>
#include <iostream>
#include <string.h>
using namespace std;
class Cliente{
	private:
		string nome;
		string numCart;
		double saldoCart;
		double limiteCart;
	public:
		Cliente(string n,string num,double saldo,double limite){
			this->nome=n;
			this->numCart=num;
			this->saldoCart=saldo;
			this->limiteCart=limite;
		}
		string getNome(){
			return nome;
		}
		string getNumero(){
			return numCart;
		}
		double getSaldo(){
			return saldoCart;
		}
		double getlimite(){
			return limiteCart;
		}
		};
class Lista{
	private:
		Cliente *l[5];
		int qtd;
	
	public :
		Lista(){
			qtd=0;
				
		}
	void inserir(string nome,string num,double saldo,double limite){
		if (qtd<5){
			Cliente *novo = new Cliente(nome,num,saldo,limite);
			l[qtd]=novo;
			qtd++;
		}
		else{
		
		cout<<"Lista Lotada!";
		}
		}
		
		
		Cliente *maiorLimite(){
		Cliente *maior=l[0];
		for(int i=0;i<qtd;i++){
			if (l[i]->getlimite() > maior->getlimite() ){
				maior=l[i];
			}
		}
		
		return maior;
				
		
		
		
	void mostrar(){
		for(int i=0;i<qtd;i++){
			cout<<"---->Informacoes<----\n";
			cout<<"Nome: "<<l[i]->getNome()<<"\n";			
			cout<<"Numero: "<<l[i]->getNumero()<<"\n";
			cout<<"Saldo: "<<l[i]->getSaldo()<<"\n";
			cout<<"Limite: "<<l[i]->getlimite()<<"\n";
			
		}
	}
	void maior(){
		Cliente *m=l->maiorLimite();
		cout<<"Maior Saldo: "<< m->getlimite();
	}
	
		
		

	
}


};
	

main(){
	Lista*lista1=new Lista();
	lista1->inserir("Edson","1",20.2,100);
	lista1->inserir("Hidelbrando","11",120.34,1000);
	lista1->mostrar();
	lista1->maior();
}


