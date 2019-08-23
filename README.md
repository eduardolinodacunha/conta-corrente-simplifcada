# conta-corrente-simplifcada


public class ContaCorrenteSimplificada {
	
	String agencia;
	String nroContaCorrente;
	double saldo;
	String nomeDoCorrentista;
	boolean especial;
	PessoaFisica [] pessoas = new PessoaFisica[2];
	int qtdMax = 2;
	int qtdAtual = 0;
	double sacar(double valor) {
		this.saldo = this.saldo = valor;
		return this.saldo;
	}
	double depositar(double valor) {
		this.saldo= this.saldo = valor;
		return this.saldo;
	}
	void exibirSaldo() {
		System.out.println("Saldo" + this.saldo);
	}
	void adicionarPessoa (PessoaFisica p) {
		if(qtdAtual < qtdMax) {
			this.pessoas[qtdAtual] = p;
			qtdAtual++;
		}
	}
		void imprimirDadosCorrentista() {
			for (int i = 0; i < qtdMax ; i++) {
			if(this.pessoas[i] != null)	{
				System.out.println("====== Correntista"+(i+1) +"======");
				System.out.println("Nome  " +this.pessoas[i].nome);
				System.out.println("CPF  " + this.pessoas[i].cpf);
				System.out.println("RG  " + this.pessoas[i].rg);
				System.out.println("ORGAO EXPEDIDOR  "+ this.pessoas[i].oragaoExpedidor);
				System.out.println("DATA DE NASCIMENTO  "+ this.pessoas[i].dataNascimento);
				System.out.println("PROFISSAO  "+ this.pessoas[i].profissao);
			}
			
			
			}
		
		
	
		}}

	


