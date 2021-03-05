---
title: Вызов служб Microsoft 365 в Visual Studio 2017 с помощью API Microsoft Graph
description: Вы можете сделать так, чтобы приложение вызывало API Microsoft Graph, с помощью Подключенных служб Visual Studio. В этой статье описано, как получить фотографию профиля вошедшего пользователя, передать ее в OneDrive и отправить письмо со ссылкой для общего доступа к фотографии.
localization_priority: Priority
ms.prod: reports
author: sarahwxy
ms.openlocfilehash: 7b93a0245c34b67d3975d0b568df5defd292b72c
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472855"
---
# <a name="call-microsoft-365-services-in-visual-studio-2017-with-the-microsoft-graph-api"></a>Вызов служб Microsoft 365 в Visual Studio 2017 с помощью API Microsoft Graph

Вы можете сделать так, чтобы приложение вызывало API Microsoft Graph, с помощью Подключенных служб Visual Studio. В этой статье описано, как получить фотографию профиля вошедшего пользователя, передать ее в OneDrive и отправить письмо со ссылкой для общего доступа к фотографии.

## <a name="get-set-up"></a>Настройка

Чтобы использовать Подключенные службы Office 365 с помощью Microsoft Graph, сделайте следующее:

- Скачайте [предварительную версию Visual Studio 2017](https://www.visualstudio.com/vs/preview/). Предварительную версию Visual Studio 2017 можно использовать параллельно с более ранней версией Visual Studio.

- Оформите подписку на Microsoft 365. Чтобы получить бесплатную пробную версию, зарегистрируйтесь в [Программе для разработчиков Microsoft 365](https://developer.microsoft.com/microsoft-365/dev-program).

## <a name="get-the-starter-project"></a>Получение исходного проекта

Скачайте [пример Подключенных служб ASP.NET Microsoft Graph](https://github.com/microsoftgraph/aspnet-connect-sample/archive/Office365connectedservice.zip). Этот пример включает ссылки, которые необходимо проверить на подлинность в Microsoft Graph. Скачав исходный проект, распакуйте и откройте пример в предварительной версии Visual Studio 2017.

## <a name="add-the-connected-service"></a>Добавление подключенной службы

Теперь можно добавить службу Microsoft Graph в проект Visual Studio. 

1. Выберите в обозревателе решений **Подключенные службы**, чтобы открыть одноименную вкладку. 

2. Выберите поставщика **Доступ к службам Microsoft 365 с помощью Microsoft Graph**. Следуйте указаниям мастера. Выберите следующие разрешения (позже их можно будет изменить):

    - Для API **File** установите разрешения **Полный доступ к вашим файлам**.
    - Для API **Mail** установите разрешения **Отправка почты от вашего имени**.
    - Для API **User** установите разрешения **Вход и чтение своего профиля**.

## <a name="call-the-microsoft-graph-api"></a>Вызов API Microsoft Graph

Настройки исходного приложения позволяют отправить простое письмо. Используя Microsoft Graph, вы можете сделать так, чтобы приложение отправляло письмо со ссылкой на фотографию из профиля вошедшего пользователя в OneDrive.

1. Откройте файл Models\GraphService.cs, который содержит код для вызова Microsoft Graph.

2. Найдите и **раскомментируйте** вызовы пакетов SDK в указанных ниже методах. Здесь показано, как вызвать Microsoft Graph, чтобы получить фотографию профиля, передать файл в OneDrive и получить ссылку для общего доступа.

    ```csharp
        GetCurrentUserPhotoStream(GraphServiceClient graphClient)
    ```
    
    ```csharp
        UploadFileToOneDrive(GraphServiceClient graphClient, byte[] file)
    ```

    ```csharp
        GetSharingLink(GraphServiceClient graphClient, string Id)
    ```
 
> **Совет.** Каждый комментарий начинается с "//Uncomment:"
 

## <a name="run-the-sample"></a>Запуск приложения
Выполните сборку и запуск приложения. Выберите ссылку **Sign-in** (Войти) справа вверху, а затем **Get email address** (Получить адрес электронной почты) и **Send email** (Отправить письмо).

В результате будет отправлено письмо со ссылкой на вашу фотографию профиля.

>**Примечания.**

>- Если вы остановите и перезапустите приложение в Visual Studio, для его работы может потребоваться выйти из учетной записи.
>- Если вы получите сообщение о том, что не выполнена проверка пользователя, повторите шаг [Добавление подключенной службы](#add-the-connected-service).
>- Войдите в систему с помощью учетной записи в том же домене, который вы выбрали на этапе **Выбор домена** в мастере.

## <a name="explore-the-code"></a>Обзор кода

Теперь можно использовать Visual Studio 2017 для подключения к службам и их настройки. Исходное приложение само создает шаблоны и ссылки.  

Исходное приложение включает следующие файлы:

- [Startup.Auth.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/App_Start/Startup.Auth.cs) выполняет аутентификацию текущего пользователя и инициализирует кэш маркеров приложения.

- TokenStorage\\[SessionTokenCache.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/TokenStorage/SessionTokenCache.cs) содержит сведения о маркере пользователя. Вы можете заменить его на собственный кэш маркеров. Дополнительные сведения см. в статье [Кэширование маркеров доступа в мультитенантном приложении](/azure/architecture/multitenant-identity/token-cache).

- Helpers\\[SampleAuthProvider.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SampleAuthProvider.cs) реализует локальный интерфейс IAuthProvider и получает маркер доступа. 

- Helpers\\[SDKHelper.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Helpers/SDKHelper.cs) инициализирует **GraphServiceClient** из [клиентской библиотеки Microsoft Graph .NET](https://github.com/microsoftgraph/msgraph-sdk-dotnet), которая используется для взаимодействия с Microsoft Graph.

- Controllers\\[HomeController.cs](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Controllers/HomeController.cs) содержит методы, использующие **GraphServiceClient** для создания и отправки вызовов в службу Microsoft Graph и обработки ответа.

- Views\\Home\\[Graph.cshtml](https://github.com/microsoftgraph/aspnet-connect-sample/tree/Office365connectedservice/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Microsoft%20Graph%20SDK%20ASPNET%20Sample/Views/Home/Graph.cshtml) содержит пользовательский интерфейс приложения. 


## <a name="need-help"></a>Нужна помощь?

Если вам нужна помощь, задайте вопрос на сайте [Вопросы и ответы Майкрософт](https://aka.ms/askgraph). Пометьте вопрос тегом {microsoft-graph-identity}.
