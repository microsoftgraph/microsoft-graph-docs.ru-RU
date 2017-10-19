# <a name="microsoft-graph-quick-start-faq"></a>Краткое руководство по Microsoft Graph: часто задаваемые вопросы

В этой статье рассматриваются вопросы и проблемы, которые могут возникнуть при выполнении инструкций одного из [кратких руководств по Microsoft Graph](https://developer.microsoft.com/en-us/graph/quick-start).

## <a name="what-do-the-quick-starts-do"></a>В чем помогут краткие руководства?

В примерах, содержащихся в кратких руководствах, показано, как использовать всю мощь Microsoft Graph. 

В предыдущих REST API корпорации Майкрософт вам необходимо было выполнять проверку подлинности для каждой службы, которую вы хотели вызвать. Microsoft Graph упростил работу разработчиков, унифицировав проверку подлинности и объединив точки входа всех API в одну точку входа API Graph. Теперь вам достаточно выполнить проверку подлинности один раз, и вы получите доступ к информации в нескольких приложениях и службах. 

Для иллюстрации в примере из краткого руководства по Microsoft Graph показано, как получить доступ к следующим трем службам, выполнив проверку подлинности только один раз: учетная запись Майкрософт, OneDrive и Outlook. В каждом кратком руководстве показано, как извлечь сведения из профилей пользователей в учетной записи Майкрософт, выполнить запись данных (фотографии) в OneDrive, а затем создать электронное письмо с помощью Outlook (включая ссылку на фотографию). 

Чтобы получить работоспособное приложение при работе с любым кратким руководством, необходимо выполнить четыре действия:
- выбрать необходимую платформу; 
- получить идентификатор для приложения (также называемый идентификатором клиента);
- выполнить сборку кода из примера;
- выполнить вход в систему и отправить фотографию из профиля по электронной почте.

>Примечание. Эти примеры не предназначены для использования в коде рабочей среды; это всего лишь несложные иллюстрации того, что вы можете сделать на разных языках программирования и платформах. После того как вы изучите краткое руководство, мы рекомендуем вам [полностью разобраться в процессе проверки подлинности](https://docs.microsoft.com/en-us/azure/active-directory/develop/active-directory-authentication-scenarios), чтобы вы могли создавать приложения для рабочей среды.


## <a name="general-quick-start-sample-questions"></a>Общие вопросы, касающиеся примеров из краткого руководства
Вопросы об организации и содержимом набора примеров из краткого руководства.

### <a name="why-does-my-quick-start-contain-a-readme-file"></a>Почему краткое руководство содержит файл сведений (Readme)?

Каждое краткое руководство позволяет зарегистрировать новое приложение и создать ZIP-файл, в котором упаковано содержимое репозитория GitHub. При этом выполняется обновление файлов в репозитории, чтобы вам не нужно было настраивать пример приложения в репозитории. Эти репозитории находятся в разделе [организации MicrosoftGraph](https://github.com/microsoftgraph?utf8=%E2%9C%93&q=connect) на GitHub.

Вы можете просмотреть репозиторий, связанный с каждым кратким руководством, сообщить на странице этого репозитория о проблемах, а также выполнить инструкции из файла сведений (Readme), чтобы зарегистрировать собственное приложение. Щелкните ссылку **Just give me the sample code** (Получить пример кода) в действии 2 краткого руководства, чтобы перейти к связанному репозиторию.

### <a name="which-microsoft-api-features-do-the-quick-start-samples-show"></a>Какие функции API Майкрософт показаны в примерах в кратких руководствах?

Набор примеров постоянно совершенствуется. Изучите репозиторий интересующего вас примера. По мере добавления функций в избранный вами пример мы объявляем об этом в файле сведений (Readme) примера. В таблице ниже показаны текущие функции, имеющиеся в примерах.

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
Вопросы, связанные с проблемами при проверке подлинности и авторизации. 

### <a name="why-dont-any-of-the-quick-start-samples-show-advanced-authentication-use-cases"></a>Почему в примерах из краткого руководства нет вариантов использования расширенной проверки подлинности?

Примеры из краткого руководства используются для ознакомления с функцией проверки подлинности и вызовов API Microsoft Graph. Когда вы добавляете функции проверки подлинности и вызовов API Graph в свое приложение для рабочей среды, вам необходимо знать, как спроектировать код для сценариев расширенной проверки подлинности, включающих вопросы обеспечения безопасности и условного доступа.

Чтобы получить дополнительные сведения о сценариях расширенной проверки подлинности для используемой вами библиотеки проверки подлинности, посетите веб-страницы издателя библиотеки проверки подлинности.

- [OAuth2Client для Android и iOS](https://github.com/nxtbgthng/OAuth2Client)
- [Passport для Node](http://passportjs.org/)
- [Illuminate Auth для PHP](https://github.com/illuminate/auth)
- [Flask для Python 3](https://pypi.python.org/pypi/Flask-OAuth2-Provider/0.2.1)
- [OmniAuth для Ruby](https://github.com/omniauth/omniauth)
- [Microsoft Authentication Library (MSAL) для .NET](https://github.com/AzureAD/microsoft-authentication-library-for-dotnet)
- [Microsoft Authentication Library для Android](https://github.com/AzureAD/microsoft-authentication-library-for-android)
- [Microsoft Authentication Library для JavaScript](https://github.com/AzureAD/microsoft-authentication-library-for-js)

## <a name="microsoft-graph-api"></a>API Microsoft Graph
Вопросы о создании кода для API Microsoft Graph

### <a name="i-didnt-get-an-email-and-i-see-no-errors-or-exceptions-why-didnt-this-work"></a>Электронное письмо не пришло, и я не вижу ошибок или исключений. Почему так случилось?

Если письма, отправленного из примера приложения, нет в папке "Входящие", проверьте папку нежелательной почты или спама. Если вы отправляете сообщение из тестового клиента, оно может быть помечено как спам.

### <a name="why-doesnt-the-email-sent-by-the-sample-have-my-profile-picture"></a>Почему в сообщении, отправленном с помощью примера кода, нет изображения из моего профиля?

- Обычно это происходит, если в вашем профиле не задано изображение профиля пользователя. Если вы выполнили вход в систему с помощью учетной записи службы Майкрософт (MSA), то даже если в вашем профиле есть изображение, оно не будет отображено в электронном письме. На данный момент API Microsoft Graph не поддерживает изображения из профилей пользователей из учетных записей MSA. <br/>Большинство примеров приложений, которые скачиваются при выполнении инструкций краткого руководства, получают изображение вашего профиля и отправляют его в корневой каталог учетной записи OneDrive. Если вы входите с использованием учетной записи Майкрософт (live.com, hotmail.com), Microsoft Graph не может получить изображение профиля, поэтому отображается комикс-облачко.

- В примере для Node и в примерах для iOS на языке Objective C не выполняется вложение изображений из профилей пользователей в электронные письма. 

## <a name="asp-net"></a>ASP .NET
Вопросы, связанные с созданием кода, сборкой или выполнением примеров из краткого руководства для ASP.NET.

## <a name="universal-windows-platform-uwp"></a>Универсальная платформа Windows (UWP)
Вопросы, связанные с созданием кода, сборкой или выполнением примеров из краткого руководства для UWP.

## <a name="xamarin"></a>Xamarin
Вопросы, связанные с созданием кода, сборкой или выполнением примеров из краткого руководства для Xamarin.

### <a name="why-wont-my--aspnet-uwp-or-xamarin-project-build"></a>Почему не удается выполнить сборку проекта для ASP.NET, UWP или Xamarin?

Если в Visual Studio не удается выполнить сборку примера, использующего библиотеки .NET, для одного или нескольких ваших проектов может действовать ограничение длины пути Windows в 260 символов. Это может произойти, в частности, с решениями Xamarin, особенно для Android. Попробуйте переместить решение в корневой каталог или соседнюю с ним папку. 

## <a name="web-stack-samples"></a>Примеры веб-решений
Вопросы, связанные с созданием кода, сборкой или выполнением примеров из краткого руководства, в которых используются веб-технологии.

### <a name="how-do-i-know-if-my-local-computer-supports-a-local-web-server"></a>Как узнать, поддерживает ли мой локальный компьютер локальный веб-сервер?
В примерах из краткого руководства, в которых используется веб-технология, содержится логика, необходимая для запуска и размещения локального веб-сервера. Например, пример для PHP, предназначенный для среды выполнения PHP 5.4.0 и более поздней версии, включает [встроенный веб-сервер](http://php.net/manual/en/features.commandline.webserver.php), который вы можете использовать для разработки. Он не предназначен для использования в рабочей среде. 

Если вы скачали пример Node.js, прочитайте это [руководство по началу работы с Node.js](https://nodejs.org/en/docs/guides/getting-started-guide/), чтобы узнать, как запустить веб-сервер Node. 

Для работы с примерами для ASP.NET в Visual Studio 2015 и более поздних версий имеется веб-сервер для разработки, который автоматически запускается, когда вы запускаете пример. Чтобы использовать веб-сервер, вам не нужно настраивать проект примера. 

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

Если в этой статье вы не нашли ответ на интересующий вас вопрос касательно одного или нескольких кратких руководств, сообщите нам об этом на сайте [Stack Overflow](https://stackoverflow.com/questions/tagged/microsoft-graph). 

Если проблема связана с примером кода, приведенном в кратком руководстве, вы можете разместить сведения о ней в репозитории примера на GitHub. Чтобы найти необходимый репозиторий, щелкните ссылку **Just give me the sample code** (Получить пример кода) в действии 2 любого краткого руководства.
