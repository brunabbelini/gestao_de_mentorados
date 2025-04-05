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
  
## 📁 Estrutura Principal
```bash
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
```

## Demonstrações da Aplicação
✅ Cadastro e Autenticação

| Cadastro de usuários | Login com erro de autenticação |
|:--:|:--:|
|![cadastro_usuarios](https://github.com/user-attachments/assets/4ad50d6f-aa82-4000-a74a-ea6392879aa2) |![login_incorreto](https://github.com/user-attachments/assets/d7d8789f-2e86-4d6d-be83-6433e38a9b40)

| Autenticação bem-sucedida e acesso aos mentorados |
|:--:|
|![mentorados_auth](https://github.com/user-attachments/assets/e1d08469-6a1f-4258-a5f1-90ae2d0e40ba)

👨‍🏫 Gerenciamento de Mentorados
| Cadastro de mentorados | Tarefa - Mentor |
|:--:|:--:|
| ![cadastro_mentorados](https://github.com/user-attachments/assets/6d68dc8e-7a33-4141-88e5-0be8f05a69cf) |![tarefa_mentor](https://github.com/user-attachments/assets/403a3db1-8c42-4b49-b7ea-1f2bad5732ad)

| Tarefa - Mentorado |
|:--:|
|![tarefa_mentorado](https://github.com/user-attachments/assets/b9be1d5b-7f16-4f4e-afae-cf52887b6f09)

📅 Reuniões
| Escolher dia | Agendar reunião |
|:--:|:--:|
| ![escolher_dia](https://github.com/user-attachments/assets/f14d1e61-739a-4ce1-88ad-74b7a838c368) |![agendar_reuniao](https://github.com/user-attachments/assets/17fd8c68-fba8-450a-8f4b-94e357a13c2e)

| Reunião marcada |
|:--:|
| ![abrir_reuniao](https://github.com/user-attachments/assets/ed633973-5240-4a04-a265-b6fe619e2eeb)

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

## 📝 Licença
Este projeto está sob a licença MIT. Veja o arquivo LICENSE para mais detalhes.


Desenvolvido com 💙 por Bruna Belini


