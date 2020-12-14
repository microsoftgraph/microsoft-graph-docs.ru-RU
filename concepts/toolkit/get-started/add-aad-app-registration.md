---
title: Создание приложения Azure Active Directory
description: Создание регистрации приложения Azure Active Directory для связи с Microsoft 365
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 7534d0d15b9ff1b2e1d94fe8d5e8e9e8f771ca91
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49659171"
---
# <a name="create-an-azure-active-directory-app-to-use-with-the-microsoft-graph-toolkit"></a>Создание приложения Azure Active Directory для использования с microsoft Graph набор средств

Microsoft Graph, API, который вы используете для подключения к Microsoft 365, защищен с помощью OAuth 2.0. Чтобы подключить приложение к Microsoft 365, необходимо создать приложение в Azure Active Directory (Azure AD) и предоставить этому приложению разрешения на доступ к определенным ресурсам от имени пользователя, используюшего ваше приложение. В этом разделе описывается регистрация и настройка веб-приложения для использования с Microsoft Graph набор средств.

## <a name="add-new-application-registration-in-azure-active-directory"></a>Добавление регистрации нового приложения в Azure Active Directory

Чтобы создать приложение в Azure Active Directory, необходимо добавить новую регистрацию приложения, а затем настроить имя и URL-адрес приложения.

Чтобы создать приложение в Azure Active Directory:

1. Перейдите на портал Azure по https://portal.azure.com ссылке .
1. В меню выберите **Azure Active Directory.**
1. В меню Azure Active Directory выберите **регистрацию приложений.**
1. В верхнем меню выберите кнопку **"Новая регистрация".**
1. Введите имя приложения; для экзаменов, `My M365 app` .
1. Для типа [](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)поддерживаемых типов учетных записей выберите "Учетные записи" в любом каталоге организации **(любой каталог Azure AD — мультитенантный)** и личных учетных записях Майкрософт (например, Skype, Xbox).
1. В поле **URI** перенаправления в dropdown выберите **"Интернет"** и введите в поле URL-адреса `http://localhost:3000` .
1. Подтвердив изменения, нажать кнопку **"Регистрация".**

## <a name="enable-oauth-implicit-flow"></a>Включить неявный поток OAuth

В большинстве случаев microsoft Graph набор средств клиентских приложениях, состоящих только из клиентского кода. Так как клиентские приложения не могут безопасно хранить секреты, необходимо использовать неявный поток [OAuth,](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka)который предполагает удостоверение приложения на основе его идентификатора и URL-адреса.

1. На портале Azure откройте только что созданную регистрацию приложения.
1. В меню выберите пункт **"Проверка подлинности".**
1. В разделе **неявного предоставления** в enable both **Access tokens** and **ID tokens** options.
1. Подтвердите изменения, нажатием кнопки **"Сохранить".**

## <a name="next-steps"></a>Дальнейшие действия

- [Создание веб-приложения](./build-a-web-app.md) (javaScript)
- [Создание вкладки Microsoft Teams](./build-a-microsoft-teams-tab.md)
- [Использование набор средств React](./use-toolkit-with-react.md)
- [Использование набор средств с Angular](./use-toolkit-with-angular.md)
