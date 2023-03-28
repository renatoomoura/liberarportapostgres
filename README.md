</p>

**Gostou do Tutorial? Faça sua Contribuição**

<img src="https://github.com/EngajamentoFlow/quepasa/blob/main/Contribui%C3%A7%C3%A3o.png" alt="Quepasa-logo" width="200" />
</p>

**PIX CNPJ**

```
45959142000119	
```
----------------------------------------------------------------------------

sudo nano /etc/postgresql/12/main/pg_hba.conf
Linha 97
host    all             all             127.0.0.1/32            scram-sha-256

Alterar para

host    all             all             0.0.0.0/0               md5

depois

sudo nano /etc/postgresql/12/main/postgresql.conf
Linha 60
#listen_addresses = 'localhost' # what IP address(es) to listen on;

Alterar para

listen_addresses = '*'		# what IP address(es) to listen on;

sudo systemctl restart postgresql

----------------------------------------------------------------------------
----------------------------------------------------------------------------

**Gostou do Tutorial? Faça sua Contribuição**

<img src="https://github.com/EngajamentoFlow/quepasa/blob/main/Contribui%C3%A7%C3%A3o.png" alt="Quepasa-logo" width="200" />
</p>


**PIX CNPJ**

```
45959142000119	
```

----------------------------------------------------------------------------
