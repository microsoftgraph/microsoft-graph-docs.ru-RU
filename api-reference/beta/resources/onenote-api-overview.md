---
title: Использование REST API для OneNote
description: 'Microsoft Graph позволяет приложения могут получить авторизованные пользователя OneNote записные книжки, разделы и страницы в личный или организации учетной записи. С соответствующими делегированной или разрешения приложения, приложение может получать доступ к данным OneNote любого пользователя в клиент или пользователь выполнил вход. '
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 7db3024224dde7ee4c95d2e3840187709471cecd
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525628"
---
# <a name="use-the-onenote-rest-api"></a>Использование REST API для OneNote

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft Graph позволяет приложения могут получить авторизованные пользователя OneNote записные книжки, разделы и страницы в личный или организации учетной записи. С [соответствующими разрешениями делегированные или приложения](/graph/permissions-reference#notes-permissions)приложение может доступ к данным OneNote любого пользователя в клиент или пользователь выполнил вход. 

## <a name="root-url"></a>Корневой URL-адрес
Для всех вызовов API OneNote используется следующий формат корневого URL-адреса службы OneNote.
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

`version` Сегмента в URL-адрес представляет версию Microsoft Graph, который вы хотите использовать:

- Значение `v1.0` предназначено для стабильного производственного кода.
- Используйте значение `beta`, чтобы опробовать функцию, находящуюся на стадии разработки. Возможности и функции в конечной точке бета-версии может изменяться; не рекомендуется использовать в рабочем коде.

В качестве расположений можно задавать записные книжки пользователя в Office 365 или личные хранилища OneDrive, записные книжки группы (в том числе размещенные на сайте SharePoint) в Office 365. 

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
> **Примечание.** Вы можете получить идентификаторы пользователей, отправив запрос GET к конечной точке `https://graph.microsoft.com/v1.0/users`.

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenote-api-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
