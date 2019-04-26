---
title: Использование REST API для OneNote
description: 'Microsoft Graph позволяет приложению получать авторизованный доступ к записным книжкам OneNote, разделам и страницам пользователя в личной учетной записи или организации. Используя соответствующие разрешения делегирования или приложения, ваше приложение может получить доступ к данным OneNote вошедшего пользователя или любого пользователя в клиенте. '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 6d92faecfd58c74f519802fe308071828a3713dc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345556"
---
# <a name="use-the-onenote-rest-api"></a>Использование REST API для OneNote

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph позволяет приложению получать авторизованный доступ к записным книжкам OneNote, разделам и страницам пользователя в личной учетной записи или организации. Используя [соответствующие разрешения делегирования или приложения](/graph/permissions-reference#notes-permissions), ваше приложение может получить доступ к данным OneNote вошедшего пользователя или любого пользователя в клиенте. 

## <a name="root-url"></a>Корневой URL-адрес
В корневом URL-АДРЕСе службы OneNote для всех вызовов API OneNote используется следующий формат.
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

`version` Сегмент в URL-адресе представляет версию Microsoft Graph, которую вы хотите использовать:

- Значение `v1.0` предназначено для стабильного производственного кода.
- Используйте значение `beta`, чтобы опробовать функцию, находящуюся на стадии разработки. Функции и функции в конечной точке бета-версии могут измениться; Мы не рекомендуем использовать его в рабочем коде.

Местоположение может представлять собой записные книжки для пользователей в Office 365 или OneDrive для пользователей, групповых записных книжек или размещенных на сайте SharePoint записных книжек группы в Office 365. 

![Стек разработки API OneNote](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a>Записные книжки пользователя
Чтобы получить доступ к личным записным книжкам в OneDrive для бизнеса или OneDrive для бизнеса, используйте один из следующих URL-адресов:

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- Значение `me` предназначено для содержимого OneNote, доступного текущему пользователю (если он является владельцем или с ним поделились этим содержимым).
- Значение `users/{id}` предназначено для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем. Использование API [пользователей](users.md) .
> **Примечание:** Вы можете получить идентификаторы пользователей, выполнив запрос GET `https://graph.microsoft.com/v1.0/users`.

### <a name="group-notebooks"></a>Записные книжки для групп

Чтобы получить доступ к записным книжкам, принадлежащим группе, используйте следующий корневой URL-адрес службы:

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a>Записные книжки сайта SharePoint
Чтобы получить доступ к записным книжкам, принадлежащим сайту группы SharePoint, используйте следующий корневой URL-адрес службы:

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
