# Promptopia

Promptopia оснащен множеством функций, направленных на улучшение взаимодействия пользователя и оптимизацию процесса работы с промптами. Эти функции делают платформу мощным инструментом для создания, обмена и поиска вдохновляющих идей.

## Превью 

https://ai-prompts-alex008145s-projects.vercel.app/



## Особенности 


- Аутентификация с Google: Пользователи могут войти в Promptopia, используя свои учетные записи Google, обеспечивая безопасный и простой процесс входа в систему.
Создание, Редактирование и Удаление Постов: После входа пользователи могут создавать новые промпты, редактировать существующие или удалять те, которые они больше не хотят сохранять. Это дает им полный контроль над своей коллекцией промптов.
- Профили Пользователей: У каждого пользователя есть своя страница профиля, на которой можно демонстрировать созданные ими промпты. Другие пользователи могут посещать эти профили, чтобы просматривать и вдохновляться промптами, которыми поделился этот пользователь.
- Функция Поиска: Главная страница Promptopia позволяет пользователям искать промпты по ключевым словам, тегам или именам пользователей. Эта функция облегчает пользователям нахождение промптов, связанных с конкретными темами или интересами.
- Копирование Текста Промпта: Удобная кнопка позволяет пользователям копировать текст промпта одним нажатием. Это делает удобным вставку промпта в AI-инструмент или любую другую платформу для письма.
- Проект создан с помощью Next.js
- Cтилизован с помощью Tailwind
- Использует базу данных MongoDB для хранения запросов и данных авторов.


- Данный проект создан по видеокурсу автора [JavaScript Mastery](https://www.youtube.com/@javascriptmastery) https://youtu.be/wm5gMKuwSYk?si=acl9fNwzIjRISRYS


## Prerequisites

Before running the application, you need to have the following installed on your system:

- Next.js (version 13)
- React
- Node.js (version 14 or later)
- MongoDB (version 4.0 or later)

Promptopia is deployed on Vercel, a cloud platform for static sites and serverless functions.

## Installation

1. Clone the repository to your local machine using the following command:

```bash
   git clone https://github.com/Alex008145/ai_prompts.git
```

2. Install the necessary dependencies by navigating to the project directory and running:

```bash
npm install
```

3. Create a `.env` file in the root directory of the project and add the following environment variables:

```bash

GOOGLE_ID=
GOOGLE_CLIENT_SECRET=
MONGODB_URI=
NEXTAUTH_URL=
NEXTAUTH_URL_INTERNAL=
NEXTAUTH_SECRET=

```

4. Run the app:

```bash
   npm run dev
```

## API Endpoints

The following API endpoints are available:

- POST /api/prompt/new :

Create new prompt.

- GET /api/users/${session.user.id}/posts:

Get all posts for the user.

- GET /api/prompt/tag/${params.tag}/:

Get all posts ralated to the tag you cllicked on.

- GET /api/users/${username}/posts:

Get all posts of the user on the user`s profile.

- GET /api/prompt/${promptId}

Get prompt.

- PATCH /api/prompt/${promptId}

Update prompt.

- GET /api/prompt

Get all prompts.

- DELETE /api/prompt/${post.\_id.toString()}

Delete prompt.

## Error Handling

The API endpoints return error responses with code and message.
