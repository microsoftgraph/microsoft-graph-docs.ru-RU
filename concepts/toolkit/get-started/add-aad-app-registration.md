---
title: Создание приложения Azure Active Directory
description: Создание регистрации приложения Azure Active Directory для связи с Microsoft 365
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 821cd6981ddb24e3917a4c0720f1c8c524081f54
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059569"
---
# <a name="create-an-azure-active-directory-app-to-use-with-the-microsoft-graph-toolkit"></a>Создание приложения Azure Active Directory для использования с Microsoft Graph Toolkit

Microsoft Graph — это API, используемый для подключения к Microsoft 365. Он защищен с помощью OAuth 2.0. Чтобы подключить приложение к Microsoft 365, вам потребуется создать приложение в Azure Active Directory (Azure AD) и предоставить этому приложению разрешения на доступ к определенным ресурсам от имени пользователя, применяющего ваше приложение. В этой статье описано, как зарегистрировать и настроить веб-приложение для использования с Microsoft Graph Toolkit.

## <a name="add-new-application-registration-in-azure-active-directory"></a>Добавление новой регистрации приложения в Azure Active Directory

Чтобы создать приложение в Azure Active Directory, вам требуется добавить новую регистрацию приложения, а затем настроить имя приложения и URL-адрес.

Создание приложения в Azure Active Directory:

1. Перейдите на портал Azure по адресу https://portal.azure.com.
1. В меню выберите **Azure Active Directory**.
1. В меню Azure Active Directory выберите **Регистрация приложений**.
1. В верхнем меню нажмите кнопку **Новая регистрация**.
1. Введите имя приложения; например, `My M365 app` .
1. Для параметра [Поддерживаемые типы учетных записей](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app) выберите **Учетные записи в любом каталоге организации (любой каталог Azure AD — мультитенантный) и персональные учетные записи Майкрософт (например, Skype, Xbox)**.
1. В разделе **URI перенаправления** в раскрывающемся списке выберите **Веб**, а в поле URL-адреса введите `http://localhost:3000`.
1. Подтвердите изменения, нажав кнопку **Зарегистрировать**.

## <a name="enable-oauth-implicit-flow"></a>Включение неявного потока OAuth

В большинстве случаев вы будете использовать Microsoft Graph Toolkit в клиентских приложениях, содержащих только клиентский код. Так как клиентские приложения не могут безопасно сохранять секреты, вам потребуется использовать [неявный поток OAuth](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka), в котором предполагается удостоверение приложения на основе его идентификатора и URL-адреса.

1. На портале Azure откройте созданную регистрацию приложения.
1. В меню выберите **Проверка подлинности**.
1. В разделе **Неявное предоставление разрешения** включите оба параметра: **Токены доступа** и **Токены ИД**
1. Подтвердите изменения, нажав кнопку **Сохранить**.

## <a name="next-steps"></a>Дальнейшие действия

- [Создание веб-приложения](./build-a-web-app.md) (обычный JavaScript)
- [Создание вкладки Microsoft Teams](./build-a-microsoft-teams-tab.md)
- [Использование набора средств Toolkit с React](./use-toolkit-with-react.md)
- [Использование набора средств Toolkit с Angular](./use-toolkit-with-angular.md)
