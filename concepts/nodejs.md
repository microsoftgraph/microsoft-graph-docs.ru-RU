# <a name="get-started-with-microsoft-graph-in-a-nodejs-app"></a>Начало работы с Microsoft Graph в приложении Node.js

В этой статье описываются задачи, которые необходимо выполнить, чтобы получить маркер доступа из конечной точки Azure AD версии 2.0 и вызвать Microsoft Graph. В ней рассматривается создание [приложения Microsoft Connect для Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample) и объясняются основные понятия, которые необходимо реализовать для использования Microsoft Graph. В этой статье рассказывается, как получить доступ к API Microsoft Graph с помощью необработанных вызовов REST.

На приведенном ниже рисунке показано создаваемое приложение. 

![Веб-приложение после входа с кнопкой "Отправить сообщение"](./images/web-screenshot.png)


**Не хотите создавать приложение?** С помощью [краткого руководства по Microsoft Graph](https://graph.microsoft.io/en-us/getting-started) вы сможете быстро приступить к работе.

Скачать вариант этого примера, использующий конечную точку Azure AD, можно на странице [приложения Microsoft Graph Connect для Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample/releases/tag/last_v1_auth).


## <a name="prerequisites"></a>Необходимые условия

Чтобы приступить к работе, вам понадобится следующее: 

- [Учетная запись Майкрософт](https://www.outlook.com/) либо [рабочая или учебная учетная запись](http://dev.office.com/devprogram).
- [Node.js с npm](https://nodejs.org/en/download/). 
- [Приложение Microsoft Connect для Node.js](https://github.com/microsoftgraph/nodejs-connect-rest-sample). Вы будете использовать папку **starter-project** в примерах файлов для этого пошагового руководства.

## <a name="register-the-application"></a>Регистрация приложения
Зарегистрируйте приложение на портале регистрации приложений (Майкрософт). При этом будут созданы идентификатор и пароль приложения, которые понадобятся при его настройке в Visual Studio.

1. Войдите на [портал регистрации приложений Майкрософт](https://apps.dev.microsoft.com/) с помощью личной, рабочей или учебной учетной записи.

2. Нажмите кнопку **Добавить приложение**.

3. Введите имя приложения и нажмите кнопку **Создать приложение**. 
    
    Откроется страница регистрации со свойствами приложения.

4. Скопируйте идентификатор приложения. Это уникальный идентификатор приложения. 

5. В разделе **Секреты приложения** нажмите кнопку **Создать новый пароль**. Скопируйте пароль из диалогового окна **Новый пароль создан**.

    Идентификатор и пароль (секрет) приложения используются для его настройки. 

6. В разделе **Платформы** выберите **Добавление платформы** > **Веб**.

7. Введите URI перенаправления *http://localhost:3000/token*. 

8. Нажмите **Сохранить**.


## <a name="configure-the-project"></a>Настройка проекта
1. Откройте папку **starter-project** с файлами примера.

1. Откройте командную строку и выполните приведенную ниже команду в корневом каталоге начального проекта. При этом устанавливаются зависимости проекта.

        npm install

1. В файлах начального проекта откройте utils\config.js.


1. В поле **credentials** замените строки **ENTER\_YOUR\_CLIENT\_ID** и **ENTER\_YOUR\_SECRET** скопированными только что значениями.

  
## <a name="authenticate-the-user-and-get-an-access-token"></a>Проверка подлинности пользователя и получение маркера доступа
На этом этапе вы добавите код для входа и управления маркером. Но для начала подробнее рассмотрим поток проверки подлинности.

В этом приложении используется поток предоставления кода авторизации с делегированным удостоверением пользователя. В веб-приложении для этого потока требуются идентификатор, секрет и URI перенаправления зарегистрированного приложения. 

Поток проверки подлинности можно разделить на следующие основные этапы:

1. Перенаправление пользователя для проверки подлинности и согласия
2. Получение кода авторизации
3. Обмен кода авторизации на маркер доступа
4. Использование маркера обновления для получения нового маркера доступа по истечении срока действия текущего

В приложении используется ПО промежуточного слоя [oauth](https://www.npmjs.com/package/oauth) для проверки подлинности и получения маркеров. С помощью ПО промежуточного слоя [cookie-parser](https://www.npmjs.com/package/cookie-parser) приложение кэширует сведения о маркере в файлах cookie. Код, используемый для хранения сведений о маркере и доступа к ним, находится в контроллере index.js.
    
   >**Важно!** Простые процедуры проверки подлинности и обработки маркеров в этом проекте представлены исключительно в качестве примера. В рабочем приложении следует реализовать более надежную процедуру проверки подлинности, включающую утверждение и безопасную обработку маркеров.

Теперь вы готовы добавить код для вызова Microsoft Graph. 

## <a name="call-microsoft-graph"></a>Вызов Microsoft Graph
Приложение вызывает Microsoft Graph, чтобы получить данные пользователя и отправить электронное сообщение от его имени. Такие вызовы отправляются из контроллера index.js в ответ на события пользовательского интерфейса.

1. Откройте utils\graphHelper.js.

1. Замените функцию **getUserData** приведенным ниже кодом. Этот код настраивает и отправляет запрос GET конечной точке */me*, а затем обрабатывает ответ.

        function getUserData(accessToken, callback) {
          request
           .get('https://graph.microsoft.com/v1.0/me')
           .set('Authorization', 'Bearer ' + accessToken)
           .end((err, res) => {
             callback(err, res);
           });
        }

1. Замените функцию **getProfilePhoto** приведенным ниже кодом. Этот код настраивает и отправляет запрос GET конечной точке */me/photo/$value*, а затем обрабатывает ответ. Обратите внимание, что фотографии профиля в настоящее время недоступны для учетных записей MSA.
    
        function getProfilePhoto(accessToken, callback) {
          // Get the profile photo of the current user (from the user's mailbox on Exchange Online).
          // This operation in version 1.0 supports only work or school mailboxes, not personal mailboxes.
          request
           .get('https://graph.microsoft.com/v1.0/me/photo/$value')
           .set('Authorization', 'Bearer ' + accessToken)
           .end((err, res) => {
             // Returns 200 OK and the photo in the body. If no photo exists, returns 404 Not Found.
             callback(err, res.body);
           });
        }

1. Замените функцию **uploadFile** следующим кодом. Он настраивает и отправляет запрос PUT в конечную точку */me/drive/root/children/mypic.jpg/content*. Если файл существует, этот запрос обновляет содержимое. В противном случае он создает файл и добавляет фотографию профиля. 

        function uploadFile(accessToken, file, callback) {
          // This operation only supports files up to 4MB in size.
          // To upload larger files, see `https://developer.microsoft.com/graph/docs/api-reference/v1.0/api/item_createUploadSession`.
          request
           .put('https://graph.microsoft.com/v1.0/me/drive/root/children/mypic.jpg/content')
           .send(file)
           .set('Authorization', 'Bearer ' + accessToken)
           .set('Content-Type', 'image/jpg')
           .end((err, res) => {
             // Returns 200 OK and the file metadata in the body.
             callback(err, res.body);
           });
        }

1. Замените функцию **getSharingLink** приведенным ниже кодом. Он настраивает и отправляет запрос GET в конечную точку */me/drive/items/{идентификатор файла}/createLink* и обрабатывает результат (ссылку для общего доступа к файлу, которая будет включена в сообщение).

        function getSharingLink(accessToken, id, callback) {
          request
           .post('https://graph.microsoft.com/v1.0/me/drive/items/' + id + '/createLink')
           .send({ type: 'view' })
           .set('Authorization', 'Bearer ' + accessToken)
           .set('Content-Type', 'application/json')
           .end((err, res) => {
             // Returns 200 OK and the permission with the link in the body.
             callback(err, res.body.link);
           });
        }

1. Замените функцию **postSendMail** приведенным ниже кодом. Этот код настраивает и отправляет запрос POST конечной точке */me/sendMail*, а затем обрабатывает отклик.

        function postSendMail(accessToken, message, callback) {
          request
           .post('https://graph.microsoft.com/v1.0/me/sendMail')
           .send(message)
           .set('Authorization', 'Bearer ' + accessToken)
           .set('Content-Type', 'application/json')
           .set('Content-Length', message.length)
           .end((err, res) => {
             // Returns 202 if successful.
             // Note: If you receive a 500 - Internal Server Error
             // while using a Microsoft account (outlook.com, hotmail.com or live.com),
             // it's possible that your account has not been migrated to support this flow.
             // Check the inner error object for code 'ErrorInternalServerTransientError'.
             // You can try using a newly created Microsoft account or contact support.
             callback(err, res);
           });
        }

1. Откройте utils\emailer.js.

1. Замените функцию **wrapEmail** приведенным ниже кодом. Этот код создает полезные данные, представляющие отправляемое сообщение.

        function wrapEmail(content, recipient, file) {
          const attachments = [{
            '@odata.type': '#microsoft.graph.fileAttachment',
            ContentBytes: file,
            Name: 'mypic.jpg'
          }];
          const emailAsPayload = {
            Message: {
              Subject: 'Welcome to Microsoft Graph development with Node.js and the Microsoft Graph Connect sample',
              Body: {
                ContentType: 'HTML',
                Content: content
              },
              ToRecipients: [
                {
                  EmailAddress: {
                    Address: recipient
                  }
                }
              ]
            },
            SaveToSentItems: true,
            Attachments: attachments
          };
          return emailAsPayload;
        }

## <a name="run-the-app"></a>Запуск приложения

1. Откройте командную строку и выполните приведенную ниже команду в корневом каталоге начального проекта.


        npm start

1. Введите в браузере адрес *http://localhost:3000* и нажмите кнопку **Подключиться к Office 365**.

1. Выполните вход и предоставьте запрашиваемые разрешения. 

1. При необходимости измените электронный адрес получателя и нажмите кнопку **Отправить сообщение**. Под кнопкой появится сообщение, что отправка выполнена успешно. 

## <a name="next-steps"></a>Дальнейшие действия
- Попробуйте REST API, используя [песочницу Graph](https://graph.microsoft.io/graph-explorer).
- Просмотрите другие [примеры Node.js](https://github.com/search?utf8=%E2%9C%93&q=node+sample+user%3Amicrosoftgraph&type=Repositories&ref=searchresults) на сайте GitHub.


## <a name="see-also"></a>См. также
- Попробуйте примеры вызовов REST в нашем [обозревателе API](https://graph.microsoft.io/graph-explorer)
- [Получение маркеров доступа для вызова Microsoft Graph](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_overview)
- [Получение доступа от имени пользователя](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_user)
- [Получение доступа без пользователя](https://developer.microsoft.com/en-us/graph/docs/concepts/auth_v2_service)
