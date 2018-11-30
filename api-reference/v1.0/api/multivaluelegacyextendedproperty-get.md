---
title: Получение объекта multiValueLegacyExtendedProperty
description: Разверните узел ".
ms.openlocfilehash: c56afa8492954bcb68c5f36df00abdfce51cc2b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027909"
---
# <a name="get-multivaluelegacyextendedproperty"></a>Получение объекта multiValueLegacyExtendedProperty

Получение экземпляра ресурса, который содержит расширенное свойство с несколькими значениями, с использованием параметра `$expand`.

С помощью параметра запроса `$expand` вы можете получить указанный экземпляр, дополненный указанным расширенным свойством. Это пока единственный способ получить объект [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md), представляющий расширенное свойство.

Поддерживаются следующие ресурсы пользователей:

- [calendar](../resources/calendar.md);
- [contact](../resources/contact.md);
- [contactFolder](../resources/contactfolder.md). 
- [событие](../resources/event.md)
- [mailFolder](../resources/mailfolder.md)
- [message](../resources/message.md) 

Кроме того, поддерживаются следующие ресурсы групп:

- [calendar](../resources/calendar.md) для групп;
- [event](../resources/event.md) для групп;
- [post](../resources/post.md) для групп.

Дополнительные сведения о том, когда следует использовать расширенные свойства или открытые расширения и как задавать расширенные свойства, см. в статье [Обзор расширенных свойств](../resources/extended-properties-overview.md).

## <a name="permissions"></a>Разрешения
В зависимости от ресурса они будут расширенные свойства из и разрешение введите (делегированные или приложения) вы запроса, разрешение, указанное в следующей таблице является минимальным необходимым условием для вызова этот интерфейс API. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Поддерживаемый ресурс | Делегированные (рабочая или учебная учетная запись) | Делегированные (личная учетная запись Майкрософт) | Для приложения |
|:-----|:-----|:-----|:-----|
| [calendar](../resources/calendar.md) | Calendars.Read | Calendars.Read | Calendars.Read |
| [контакт](../resources/contact.md) | Contacts.Read | Contacts.Read | Contacts.Read |
| [contactFolder](../resources/contactfolder.md). | Contacts.Read | Contacts.Read | Contacts.Read |
| [событие](../resources/event.md) | Calendars.Read | Calendars.Read |  Calendars.Read|
| [calendar](../resources/calendar.md) для групп; | Group.Read.All | Не поддерживается | Не поддерживается |
| [event](../resources/event.md) для групп; | Group.Read.All | Не поддерживается | Не поддерживается |
| [post](../resources/post.md) для групп. | Group.Read.All | Не поддерживается | Group.Read.All |
| [mailFolder](../resources/mailfolder.md) | Mail.Read | Mail.Read | Mail.Read |
| [message](../resources/message.md) | Mail.Read | Mail.Read | Mail.Read |
 
## <a name="http-request"></a>HTTP-запрос

Вы можете получить экземпляр ресурса, дополненный расширенным свойством, которое совпадает с фильтром в свойстве **id**. Убедитесь, что вы применяете [кодировку URL](https://www.w3schools.com/tags/ref_urlencode.asp) для символов пробелов в строке фильтра.

Получение экземпляра **сообщения** :<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/mailFolders/{id}/messages/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
Получение экземпляра **mailFolder** :<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/mailFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

Получение экземпляра **событий** :<!-- { "blockType": "ignored" } -->
```http
GET /me/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
Получение экземпляра **календаря** :<!-- { "blockType": "ignored" } -->
```http
GET /me/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/calendars/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
Получение экземпляра **контактов** :<!-- { "blockType": "ignored" } -->
```http
GET /me/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /me/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}/contacts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
Получение экземпляра **contactFolder** :<!-- { "blockType": "ignored" } -->
```http
GET /me/contactfolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /users/{id|userPrincipalName}/contactFolders/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```
Получение экземпляра **события** группы:<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

Получение экземпляра **публиковать** группы:<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
GET /groups/{id}/conversations/{id}/threads/{id}/posts/{id}?$expand=multiValueExtendedProperties($filter=id eq '{id_value}')
```

## <a name="path-parameters"></a>Параметры пути
|Параметр|Тип|Description|
|:-----|:-----|:-----|
|id_value|String|Идентификатор расширенного свойства, для которого необходимо найти совпадение. Свойство должно иметь один из поддерживаемых форматов. Дополнительные сведения см. в статье [Обзор расширенных свойств Outlook](../resources/extended-properties-overview.md). Обязательный.|

## <a name="request-headers"></a>Заголовки запросов
| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте тело запроса для этого метода.

## <a name="response"></a>Ответ

При успешном выполнении этот метод возвращает код отклика `200 OK`. 

Основной текст отклика содержит объект, который представляет запрошенный экземпляр ресурса, дополненный соответствующим объектом [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В этом примере показано, как получить указанное событие и дополнить его расширенным свойством с несколькими значениями. Фильтр возвращает расширенное свойство, у которого параметр **id** совпадает со строкой `StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation` (здесь кодировка URL удалена для улучшения читаемости).

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/events('AAMkAGE1M2_bs88AACbuFiiAAA=')?$expand=multiValueExtendedProperties($filter=id%20eq%20'StringArray%20{66f5a359-4659-4830-9070-00050ec6ac6e}%20Name%20Recreation')
```
##### <a name="response"></a>Отклик

Основной текст отклика включает в себя все свойства указанного события и расширенное свойство, возвращенное из фильтра.

Примечание. Показанный здесь объект **event** усечен для краткости. Все свойства будут возвращены при фактическом вызове.

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
Content-type: application/json
{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/users('ddfcd489-628b-40d7-b48b-57002df800e5@1717622f-1d94-4d0c-9d74-709fad664b77')/events('AAMkAGE1M2_bs88AACbuFiiAAA=')",
    "@odata.etag": "W/\"mODEKWhc/Um6lA3uPm7PPAAAm8k15A==\"",
    "id": "AAMkAGE1M2_bs88AACbuFiiAAA=",
    "start": {
        "dateTime": "2015-11-26T17:00:00.0000000",
        "timeZone": "UTC"
    },
    "end": {
        "dateTime": "2015-11-30T05:00:00.0000000",
        "timeZone": "UTC"
    },
    "organizer": {
        "emailAddress": {
            "name": "Christine Irwin",
            "address": "christine@contoso.com"
        }
    },
    "multiValueExtendedProperties@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Me/events('AAMkAGE1M2_bs88AACbuFiiAAA%3D')/multiValueExtendedProperties",
    "multiValueExtendedProperties": [
        {
            "id": "StringArray {66f5a359-4659-4830-9070-00050ec6ac6e} Name Recreation",
            "value": [
                "Food",
                "Hiking",
                "Swimming"
            ]
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get multiValueLegacyExtendedProperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->