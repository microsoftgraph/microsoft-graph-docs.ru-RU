---
title: Создание многозначного расширенного свойства
description: 'Создание одного или нескольких многозначных расширенных свойств в новом или существующем экземпляре ресурса. '
localization_priority: Normal
ms.openlocfilehash: ba54bc3de2eb80fd7283f1a313448b77a04bbe4d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510871"
---
# <a name="create-multi-value-extended-property"></a>Создание многозначного расширенного свойства

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание одного или нескольких многозначных расширенных свойств в новом или существующем экземпляре ресурса. 

Поддерживаются следующие ресурсы пользователей:

- [calendar](../resources/calendar.md);
- [contact](../resources/contact.md);
- [contactFolder](../resources/contactfolder.md). 
- [event](../resources/event.md)
- [mailFolder](../resources/mailfolder.md)
- [message](../resources/message.md)
- [Задача Outlook](../resources/outlooktask.md)
- [Папки задач Outlook](../resources/outlooktaskfolder.md)

Кроме того, поддерживаются следующие ресурсы групп:

- [calendar](../resources/calendar.md) для групп;
- [event](../resources/event.md) для групп;
- [post](../resources/post.md) для групп. 

Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).

## <a name="permissions"></a>Разрешения
В зависимости от ресурса при создании расширенные свойства в и введите (делегированные или приложения) вы запроса на разрешение, разрешение, указанное в следующей таблице является минимальным необходимым условием для вызова этот интерфейс API. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Поддерживаемый ресурс | Делегированное (рабочая или учебная учетная запись) | Делегированное (личная учетная запись Майкрософт) | Для приложений |
|:-----|:-----|:-----|:-----|
| [calendar](../resources/calendar.md) | Calendars.ReadWrite | Calendars.ReadWrite | Calendars.ReadWrite |
| [contact](../resources/contact.md) | Contacts.ReadWrite | Contacts.ReadWrite | Contacts.ReadWrite |
| [contactFolder](../resources/contactfolder.md). | Contacts.ReadWrite | Contacts.ReadWrite | Contacts.ReadWrite |
| [event](../resources/event.md) | Calendars.ReadWrite | Calendars.ReadWrite |  Calendars.ReadWrite|
| [calendar](../resources/calendar.md) для групп; | Group.ReadWrite.All | Не поддерживается | Не поддерживается |
| [event](../resources/event.md) для групп; | Group.ReadWrite.All | Не поддерживается | Не поддерживается |
| [post](../resources/post.md) для групп. | Group.ReadWrite.All | Не поддерживается | Не поддерживается |
| [mailFolder](../resources/mailfolder.md) | Mail.ReadWrite | Mail.ReadWrite | Mail.ReadWrite |
| [message](../resources/message.md) | Mail.ReadWrite | Mail.ReadWrite | Mail.ReadWrite |
| [Задача Outlook](../resources/outlooktask.md) | Tasks.ReadWrite | Tasks.ReadWrite | Не поддерживается |
| [Папки задач Outlook](../resources/outlooktaskfolder.md) | Tasks.ReadWrite | Tasks.ReadWrite | Не поддерживается |

## <a name="http-request"></a>HTTP-запрос
Вы можете создавать расширенные свойства в новом или существующем экземпляре ресурса.

Создайте один или несколько расширенных свойств в _новый_ экземпляр ресурсов, использование того же запроса REST создания экземпляра и включить свойства нового ресурса экземпляра _и расширенные свойства_ в тексте запроса.
Обратите внимание, что некоторые ресурсы поддержки в несколько способов создания. Дополнительные сведения о создании этих экземплярах ресурсов см в соответствующие разделы для создания [сообщения](../resources/message.md), [mailFolder](../api/user-post-mailfolders.md), [события](../api/user-post-events.md), [календаря](../api/user-post-calendars.md), [контактов](../api/user-post-contacts.md), [contactFolder](../api/user-post-contactfolders.md) [задач Outlook](../resources/outlooktask.md), [ Папки задач Outlook](../resources/outlooktaskfolder.md), [событие группы](../api/group-post-events.md)и [группы post](../resources/post.md). 
 
