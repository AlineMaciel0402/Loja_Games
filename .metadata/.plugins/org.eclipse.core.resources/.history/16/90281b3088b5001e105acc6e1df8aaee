package com.generation.lojagames.model;

import java.time.LocalDateTime;

import org.hibernate.annotations.UpdateTimestamp;

import com.fasterxml.jackson.annotation.JsonIgnoreProperties;

import jakarta.persistence.Entity;
import jakarta.persistence.GeneratedValue;
import jakarta.persistence.GenerationType;
import jakarta.persistence.Id;
import jakarta.persistence.ManyToOne;
import jakarta.persistence.Table;
import jakarta.validation.constraints.NotBlank;
import jakarta.validation.constraints.Size;

@Entity
@Table(name = "tb_produtos" )


public class Produto {
	
	@Id
	@GeneratedValue(strategy=GenerationType.IDENTITY)
	private Long id; 
	
	@Size(min=5, max= 100, message = "O nome deve ter no mínimo 5 caracteres e no máximo 100")
	@NotBlank( message = "Atributo título é obrigatório")
	private String nome;
	
	private Double preco;
	
	private Integer AnoLancamento;
	
	@Size(min=5, max= 100, message = "A desenvolvedora deve ter no mínimo 5 caracteres e no máximo 100")
	@NotBlank( message = "Atributo desenvolvedora é obrigatório")
	private String desenvolvedora;
	
	@UpdateTimestamp 
	private LocalDateTime data;
	
	@ManyToOne
	@JsonIgnoreProperties("produto")
	private Categoria categoria;

	public Long getId() {
		return id;
	}

	public void setId(Long id) {
		this.id = id;
	}

	public String getNome() {
		return nome;
	}

	public void setNome(String nome) {
		this.nome = nome;
	}

	public Double getPreco() {
		return preco;
	}

	public void setPreco(Double preco) {
		this.preco = preco;
	}

	public Integer getAnoLancamento() {
		return AnoLancamento;
	}

	public void setAnoLancamento(Integer anoLancamento) {
		AnoLancamento = anoLancamento;
	}

	public String getDesenvolvedora() {
		return desenvolvedora;
	}

	public void setDesenvolvedora(String desenvolvedora) {
		this.desenvolvedora = desenvolvedora;
	}

	public LocalDateTime getData() {
		return data;
	}

	public void setData(LocalDateTime data) {
		this.data = data;
	}

	public Categoria getCategoria() {
		return categoria;
	}

	public void setCategoria(Categoria categoria) {
		this.categoria = categoria;
	}
	
	


	}
	
	

