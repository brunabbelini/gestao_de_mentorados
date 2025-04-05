# Sistema de Gerenciamento de Mentorias 🎓✨

Este é um sistema web desenvolvido com Django, TailwindCSS e HTMX, com foco na organização de mentorias, gerenciamento de tarefas e acompanhamento de reuniões com mentorados.
A plataforma permite que mentores acompanhem o progresso de seus mentorados, atribuam tarefas, visualizem vídeos de reuniões e organizem tudo de forma prática e intuitiva.

## 🚀 Tecnologias Utilizadas

- [Django](https://www.djangoproject.com/) — Back-end do projeto
- [Tailwind CSS](https://tailwindcss.com/) — Estilização moderna e responsiva
- [HTMX](https://htmx.org/) — Requisições assíncronas sem precisar de JavaScript complexo
- [SQLite](https://www.sqlite.org/index.html) — Banco de dados padrão
- HTML5, CSS3, Python 3.12+

## 📚 Funcionalidades

- Cadastro de **mentorados** com upload de fotos
- Registro de **tarefas** para cada mentorado
- Marcação de tarefas como realizadas (via HTMX e checkbox)
- Upload e exibição de **vídeos** de reuniões
- Interface limpa e responsiva com Tailwind

## 📸 Tela do Projeto

<p align="center">
  <img src="screenshot.png" alt="Tela do sistema" width="600">
</p>

## 🔧 Como rodar o projeto localmente

1. Clone o repositório:

```bash
git clone https://github.com/brunabbelini/gestao_de_mentorados/
cd seu-repositorio
```
2. Crie e ative um ambiente virtual:
```bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate      # Windows
```
3. Instale as dependências:
```bash
pip install -r requirements.txt
```
4. Aplique as migrações e inicie o servidor:
```bash
python manage.py makemigrations
python manage.py migrate
```
5. Crie um superusuário (opcional, para acessar o admin)
```bash
python manage.py createsuperuser
```
6. Rode o servidor
```bash
python manage.py runserver
``` 
Acesse no navegador: http://127.0.0.1:8000
   
## 📁 Estrutura Principal
gestao_de_mentorados/ 

├── core/                                                                

│   ├── __init__.py                                                      

│   ├── settings.py                                                      

│   ├── urls.py                                                          

│   └── wsgi.py

├── mentorados/

│   ├── migrations/

│   ├── templates/ 

|   ├── apps.py

|   ├── admin.py

|   ├── auth.py

│   ├── models.py

│   ├── views.py

│   └── urls.py

├── media/

├── templates/

│   ├── static/

│   ├── base.html

├── usuarios/

│   ├── templates/

│   ├── views.py

│   └── urls.py

├── venv/

├── db.sqlite3

├── manage.py

└── requirements.txt


## 📝 Licença
Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.


Desenvolvido com 💙 por Bruna Belini