Ниже приведен синтаксис запросов. 

<!-- { "blockType": "ignored" } -->
```http
POST /me/messages
POST /users/{id|userPrincipalName}/messages
POST /me/mailFolders/{id}/messages

POST /me/mailFolders
POST /users/{id|userPrincipalName}/mailFolders

POST /me/events
POST /users/{id|userPrincipalName}/events

POST /me/calendars
POST /users/{id|userPrincipalName}/calendars

POST /me/contacts
POST /users/{id|userPrincipalName}/contacts

POST /me/contactFolders
POST /users/{id|userPrincipalName}/contactFolders

POST /me/outlook/tasks
POST /users/{id|userPrincipalName}/outlook/tasks
POST /me/outlook/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks
POST /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks

POST /me/outlook/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskFolders
POST /me/outlook/taskGroups/{id}/taskFolders
POST /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders

POST /groups/{id}/events

POST /groups/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/reply
POST /groups/{id}/threads/{id}/reply
POST /groups/{id}/conversations/{id}/threads/{id}/reply
POST /groups/{id}/threads
POST /groups/{id}/conversations
```

Чтобы создать одно или несколько расширенных свойств в существующем экземпляре ресурса, укажите экземпляр в запросе и включите расширенное свойство в тело запроса.

**Примечание.** Расширенное свойство невозможно создать в существующем экземпляре post для групп.

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id|userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}

PATCH /me/mailFolders/{id}
PATCH /users/{id|userPrincipalName}/mailFolders/{id}

PATCH /me/events/{id}
PATCH /users/{id|userPrincipalName}/events/{id}

PATCH /me/calendars/{id}
PATCH /users/{id|userPrincipalName}/calendars/{id}

PATCH /me/contacts/{id}
PATCH /users/{id|userPrincipalName}/contacts/{id}

PATCH /me/contactFolders/{id}
PATCH /users/{id|userPrincipalName}/contactFolders/{id}

PATCH /me/outlook/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/tasks/{id}
PATCH /me/outlook/taskFolders/{id}/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}/tasks/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}/tasks/{id}

PATCH /me/outlook/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskFolders/{id}
PATCH /me/outlook/taskGroups/{id}/taskFolders/{id}
PATCH /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}

