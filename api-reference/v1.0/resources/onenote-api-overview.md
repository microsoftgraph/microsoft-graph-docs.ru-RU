---
title: Использование REST API для OneNote
description: Microsoft Graph позволяет приложения могут получить авторизованные пользователя OneNote записные книжки, разделы и страницы в личный или организации учетной записи. С соответствующими делегированной или разрешения приложения, приложение может получать доступ к данным OneNote любого пользователя в клиент или пользователь выполнил вход.
ms.openlocfilehash: c439e7896eea85e84d567e54aaa57bb5191a70d2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024799"
---
# <a name="use-the-onenote-rest-api"></a>Использование REST API для OneNote

Microsoft Graph позволяет приложения могут получить авторизованные пользователя OneNote записные книжки, разделы и страницы в личный или организации учетной записи. С [соответствующими разрешениями делегированные или приложения](/graph/permissions-reference#notes-permissions)приложение может доступ к данным OneNote любого пользователя в клиент или пользователь выполнил вход.

## <a name="root-url"></a>Корневой URL-адрес
Для всех вызовов API OneNote используется следующий формат корневого URL-адреса службы OneNote.
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```
`version` Сегмента в URL-адрес представляет версию Microsoft Graph, который вы хотите использовать:

- Значение `v1.0` предназначено для стабильного производственного кода.
- Используйте значение `beta`, чтобы опробовать функцию, находящуюся на стадии разработки. Возможности и функции в конечной точке бета-версии может изменяться; не рекомендуется использовать в рабочем коде.

Расположение может быть записных книжек пользователя на Office 365 или потребитель OneDrive, группа записных книжек или записных книжек размещенного сайта группы SharePoint на Office 365. 

![Стек разработки API-интерфейса OneNote](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a>Записные книжки пользователя
Для доступа к личные записные книжки на потребителей OneDrive или OneDrive для бизнеса, используйте один из следующих URL-адресов:

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- Значение `me` предназначено для содержимого OneNote, доступного текущему пользователю (если он является владельцем или с ним поделились этим содержимым).
- Значение `users/{id}` предназначено для содержимого OneNote, которым указанный (в URL-адресе) пользователь поделился с текущим пользователем. С помощью API [пользователей](users.md) .
> **Примечание:** Идентификаторы пользователей можно получить, выбрав запрос GET на `https://graph.microsoft.com/v1.0/users`.

### <a name="group-notebooks"></a>Группа записных книжек
Для доступа к записные книжки, владельцем которых является группу, используйте следующие корневой URL-адрес службы:

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a>Записные книжки сайта SharePoint

Для доступа к портативные компьютеры, принадлежащие сайту группы SharePoint, используйте следующие корневой URL-адрес службы:

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

