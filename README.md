# Repositorio_POO
Repositório_Teste
package Poo.Ed;

import java.util.ArrayList;

public class Main implements Delivery {
	
	private ArrayList<Cliente> clientes;
	private ArrayList<Cliente> restaurantes;
	private ArrayList<Cliente> bebidas;
	private ArrayList<Cliente> lanches;
	private ArrayList<Cliente> jantas;
	private ArrayList<Cliente> almoços;
	private ArrayList<Cliente> sobremesas;

	@Override
	public void addCliente(int idCliente, String nome, String tel_cliente, String endereço)
			throws IdClienteNullException, NomeClienteNullException, EndereçoNullException {
		Cliente c = new Cliente();
		
		if (clientes.contains(c)) {
			System.out.println("O cliente já existe");
		}else {
			clientes.add(c);
		}	
	}

	@Override
	public void RemoveCliente(int idCliente) throws IdClienteNullException {
		if (clientes.contains(idCliente)) {
			clientes.remove(idCliente);
		}else {
			System.out.println("O cliente não existe!");
		}		
	}

	@Override
	public Cliente buscarCliente(String nome, int idCliente) throws IdClienteNullException, NomeClienteNullException {
		for (int i = 0; i < clientes.size(); i++) {
			if(i == idCliente) {
				return Cliente; 
			}else {
				System.out.println("O cliente não existe!");
			}
		}
	}

	@Override
	public void addRestaurante(String endereço, int idResta, String tel, String nome)
			throws IdRestaNullException, NomeRestaNullException, EndereçoNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public void RemoveRestaurante(int idResta) throws IdRestaNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public Resta buscarRestaurante(String nome, int idResta) throws IdRestaNullException, NomeRestaNullException {
		// TODO Auto-generated method stub
		return null;
	}

	@Override
	public void addBebida(String nome, String tipo, String marca, int idBebida, float preco)
			throws IdBebidaNullException, NomeBebidaNullException, TipoBebidaNullException, MarcaBebidaNullException,
			PrecoBebidaNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public void RemoveBebida(int idBebida) throws IdBebidaNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public Bebida buscarBebida(String nome, int idBebida) throws IdBebidaNullException, NomeBebidaNullException {
		// TODO Auto-generated method stub
		return null;
	}

	@Override
	public void addAlmoço(String nome, String acompanhamento, int idAlmoço, float preco)
			throws IdAlmocoNullException, NomeAlmocoNullException, PrecoAlmocoNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public void RemoveAlmoço(int idAlmoço) throws IdAlmocoNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public Almoço buscarAlmoço(String nome, int idAlmoço) throws IdAlmocoNullException, NomeAlmocoNullException {
		// TODO Auto-generated method stub
		return null;
	}

	@Override
	public void addLanche(String nome, String tipo, int idLanche, float preco)
			throws IdLancheNullException, NomeLancheNullException, PrecoLancheNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public void RemoveLanche(int idLanche) throws IdLancheNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public Lanche buscarLanche(String nome, int idLanche) throws IdLancheNullException, NomeLancheNullException {
		// TODO Auto-generated method stub
		return null;
	}

	@Override
	public void addJanta(String nome, float preço, String acompanhamentos, int idJantar)
			throws IdJantaNullException, PreçoJantaNullException, IdJantarNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public void RemoveJanta(int idJanta) throws IdJantaNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public Jantar buscarJanta(String nome, int idJanta) throws IdJantaNullException, NomeJantaNullException {
		// TODO Auto-generated method stub
		return null;
	}

	@Override
	public void addSobremesa(String nome, float preço, String tipo, int idSobremesa)
			throws IdSobremesaNullException, PreçoSobremesaNullException, NomeSobremesaNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public void RemoveSobremesa(int idSobremesa) throws IdSobremesaNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public Sobremesa buscarSobremesa(String nome, int idSobremesa)
			throws IdSobremesaNullException, NomeSobremesaNullException {
		// TODO Auto-generated method stub
		return null;
	}

	@Override
	public void addGarçom(String nome, int idGarçom) throws IdGarçomNullException, NomeGarçomNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public void RemoveGarçom(int idGarçom) throws IdGarçomNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public Garçom buscarGarçom(String nome, int idGarçom) throws IdGarçomNullException, NomeGarçomNullException {
		// TODO Auto-generated method stub
		return null;
	}

	@Override
	public void addEntregador(int idEntregador, String contato, String nome)
			throws IdEntregadorNullException, ContatoEntregadorNullException, NomeEntregadorNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public void RemoveEntregador(int idEntregador) throws IdEntregadorNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public Entregador buscarEntregador(String nome, int idEntregador)
			throws NomeEntregadorNullException, IdEntregadorNullException {
		// TODO Auto-generated method stub
		return null;
	}

	@Override
	public void addConta(int idConta, String pedido, int valor)
			throws IdContaNullException, ValorContaNullException, PedidoContaNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public void RemoveConta(int idEntregador) throws IdContaNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public Conta buscarConta(String nome, int idEntregador) throws IdContaNullException {
		// TODO Auto-generated method stub
		return null;
	}

	@Override
	public void addPedido(String formaPag, int idPedido, int quantiPedido, String nomeLanche)
			throws FormaPagNullException, IdPedidoNullException, QuantiPedidoNullException, NomeLancheNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public void RemovePedido(int idPedido) throws IdPedidoNullException {
		// TODO Auto-generated method stub
		
	}

	@Override
	public Pedido buscarPedido(int idPedido) throws IdPedidoNullException {
		// TODO Auto-generated method stub
		return null;
	}


	
	

}
