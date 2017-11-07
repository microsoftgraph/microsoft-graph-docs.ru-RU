# <a name="microsoft-graph-quick-start-faq"></a>Краткое руководство по Microsoft Graph: часто задаваемые вопросы

В этой статье представлены ответы на вопросы, связанные с [краткими руководствами по Microsoft Graph](https://developer.microsoft.com/en-us/graph/quick-start).

## <a name="what-do-the-quick-starts-do"></a>В чем помогут краткие руководства?

В примерах, содержащихся в кратких руководствах, показано, как использовать всю мощь Microsoft Graph. 

Если вы используете интерфейсы REST API Office 365, то необходимо выполнять проверку подлинности для каждой вызываемой службы. Microsoft Graph упрощает эту задачу, объединяя проверку подлинности и предоставляя вам доступ ко всем API через одну точку входа. Достаточно выполнить проверку подлинности один раз, и вы получите доступ к сведениям из множества приложений и служб. 

После однократной проверки подлинности краткие руководства по Microsoft Graph получают доступ к трем службам: учетной записи Майкрософт, OneDrive и Outlook. В каждом кратком руководстве демонстрируются доступ к сведениям из профилей пользователей учетных записей Майкрософт, запись данных в OneDrive (фотографии) и создание электронного письма с помощью Outlook (со ссылкой на фотографию). 

В каждом кратком руководстве необходимо выполнить четыре действия:
- выбрать необходимую платформу; 
- получить идентификатор для приложения (также называемый идентификатором клиента);
- выполнить сборку кода из примера;
- выполнить вход в систему и отправить фотографию из профиля по электронной почте.

В итоге вы получите приложение, готовое к запуску.


## <a name="general-quick-start-sample-questions"></a>Общие вопросы, касающиеся примеров из краткого руководства
В этом разделе представлены ответы на вопросы об организации и содержимом примеров из краткого руководства.

### <a name="why-does-my-quick-start-contain-a-readme-file"></a>Почему краткое руководство содержит файл сведений?

Каждое краткое руководство позволяет зарегистрировать новое приложение и создать ZIP-файл, в котором упаковано содержимое репозитория GitHub. При этом выполняется обновление файлов в репозитории, чтобы вам не нужно было настраивать пример приложения в репозитории. Эти репозитории находятся в разделе [организации MicrosoftGraph](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=connect) на GitHub.

Вы можете просмотреть репозиторий, связанный с каждым кратким руководством, сообщить на странице этого репозитория о проблемах, а также выполнить инструкции из файла сведений (Readme), чтобы зарегистрировать собственное приложение. Чтобы открыть репозиторий, перейдите по ссылке **Just give me the sample code** (Получить пример кода) на этапе 2 любого краткого руководства.

### <a name="which-microsoft-graph-features-do-the-quick-start-samples-use"></a>Какие функции Microsoft Graph используются в примерах из кратких руководств?

Мы постоянно обновляем примеры в кратких руководствах. Чтобы получить обновления, поищите в репозитории интересующий вас пример. По мере добавления функций мы будем обновлять файл сведений, приведенный для примера. В приведенной ниже таблице перечислены текущие функции каждого примера.
 +<!-- Replace the check mark images with an actual character that can be read by a screen reader. Or you could add alt text to each instance of the image. -->

|Пример|Проверка подлинности|Получение изображения из профиля|Отправка изображения в OneDrive|Ссылка для общего доступа в электронном письме|Вложение изображения в электронное письмо|Отправка электронного письма|
|-----:|-----:|-----:|------:|------:|------:|-----:|
|[Android Connect](https://github.com/microsoftgraph/android-java-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[Angular 2 Connect](https://github.com/microsoftgraph/angular-connect-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[Angular 2 Connect REST](https://github.com/microsoftgraph/angular2-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[ASP.NET Connect](https://github.com/microsoftgraph/aspnet-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[iOS Connect — Swift](https://github.com/microsoftgraph/ios-swift-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[iOS Connect REST — Objective C](https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|[](./images/Check.PNG)|
|[Node.js Connect REST](https://github.com/microsoftgraph/nodejs-connect-rest-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)| |![](./images/Check.PNG)|
|[php Connect REST](https://github.com/microsoftgraph/php-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[php Connect](https://github.com/microsoftgraph/php-connect-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[Ruby Connect REST](https://github.com/microsoftgraph/ruby-connect-rest-sample)|![](./images/Check.PNG)| | | | |![](./images/Check.PNG)|
|[UWP Connect](https://github.com/microsoftgraph/uwp-csharp-connect-sample) |![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|
|[Xamarin Connect](https://github.com/microsoftgraph/uwp-csharp-connect-sample)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|![](./images/Check.PNG)|

## <a name="authentication-and-authorization"></a>Проверка подлинности и авторизация
В этом разделе представлены ответы на вопросы, связанные с проблемами при проверке подлинности и авторизации. 

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a>Почему в примерах из краткого руководства нет вариантов использования расширенной проверки подлинности?

Примеры из краткого руководства используются для ознакомления с функцией проверки подлинности и вызовов API Microsoft Graph. Когда вы добавляете код проверки подлинности и вызовы API Microsoft Graph в свое приложение для рабочей среды, вам необходимо знать, как спроектировать приложение для сценариев расширенной проверки подлинности, включающих вопросы обеспечения безопасности и условного доступа.

Чтобы получить дополнительные сведения о сценариях расширенной аутентификации для используемой вами библиотеки проверки подлинности, посетите страницу ее издателя.

- [OAuth2Client для Android и iOS](https://github.com/nxtbgthng/OAuth2Client)
- [Passport для Node](http://passportjs.org/)
- [Illuminate Auth для PHP](https://github.com/illuminate/auth)
- [Flask для Python 3](https://pypi.python.org/pypi/Flask-OAuth2-Provider/0.2.1)
- [OmniAuth для Ruby](https://github.com/omniauth/omniauth)
- [Microsoft Authentication Library (MSAL) для .NET](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet)
- [Microsoft Authentication Library для Android](https://github.com/AzureAD/microsoft-authentication-library-for-android)
- [Microsoft Authentication Library для JavaScript](https://github.com/AzureAD/microsoft-authentication-library-for-js)

## <a name="microsoft-graph-api"></a>API Microsoft Graph
В этом разделе представлены ответы на вопросы о написании кода приложений с использованием API Microsoft Graph.

### <a name="i-didnt-get-an-email-and-i-dont-see-any-errors-or-exceptions-why-didnt-this-work"></a>Электронное письмо не пришло, и я не вижу ошибок или исключений. Почему так случилось?

Если письма, отправленного из примера приложения, нет в папке "Входящие", проверьте папку нежелательной почты или спама. Если вы отправляете сообщение из тестового клиента, оно может быть помечено как спам.

### <a name="why-doesnt-the-email-sent-by-the-sample-have-my-profile-picture"></a>Почему в сообщении, отправленном с помощью примера кода, нет изображения из моего профиля?

Обычно это происходит, если в вашем профиле пользователя не задан аватар. Если вы вошли с помощью учетной записи Майкрософт, то даже если в вашем профиле есть аватар, он не будет отображаться в электронном письме. В настоящее время API Microsoft Graph не поддерживает аватары пользователей из учетных записей Майкрософт. Большинство примеров из кратких руководств получают ваш аватар и отправляют его в корневой каталог учетной записи OneDrive. Если вы входите с использованием учетной записи Майкрософт (live.com, hotmail.com), Microsoft Graph не может получить аватар, поэтому отображается комикс-облачко.

В примерах для Node iOS на языке Objective C аватары пользователей не вкладываются в электронные письма. 

## <a name="aspnet"></a>ASP.NET
В этом разделе представлены ответы на вопросы, связанные с написанием кода, сборкой и запуском примера из краткого руководства для ASP.NET.

### <a name="why-wont-my-aspnet-project-build"></a>Почему не выполняется сборка проекта ASP.NET?
Если в Visual Studio не удается выполнить сборку примера, использующего библиотеки .NET, для одного или нескольких ваших проектов может действовать ограничение длины пути Windows в 260 символов. Попробуйте переместить решение в корневой каталог или соседнюю с ним папку. 

## <a name="universal-windows-platform-uwp"></a>Универсальная платформа Windows (UWP)
В этом разделе представлены ответы на вопросы, связанные с написанием кода, сборкой и запуском примера из краткого руководства для UWP.

### <a name="why-wont-my-uwp-project-build"></a>Почему не выполняется сборка проекта UWP?
Если в Visual Studio не удается выполнить сборку примера, использующего библиотеки .NET, для одного или нескольких ваших проектов может действовать ограничение длины пути Windows в 260 символов. Попробуйте переместить решение в корневой каталог или соседнюю с ним папку. 

## <a name="xamarin"></a>Xamarin
В этом разделе представлены ответы на вопросы, связанные с написанием кода, сборкой и запуском примера из краткого руководства для Xamarin.

### <a name="why-wont-my-xamarin-project-build"></a>Почему не выполняется сборка проекта Xamarin?

Если в Visual Studio не удается выполнить сборку примера, использующего библиотеки .NET, для одного или нескольких ваших проектов может действовать ограничение длины пути Windows в 260 символов. Это может произойти, в частности, с решениями Xamarin, особенно для Android. Попробуйте переместить решение в корневой каталог или соседнюю с ним папку. 

## <a name="web-stack-samples"></a>Примеры веб-решений
В этом разделе представлены ответы на вопросы, связанные с написанием кода, сборкой и запуском примеров из краткого руководства, в которых используются веб-технологии.

### <a name="how-do-i-know-if-my-local-computer-supports-a-local-web-server"></a>Как узнать, поддерживается ли локальный веб-сервер на моем локальном компьютере?
В примерах из краткого руководства, в которых используются веб-технологии, есть логика, необходимая для запуска и размещения локального веб-сервера. Например, образец на языке PHP, предназначенный для среды выполнения PHP 5.4.0 и более поздних версий, включает [встроенный веб-сервер](http://php.net/manual/en/features.commandline.webserver.php), который вы можете использовать для разработки. Он не предназначен для использования в рабочей среде. 

Если вы скачали пример Node.js, прочитайте это [руководство по началу работы с Node.js](https://nodejs.org/en/docs/guides/getting-started-guide/), чтобы узнать, как запустить веб-сервер Node. 

Чтобы можно было работать с примерами для ASP.NET, Visual Studio 2015 и более поздних версий включает веб-сервер для разработки, который автоматически запускается при выполнении примера. Чтобы использовать веб-сервер, вам не нужно настраивать проект примера. 

В [файле сведений (Readme)](https://github.com/microsoftgraph/ruby-connect-rest-sample/blob/master/README.md) примера для Ruby Connect имеются инструкции, которые необходимы вам для запуска локального веб-сервера Ruby. 

### <a name="if-a-web-platform-quick-start-provides-rest-and-sdk-samples-can-i-run-them-both-at-the-same-time"></a>Если в кратком руководстве для веб-платформы есть примеры для пакетов SDK и REST, могу ли я запустить их одновременно?

Да, можно одновременно запускать оба примера. Просто убедитесь, что один из них не запущен на порту по умолчанию. Это означает, что при запуске тестового веб-сервера нужно указать номер порта по крайней мере для одной версии примера.

### <a name="why-do-some-quick-starts-include-an-app-secret-and-others-dont"></a>Почему в одних кратких руководствах есть секрет приложения, а в других — нет?

Секреты приложения требуются для серверных веб-приложений, которым нужно выполнять защищенные вызовы API Microsoft Graph. Именно поэтому краткие руководства для ASP.NET MVC, Node.js, PHP и Ruby предусматривают наличие секрета приложения.

### <a name="why-doesnt-the-angular-quick-start-give-me-an-app-secret-when-all-the-other-web-platform-quick-starts-do"></a>Почему краткое руководство для Angular, в отличие от всех остальных кратких руководств для веб-платформ, не предусматривает наличия секрета приложения?

Секрет приложения требуется только для серверных веб-приложений.

### <a name="i-get-an-error-when-i-try-to-sign-in-and-authorize-the-sample-app-what-steps-can-i-take-to-fix-this"></a>Когда я пытаюсь выполнить вход в систему и авторизовать пример приложения, возникает ошибка. Как это можно исправить? 

Сначала попробуйте запустить пример приложения в режиме InPrivate или инкогнито. Иногда настройки кэша веб-браузера могут привести к проблемам с авторизацией, особенно при входе с использованием нескольких учетных записей Майкрософт. Если это не поможет, свяжитесь с нами на сайте [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph). Пометьте свой вопрос тегом microsoft-graph и скопируйте сведения об ошибке в текст вопроса.

## <a name="didnt-find-what-you-need"></a>Не нашли то, что искали?

Если в этой статье вы не нашли ответ на интересующий вас вопрос касательно одного или нескольких кратких руководств, сообщите нам об этом на сайте [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph). Не забывайте отмечать свои вопросы тегом microsoft-graph.

Если проблема связана с примером кода, приведенном в кратком руководстве, вы можете разместить сведения о ней в репозитории примера на GitHub. Чтобы найти необходимый репозиторий, щелкните ссылку **Just give me the sample code** (Получить пример кода) в действии 2 любого краткого руководства.
