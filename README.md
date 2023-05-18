</p>

**Gostou do Tutorial? Faça sua Contribuição**

<img src="https://github.com/EngajamentoFlow/quepasa/blob/main/Contribui%C3%A7%C3%A3o.png" alt="Quepasa-logo" width="200" />
</p>

**PIX CNPJ**

```
45959142000119	
```
----------------------------------------------------------------------------

</p>
sudo nano /etc/postgresql/12/main/pg_hba.conf
</p>
Linha 97
</p>
host    all             all             127.0.0.1/32            scram-sha-256
</p>
Alterar para
</p>
host    all             all             0.0.0.0/0               md5
</p>
depois
</p>
sudo nano /etc/postgresql/12/main/postgresql.conf
</p>
Linha 60
</p>
#listen_addresses = 'localhost' # what IP address(es) to listen on;

Alterar para
</p>
listen_addresses = '*'		# what IP address(es) to listen on;
</p>
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