PATCH /groups/{id}/events/{id}
```

## <a name="request-headers"></a>Заголовки запросов
| Имя       | Значение |
|:---------------|:----------|
| Авторизация | Bearer {токен}. Обязательный. |
| Content-Type | application/json |

## <a name="request-body"></a>Тело запроса

Предоставьте тело в формате JSON для каждого объекта [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) в свойстве коллекции **multiValueExtendedProperties** для экземпляра ресурса.

|**Свойство**|**Тип**|**Описание**|
|:-----|:-----|:-----|
|multiValueExtendedProperties|Коллекция [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md)| Массив из одного или нескольких многозначных расширенных свойств. |
|id|String|Чтобы идентифицировать свойства в коллекции **multiValueExtendedProperties**, укажите этот параметр для каждого из них. Свойство должно относиться к одному из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный параметр.|
|значение|строка|Укажите значение для каждого свойства в коллекции **multiValueExtendedProperties**. Обязательный параметр.|

При создании расширенного свойства в _новом_ экземпляре ресурса, помимо новой коллекции **multiValueExtendedProperties**, нужно указать описание этого экземпляра ресурса (то есть [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md) и т. д.) в формате JSON.

## <a name="response"></a>Отклик

#### <a name="response-code"></a>Код отклика
В результате успешной операции создания расширенного свойства в новом экземпляре ресурса возвращается код `201 Created` (в случае post для групп в зависимости от используемого метода операция может возвращать код `200 OK` или `202 Accepted`).

В результате успешной операции создания в существующем экземпляре ресурса возвращается код `200 OK`. 


#### <a name="response-body"></a>Тело отклика

При создании расширенного свойства в поддерживаемом ресурсе, отличном от [post для групп](../resources/post.md), отклик включает только новый или существующий экземпляр (он будет без нового расширенного свойства). Чтобы просмотреть только что созданное расширенное свойство, [разверните экземпляр с этим свойством](../api/multivaluelegacyextendedproperty-get.md).

При создании расширенного свойства в _новом_ экземпляре post для групп отклик включает только код отклика и не содержит ни новой записи, ни расширенного свойства. Расширенное свойство невозможно создать в существующем экземпляре post для групп.


## <a name="example"></a>Пример
##### <a name="request-1"></a>Запрос 1

В первом примере в новом экземпляре event создается многозначное расширенное свойство с помощью одной операции POST. Помимо свойств, которые обычно указываются для нового события, тело запроса включает коллекцию **multiValueExtendedProperties**, которая содержит одно расширенное свойство. Тело запроса включает следующие данные для многозначного расширенного свойства:

- **id**. Задает свойство в виде массива строк с заданным идентификатором GUID и именем `Recreation`. 
- **value**. Задает `Recreation` в виде массива из 3 строковых значений, `["Food", "Hiking", "Swimming"]`.
 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/beta/me/events
Content-Type: application/json

{
  "subject": "Family reunion",
  "body": {
    "contentType": "HTML",
    "content": "Let's get together this Thanksgiving!"
  },
  "start": {
      "dateTime": "2015-11-26T09:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "end": {
      "dateTime": "2015-11-29T21:00:00",
      "timeZone": "Pacific Standard Time"
  },
  "attendees": [
    {
      "emailAddress": {
        "address": "Terrie@contoso.com",
        "name": "Terrie Barrera"
      },
      "type": "Required"
    },
    {
      "emailAddress": {
        "address": "Lauren@contoso.com",
        "name": "Lauren Solis"
      },
      "type": "Required"
    }
  ],
  "multiValueExtendedProperties": [
     {
           "id":"StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
           "value": ["Food", "Hiking", "Swimming"]
     }
  ]
}
```

##### <a name="response-1"></a>Отклик 1

Отклик в результате успешного выполнения обозначен кодом `HTTP 201 Created` и включает в себя новое событие, подобно отклику при [создании просто события](../api/user-post-events.md). Отклик не включает только что созданные расширенные свойства.

Чтобы просмотреть новое расширенное свойство, [разверните event с этим свойством](../api/multivaluelegacyextendedproperty-get.md).


****

##### <a name="request-2"></a>Запрос 2

Во втором примере создается многозначное расширенное свойство для указанного сообщения. Это расширенное свойство — единственный элемент в коллекции **multiValueExtendedProperties**. Тело запроса включает следующие данные для расширенного свойства:

- **id**. Задает свойство в виде массива строк с указанным идентификатором GUID и именем `Palette`.
- **value**. Задает `Palette` в виде массива 3 строковых значений, `["Green", "Aqua", "Blue"]`.

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/beta/me/messages('AAMkAGE1M2_as77AACHsLrBBBA=')

Content-Type: application/json

{
  "multiValueExtendedProperties": [
      {
         "id":"StringArray {66f5a359-4659-4830-9070-00049ec6ac6e} Name Palette",
         "value":["Green", "Aqua", "Blue"]
      }
    ]
}
```

##### <a name="response-2"></a>Отклик 2

Отклик в результате успешного выполнения обозначен кодом `HTTP 200 OK` и включает в себя указанное сообщение подобно отклику при [обновлении сообщения](../api/message-update.md). Отклик не включает только что созданное расширенное свойство.

Чтобы просмотреть новое расширенное свойство, [разверните message с этим свойством](../api/multivaluelegacyextendedproperty-get.md).


<!-- This page was manually created. -->
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create a single-value extended property",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->




