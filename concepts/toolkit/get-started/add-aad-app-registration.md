---
title: Создание приложения Azure Active Directory
description: Создание регистрации приложения Azure Active Directory для связи с Microsoft 365
localization_priority: Normal
author: waldekmastykarz
ms.openlocfilehash: 13b3a876e80e5c2437eba3d264053cdbbcbb5909
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48982327"
---
# <a name="create-an-azure-active-directory-app-to-use-with-the-microsoft-graph-toolkit"></a>Создание приложения Azure Active Directory для использования с набором инструментов Microsoft Graph

API Microsoft Graph, который используется для подключения к Microsoft 365, защищен с помощью OAuth 2,0. Чтобы подключить приложение к Microsoft 365, вам потребуется создать приложение в Azure Active Directory (Azure AD) и предоставить этому приложению разрешения на доступ к определенным ресурсам от имени пользователя, использующего ваше приложение. В этом разделе описывается регистрация и Настройка веб-приложения для использования с набором средств Microsoft Graph.

## <a name="add-new-application-registration-in-azure-active-directory"></a>Добавление регистрации нового приложения в Azure Active Directory

Чтобы создать приложение в Azure Active Directory, необходимо добавить новую регистрацию приложения, а затем настроить имя приложения и расположение URL-адреса.

Чтобы создать приложение в Azure Active Directory, выполните следующие действия:

1. Перейдите на портал Azure по адресу https://portal.azure.com .
1. В меню выберите **Azure Active Directory**.
1. В меню Azure Active Directory выберите пункт **Регистрация приложений**.
1. В верхнем меню выберите **Новая кнопка регистрации** .
1. Введите имя приложения; для ексампе, `My M365 app` .
1. В разделе [Поддерживаемые типы учетных записей](/azure/active-directory/develop/single-and-multi-tenant-apps#who-can-sign-in-to-your-app)выберите **учетные записи в любом организационном каталоге (любой Azure AD Active Directory) и личных учетных записях Майкрософт (например, Skype, Xbox)**.
1. В поле **URI перенаправления** в раскрывающемся списке выберите **веб-сайт** , а в поле URL-адрес введите `https://localhost:3000` .
1. Подтвердите изменения, нажав кнопку **Регистрация** .

## <a name="enable-oauth-implicit-flow"></a>Включение неявного поток OAuth

В большинстве случаев набор средств набора инструментов Microsoft Graph будет использоваться в клиентских приложениях, состоящих только из клиентского кода. Так как клиентские приложения не могут хранить конфиденциальные данные безопасно, необходимо использовать [неявный поток OAuth](/azure/active-directory/develop/v2-oauth2-implicit-grant-flow?WT.mc_id=m365-10340-wmastyka), который предполагает удостоверение приложения на основе его идентификатора и URL-адреса.

1. На портале Azure откройте новую регистрацию приложения.
1. В меню выберите пункт **Проверка подлинности**.
1. В разделе **неявные гранты** включите параметры **маркеров доступа** и **маркеров идентификаторов** .
1. Подтвердите изменения, нажав кнопку **сохранить** .

## <a name="next-steps"></a>Дальнейшие действия

- [Создание веб-приложения](./build-a-web-app.md) (Ванилла JavaScript)
- [Создание вкладки Microsoft Teams](./build-a-microsoft-teams-tab.md)
- [Использование набора инструментов с откликом](./use-toolkit-with-react.md)
- [Использование набора инструментов с угловой](./use-toolkit-with-angular.md)
