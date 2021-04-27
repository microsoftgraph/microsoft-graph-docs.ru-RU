---
title: Получение контакта
description: Извлечение свойств и связей контактного объекта.
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6bd7036e86315870e3cea8b39e41a79ff080f9f1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047121"
---
# <a name="get-contact"></a>Вывод контакта

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение свойств и связей контактного объекта.

Существует два сценария, в которых приложение может получить контакт в папке контактов другого пользователя:

* У приложения есть разрешения для приложений; или
* У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой контактов или предоставил ему делегированный доступ. См. [подробные сведения и пример](/graph/outlook-get-shared-contacts-folders).


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Contacts.Read, Contacts.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Contacts.Read, Contacts.ReadWrite    |
|Для приложений | Contacts.Read, Contacts.ReadWrite |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
Контакт [в](../resources/contact.md) почтовом ящике пользователя.
```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
Контакт [с](../resources/contact.md) верхнего уровня [contactFolder](../resources/contactfolder.md) пользователя.
```http
GET /me/contactfolders/{Id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```
Объект [contact](../resources/contact.md) из дочерней папки в папке [contactFolder](../resources/mailfolder.md).  Приведенный ниже пример показывает один уровень вложенности, но для хранения контакта допускается несколько.
```http
GET /me/contactFolders/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="optional-query-parameters"></a>Необязательные параметры запросов
|Имя|Значение|Описание|
|:---------------|:--------|:-------|
|$expand|string|Список отношений, развертываемых и включаемых в ответ (разделитель — запятая). См. таблицу [связей контактного](../resources/contact.md) объекта для поддерживаемых имен. |
|$select|string|Разделенный запятыми список свойств, включаемых в ответ.|

## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и объект [contact](../resources/contact.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contact"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/contacts/AAMkAGI2THk0AAA=
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "AAMkAGI2THk0AAA=",
  "createdDateTime": "2014-10-19T23:08:24Z",
  "lastModifiedDateTime": "2014-10-19T23:08:24Z",
  "changeKey": "EQAAABYAAACd9nJ/tVysQos2hTfspaWRAAADTIa4",
  "categories": [],
  "parentFolderId": "AAMkAGI2AAEOAAA=",
  "birthday": "1974-07-22",
  "fileAs": "Fort, Garth",
  "displayName": "Garth Fort",
  "givenName": "Garth",
  "initials": "G.F.",
  "middleName": null,
  "nickName": "Garth",
  "surname": "Fort",
  "title": null,
  "yomiGivenName": null,
  "yomiSurname": null,
  "yomiCompanyName": null,
  "generation": null,
  "emailAddresses": [
    {
      "name": "Garth",
      "address": "garth@a830edad9050849NDA1.onmicrosoft.com",
      "type": "unknown"
    },
    {
      "name": "Garth",
      "address": "garth@contoso.onmicrosoft.com",
      "type": "personal"
    }
  ],
  "imAddresses": [
    "sip:garthf@a830edad9050849nda1.onmicrosoft.com"
  ],
  "jobTitle": "Web Marketing Manager",
  "companyName": "Contoso, Inc.",
  "department": "Sales & Marketing",
  "officeLocation": "20/1101",
  "profession": null,
  "assistantName": null,
  "manager": null,
  "phones": [{
    "type": "business",
    "number": "+1 918 555 0101"
  }],
  "postalAddresses": [{
    "type": "business",
    "postOfficeBox": "P.O. Box 100",
    "street": "123 Some street",
    "city": "Seattle",
    "state": "WA",
    "countryOrRegion": "USA",
    "postalCode": "98121"
  }],
  "spouseName": null,
  "personalNotes": null,
  "children": [], 
  "gender": null,
  "websites": [{
      "type": "work",
      "address": "https://www.contoso.com",
      "name": "Contoso"
  }],
  "weddingAnniversary": null
}
```

## <a name="see-also"></a>См. также

- [Добавление пользовательских данных в ресурсы с помощью расширений](/graph/extensibility-overview)
- [Добавление пользовательских данных в ресурсы user с помощью открытых расширений (предварительная версия)](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


