# <a name="get-started-with-microsoft-graph-in-a-java-app"></a>Начало работы с Microsoft Graph в приложении Java

В этой статье рассказывается, как отправлять почту через Microsoft Graph из консольного Java-приложения. В качестве примера используется приложение [console-java-connect-sample](https://github.com/microsoftgraph/console-java-connect-sample). В статье приведен код, который вам следует добавить в свое Java-приложение, чтобы вы могли использовать API Microsoft Graph. Приложение получает доступ к Microsoft Graph, используя [пакет SDK Microsoft Graph для Java](https://github.com/microsoftgraph/msgraph-sdk-java).

## <a name="choose-an-authentication-library"></a>Выбор библиотеки аутентификации

В Microsoft Graph применяются стандарты OAuth 2.0 и Open ID Connect, что позволяет выбирать любые библиотеки Java среди большого количества доступных библиотек OAuth 2 с открытым кодом. Группа разработчиков Azure AD рекомендует использовать [ScribeJava](https://github.com/scribejava/scribejava). Это простая библиотека OAuth2 для Java.

В примере показано, как реализовать поток предоставления кода авторизации, который подходит для сценария авторизации клиента, пользователя и конечной точки с поддержкой OAuth 2. В Java-приложениях типа "сервер-сервер" в рабочей среде используется поток авторизации по учетным данным клиента. Библиотека **ScribeJava** обрабатывает оба этих потока авторизации. Чтобы упростить регистрацию, аутентификацию и выполнение этого примера, мы демонстрируем самый простой поток.

Чтобы ваше приложение могло вызывать Microsoft Graph, оно должно получить маркер доступа из Azure Active Directory (Azure AD). Этот маркер должен присутствовать в HTTP-заголовке аутентификации в каждом вызове Microsoft Graph. **Пакет SDK Microsoft Graph** вставляет заголовок и добавляет маркер в каждый вызов через интерфейс [IAuthenticationProvider](https://github.com/microsoftgraph/msgraph-sdk-java/blob/dev/src/main/java/com/microsoft/graph/authentication/IAuthenticationProvider.java). Библиотека **ScribeJava** выполняет аутентификацию и получает маркер доступа. Ваше приложение предоставляет маркер доступа в пакет SDK Microsoft Graph через интерфейс **IAuthenticationProvider**.

## <a name="install-and-run-the-sample"></a>Установка и запуск примера

Чтобы установить и настроить пример приложения, выполните инструкции в документе [README](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md) в репозитории **console-java-connect-sample** на веб-сайте GitHub. C помощью указанной ниже команды клонирования репозитория вы можете клонировать этот пример и пошагово изучить код в удобном для вас интерфейсе IDE Java.

```
git@github.com:microsoftgraph/console-java-connect-sample.git
```

Когда вы [регистрируете приложение Console Java Connect](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md#register-your-app), назначьте делегированные разрешения примеру. Убедитесь, что разрешения соответствуют показанным на рисунке ниже.

![Разрешения для примера Console Java Connect](../concepts/images/console-java-connnect-sample-permissions.JPG)

После того как вы зарегистрируете приложение и [настроите пример](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/README.md#configure-your-app) для **идентификатора приложения**, который вы получите при регистрации приложения, вы можете выполнить сборку примера и запустить его.

## <a name="console-java-connect-code"></a>Код Console-Java-Connect 

Прежде чем анализировать логику примера, изучите [структуру примера проекта](#sample-project-structure). После этого можете приступать к анализу логики в примере:


   
### <a name="walk-through-the-code"></a>Подробный анализ кода
Мы рассмотрим код примера бегло, а затем углубимся в подробности создания и отправки электронного письма.

#### <a name="the-user-experience"></a>Взаимодействие с пользователем

В этом разделе рассмотрена логика, которая запускает приложение и затем отображает пример выходных данных для пользователя.

Метод [PublicClient](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/PublicClient.java) **main** static создает экземпляр объекта **PublicClient** и запускает процесс входа в систему и аутентификации.  

[AuthenticationManager](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/AuthenticationManager) предоставляет отдельный экземпляр, который используется для подключения пользователя к Microsoft Graph. **AuthenticationManager** предоставляет **маркер доступа** в качестве строкового свойства. **Azure AD** возвращает маркер доступа, когда пользователь проходит аутентификацию, и предоставляет примеру разрешение на доступ к запрошенным ресурсам Microsoft Graph. 

Метод **PublicClient.startSendMail** выполняет указанные ниже действия.

- Создает экземпляр класса [GraphSendMail](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphSendMail.java). 
- Вызывает метод **GraphSendMail.getMeUser()**, чтобы возвратить профиль текущего пользователя в **Azure AD**. Благодаря этому объект консоли может персонализировать отображаемые запросы. 
- В консоли отображается следующее сообщение:

   `Hello, Laura Steele. Would you like to send an email to yourself or someone else?`

   `Enter the address to which you'd like to send a message. If you enter nothing, the message will go to your address`

- Вызывает метод **GraphSendMail.sendMail**, который принимает вводимые пользователем данные. Если указан электронный адрес, метод **sendMail** отправляет сообщение по этому адресу. В противном случае сообщение отправляется текущему пользователю. 

- Спрашивает у пользователя, что нужно сделать: отправить еще одно электронное сообщение или выйти из приложения консоли.

   `Email sent!`

   `Want to send another message? Type 'y' for yes and any other key to exit.`

#### <a name="the-send-mail-logic"></a>Логика отправки почты

Логика отправки почты выполняет указанные ниже действия.



1. **Получение аватара**:<br/> Вызывает метод **GraphServiceController.getUserProfilePicture()**, чтобы получить массив байтов, представляющих аватар вошедшего пользователя **Azure AD**.

   **Вызов API**

```java
            photoStream = mGraphServiceClient
                    .me()
                    .photo()
                    .content()
                    .buildRequest()
                    .get();

```
2. **Отправка изображения в OneDrive**:
<br/>Вызывает метод **GraphServiceController.uploadPictureToOneDrive(bytes)**, чтобы разместить аватар в корневой папке OneDrive пользователя. Система возвращает объект **DriveItem** из пакета SDK Microsoft Graph. 

   **Вызов API**
```java
            driveItem = mGraphServiceClient
                    .me()
                    .drive()
                    .root()
                    .itemWithPath("me2.png")
                    .content()
                    .buildRequest()
                    .put(picture);

```
3. **Получение ссылки для общего доступа к изображению в OneDrive**:<br/>Вызывает метод **GraphServiceController.getPermissionSharingLink**, чтобы создать ссылку для общего доступа. Система возвращает объект **Permission** из пакета SDK Microsoft Graph.

   **Вызов API**
```java
            permission = mGraphServiceClient
                    .me()
                    .drive()
                    .items(id)
                    .createLink("view", "organization")
                    .buildRequest()
                    .post();

```
4. **Заменяет содержимое тега привязки шаблона HTML** ссылкой для общего доступа (**webUrl**), полученной на предыдущем шаге. 
> **Примечание.** Тело сообщения, оправленного приложением, создается на основе шаблона HTML, хранящегося в статической строке [Constants.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Constants.java). При отправке тело сообщения содержит общедоступную гиперссылку для общего доступа к изображению, которое пример отправляет в корневую папку OneDrive пользователя. 
5. **Создание черновика сообщения**: <br/>Вызывает метод **GraphServiceController.createDraftMail**, передавая в него электронный адрес получателя, тему и обновленный шаблон HTML. В папке черновиков сообщений пользователя создается черновик сообщения.

   **Вызов API**
```java
            message = mGraphServiceClient
                    .me()
                    .messages()
                    .buildRequest()
                    .post(message);

```
6. **Прикрепление изображения к черновику сообщения**: <br/>Вызывает метод **GraphServiceController.addPictureToDraftMessage**, чтобы получить черновик сообщения, и добавляет изображение в сообщение в виде вложения объекта.

   **Вызов API**
```java
            FileAttachment fileAttachment = new FileAttachment();
            fileAttachment.oDataType = "#microsoft.graph.fileAttachment";
            fileAttachment.contentBytes = attachementBytes;
            fileAttachment.name = "me.png";
            fileAttachment.size = attachementBytes.length;
            fileAttachment.isInline = false;
            fileAttachment.id = "my profile picture";

            attachment = mGraphServiceClient
                    .me()
                    .messages(messageId)
                    .attachments()
                    .buildRequest()
                    .post(fileAttachment);

```
7. **Отправка черновика сообщения**:<br/>Вызывает метод **GraphServiceController.sendDraftMessage**, чтобы отправить обновленный черновик сообщения указанному получателю.

   **Вызов API**
```java
            mGraphServiceClient
                    .me()
                    .mailFolders("Drafts")
                    .messages(messageId)
                    .send()
                    .buildRequest()
                    .post();

```



### <a name="sample-project-structure"></a>Структура примера проекта

### <a name="connect-package"></a>Пакет connect
Этот пакет содержит логику потока аутентификации OAuth2 и конфигурацию, которую вы измените.

- [AuthenticationManager.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/AuthenticationManager.java): этот класс импортирует объекты **ScribeJava**, используемые для потока предоставления кода авторизации.
- [Constants.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Constants.java): содержит строки public static для указания значений, связанных с регистрацией приложений, и шаблон электронного письма, которое отправляет приложение.
- [Debug.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/Debug.java): общедоступный флаг уровня отладки. Задайте значение, чтобы изменить режим ведения журнала приложения.
- [DebugLogger.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/DebugLogger.java): служебная программа ведения журнала, которая записывает информацию в консоль согласно заданному уровню отладки.
- [IConnectCallback](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/connect/IConnectCallback.java): определяет метод обратного вызова, который следует использовать, если вы вызываете асинхронную перегрузку метода **ScribeJava.getAccessToken**.
- [SendMailException](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/SendMailException.java): класс, производный от класса **Exception**, который инкапсулирует информацию об исключении Microsoft Graph. Классы в пакете **GraphSendMail** могут создавать исключения этого типа.

### <a name="msgraph-package"></a>Пакет msgraph

Этот пакет содержит всю логику, которая вызывает Microsoft Graph.

- [GraphSendMail](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphSendMail.java): последовательно соединяет вызовы в объект **GraphServiceController** (пример вспомогательного класса API Microsoft Graph) для создания и отправки сообщения с вложенным изображением.
- [GraphServiceClientManager.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphServiceClientManager.java): создает экземпляр [GraphServiceClient](https://github.com/microsoftgraph/msgraph-sdk-java/blob/dev/src/main/java/com/microsoft/graph/requests/extensions/GraphServiceClient.java) в пакете SDK Microsoft Graph и добавляет маркер доступа во все исходящие вызовы API в конечной точке Microsoft Graph.

- [GraphServiceController.java](https://github.com/microsoftgraph/console-java-connect-sample/blob/master/src/main/java/com/microsoft/graphsample/msgraph/GraphServiceController.java): использует пакет SDK Microsoft Graph для всех вызовов **GraphServiceClient**. Ниже перечислены такие вызовы.

   - **createDraftMail**: создает черновик сообщения и сохраняет его в вашей папке черновиков.
   - **sendNewMessageAsync**: создает и отправляет электронное сообщение.
   - **addPictureToDraftMessage**: публикует вложенный файл в черновике сообщения по идентификатору сообщения.
   - **addAttachmentToDraftAsync**: добавляет вложение в черновик сообщения.
   - **sendDraftMessage**: отправляет сообщение из папки "Черновики".
   - **getDraftMessage**: получает сообщение из коллекции сообщений пользователя по идентификатору сообщения.
   - **getUser**: получает локального пользователя, который прошел аутентификацию в конечной точке API Microsoft Graph.
   - **getUserProfilePicture**: получает аватар вошедшего пользователя из Microsoft Graph.
   - **uploadPictureToOneDrive**: отправляет изображение в виде массива байтов в корневую папку OneDrive пользователя.
   - **getPermissionSharingLink**: отправляет в OneDrive запрос на создание общедоступной ссылки для общего доступа к изображению, хранящемуся в OneDrive.

## <a name="other-microsoft-graph-samples"></a>Другие примеры кода для Microsoft Graph

Если вы хотите увидеть какой-то конкретный пример, сообщите нам об этом, [отправив сообщение о проблеме](https://github.com/microsoftgraph/console-java-connect-sample/issues). Мы будем рады узнать, какие сценарии Microsoft Graph вы хотели бы реализовать на Java!

API Microsoft Graph — очень мощный API, с помощью которого можно взаимодействовать со всеми данными Майкрософт. Чтобы узнать больше о возможностях Microsoft Graph, ознакомьтесь с [документацией для разработчиков](https://developer.microsoft.com/ru-RU/graph/docs/concepts/overview) или опробуйте [песочницу Graph](https://developer.microsoft.com/ru-RU/graph/graph-explorer).
