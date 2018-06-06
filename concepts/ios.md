# <a name="ios-samples-for-the-microsoft-graph-api"></a>Примеры использования API Microsoft Graph для iOS
В этой статье приведены два примера для iOS, в которых показано, как выполнить проверку подлинности пользователя в Office 365 или в управляемых учетных записях служб (MSA), например для пользователей-потребителей Outlook. Оба примера кода отправляют электронное сообщение через службу Outlook, но один из них еще и получает фотографию из профиля пользователя и отправляет ее в тексте письма.

## <a name="ios-objective-c-connect-rest-sample"></a>Пример кода подключения на Objective-C для iOS, выполняющего REST-вызовы
Этот пример использует стандартную библиотеку HTTPS для iOS, чтобы выполнять REST-вызовы Microsoft Graph. Для аутентификации пользователя в примере используется [библиотека Microsoft Authentication Library (MSAL)](https://github.com/AzureAD/microsoft-authentication-library-for-objc/blob/dev/README.md). Библиотека MSAL позволяет приложению выполнять аутентификацию пользователя Office 365 или MSA. Вам не удастся выполнить проверку подлинности пользователя из локального экземпляра Azure Active Directory.

Пример кода позволяет отправить электронное сообщение, но при этом не извлекает фотографию пользователя, прошедшего проверку подлинности, и не внедряет ее в письмо.

- [Начало работы с Microsoft Graph в приложении для iOS на языке Objectve-C](ios_objectivec.md)

## <a name="ios-swift-connect-rest-sample"></a>Пример Swift Connect REST для iOS
Этот пример использует библиотеку Foundation HTTP и [PromiseKit](https://github.com/mxcl/PromiseKit/blob/master/README.md) для оценки конечной точки Microsoft Graph с помощью операций REST с асинхронным шаблоном **Обещания**. Для аутентификации пользователя в примере используется [библиотека Microsoft Authentication Library (MSAL)](https://github.com/AzureAD/microsoft-authentication-library-for-objc/blob/dev/README.md). Эта библиотека позволяет приложению выполнять аутентификацию пользователя Office 365 или MSA.

В этом примере показано, как получить доступ к профилю пользователя в Azure с помощью Graph. Кроме того, вы узнаете, как получить фотографию пользователя из его профиля, отправить ее в хранилище OneDrive пользователя и внедрить фотографию в текст электронного письма в Outlook.

- [Начало работы с Microsoft Graph в приложении для iOS](ios_swift.md)
