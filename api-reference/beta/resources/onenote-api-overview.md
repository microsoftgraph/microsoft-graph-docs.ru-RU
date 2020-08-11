---
title: Использование REST API для OneNote
description: 'Microsoft Graph позволяет вашему приложению получать авторизованный доступ к записным книжкам, разделам и страницам OneNote в личной или организационной учетной записи. Имея соответствующие разрешения приложения или делегированные разрешения, приложение может получать доступ к данным OneNote вошедшего пользователя или любого пользователя в клиенте. '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
doc_type: conceptualPageType
ms.openlocfilehash: 0c13ebeb6381e894684a14be42772d69b5d31e62
ms.sourcegitcommit: ab36e03d6bcb5327102214eb078d55709579d465
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630328"
---
# <a name="use-the-onenote-rest-api"></a>Использование REST API для OneNote

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph позволяет вашему приложению получать авторизованный доступ к записным книжкам, разделам и страницам OneNote в личной или организационной учетной записи. Имея [соответствующие разрешения приложения или делегированные разрешения](/graph/permissions-reference#notes-permissions), приложение может получать доступ к данным OneNote вошедшего пользователя или любого пользователя в клиенте. 

## <a name="root-url"></a>Корневой URL-адрес
Для всех вызовов API OneNote используется следующий формат корневого URL-адреса службы OneNote.

```http
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

Сегмент `version` URL-адреса представляет нужную версию Microsoft Graph.

- Значение `v1.0` предназначено для стабильного производственного кода.
- Используйте значение `beta`, чтобы опробовать функцию, находящуюся на стадии разработки. Функции бета-версии конечной точки могут меняться. Не рекомендуем использовать ее в рабочем коде.

Местоположение может представлять собой записные книжки для пользователей в Microsoft 365 или OneDrive для пользователей, групповые записные книжки или записные книжки группы SharePoint, размещенные на сайте Microsoft 365. 

![Стек разработки API OneNote](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

## <a name="user-notebooks"></a>Записные книжки пользователей
Чтобы получить доступ к персональным записным книжкам в OneDrive для бизнеса или личном хранилище OneDrive, воспользуйтесь одним из следующих URL-адресов:

```http
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- Значение `me` предназначено для содержимого OneNote, доступного текущему пользователю (если он является владельцем или с ним поделились этим содержимым).
- Значение `users/{id}` предназначено для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем. Используйте API для работы с [пользователями](users.md).
> **Примечание.** Вы можете получить идентификаторы пользователей, отправив запрос GET к конечной точке `https://graph.microsoft.com/v1.0/users`.

## <a name="group-notebooks"></a>Записные книжки группы

Чтобы получить доступ к записным книжкам группы, воспользуйтесь следующим корневым URL-адресом службы:

```http
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
## <a name="sharepoint-site-notebooks"></a>Записные книжки на сайте SharePoint
Чтобы получить доступ к записным книжкам на сайте группы SharePoint, воспользуйтесь следующим корневым URL-адресом службы:

```http
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="whats-new"></a>Новые возможности
Узнайте о [новых функциях и обновлениях](/graph/whats-new-overview) для этого набора API.
