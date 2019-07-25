---
title: Обновление контакта
description: Обновление свойств объекта Contact.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: e8e1bb9332ca6a5821e0c17d12060a9f4044a983
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863359"
---
# <a name="update-contact"></a>Обновление контакта

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновление свойств объекта Contact.
## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Contacts.ReadWrite    |
|Делегированные (личная учетная запись Майкрософт) | Contacts.ReadWrite    |
|Для приложений | Contacts.ReadWrite |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
[Контакт](../resources/contact.md) от [contactFolder](../resources/contactfolder.md)пользователя по умолчанию.
```http
PATCH /me/contacts/{id}
PATCH /users/{id | userPrincipalName}/contacts/{id}
```
Объект [contact](../resources/contact.md) из пользовательской папки [contactFolder](../resources/contactfolder.md) верхнего уровня.
```http
PATCH /me/contactFolders/{id}/contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/contacts/{id}
```
Объект [contact](../resources/contact.md) из дочерней папки в папке [contactFolder](../resources/mailfolder.md).  Приведенный ниже пример показывает один уровень вложенности, но для хранения контакта допускается несколько.
```http
PATCH /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```
## <a name="request-headers"></a>Заголовки запросов
| Заголовок       | Значение |
|:---------------|:--------|
| Авторизация  | Bearer {токен}. Обязательный.  |
| Content-Type  | application/json. Обязательный.  |

## <a name="request-body"></a>Текст запроса
В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.

| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|assistantName|String|Имя помощника контакта.|
|birthday|DateTimeOffset|Дата рождения контакта.|
|categories|String|Категории, связанные с контактом.|
|children|String||
|companyName|String|Название компании контакта.|
|department|String|Отдел контакта.|
|displayName|Строка|Отображаемое имя контакта. Обратите внимание, что последующие обновления других свойств могут привести к тому, что автоматически созданное значение перезапишет указанное значение displayName. Чтобы сохранить существующее значение, всегда добавляйте его как displayName в операцию обновления.|
|emailAddresses|Коллекция [типедемаиладдресс](../resources/typedemailaddress.md)|Электронные адреса контакта.|
|fileAs|String|Имя, под которым хранится контакт.|
|gender |String |Пол контакта. |
|generation|String|Поколение контакта.|
|givenName|String|Имя контакта.|
|imAddresses|String|Адреса контакта для обмена мгновенными сообщениями.|
|initials|String|Инициалы контакта.|
|jobTitle|String|Должность контакта.|
|manager|String|Имя руководителя контакта.
|middleName|String|Отчество контакта.|
|nickName|String|Псевдоним контакта.|
|officeLocation|String|Расположение офиса контакта.|
|parentFolderId|Строка|Идентификатор родительской папки контакта.|
|personalNotes|String|Заметки пользователя о контакте.|
|phones |Коллекция [phone](../resources/phone.md) |Номера телефонов, связанные с контактом, например домашний телефон, мобильный телефон и служебный телефон. |
|postalAddresses |Коллекция [physicalAddress](../resources/physicaladdress.md) |Адреса, связанные с контактом, например домашний адрес и служебный адрес. |
|profession|String|Профессия контакта.|
|spouseName|String|Имя супруга или супруги контакта.|
|surname|String|Фамилия контакта.|
|title|String|Звание контакта.|
|websites |Коллекция [website](../resources/website.md)|Веб-сайты, связанные с контактом. |
|Веддинганниверсари |Дата |Годовщина свадьбы контакта. |
|yomiCompanyName|String|Название компании контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.|
|yomiGivenName|String|Имя контакта, записанное так, как оно звучит по-японски. Это необязательное свойство.|
|yomiSurname|String|Фамилия контакта, записанная так, как она звучит по-японски. Это необязательное свойство.|

Так как **контактный** ресурс поддерживает [расширения](/graph/extensibility-overview), с помощью `PATCH` операции можно добавлять, обновлять или удалять собственные данные, относящиеся к приложению, в пользовательских свойствах расширения в существующем экземпляре **контакта** .

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [Contact](../resources/contact.md) в тексте отклика.
## <a name="example"></a>Пример
##### <a name="request"></a>Запрос
В следующем примере обновляется личный адрес электронной почты указанного контакта.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contact"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contacts/AAMkADh6v5AAAvgTCEAAA=
Content-type: application/json

{
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
          "address": "pavelb@fabrikam.onmicrosoft.com",
          "name": "Pavel Bansky",
          "type": "other",
          "otherLabel": "Volunteer work"
        }
    ]
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contact-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contact-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Цель — C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contact-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-contact-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>Отклик
Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contact"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('c3e1fcd2-db78-42a8-aec5-1f2cd59abb5c')/contacts/$entity",
    "@odata.etag":"W/\"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh\"",
    "id":"AAMkADh6v5AAAvgTCEAAA=",
    "createdDateTime":"2018-06-11T19:56:07Z",
    "lastModifiedDateTime":"2018-06-11T20:26:23Z",
    "changeKey":"EQAAABYAAACv7At+UNVFRLhGciJGF6v5AAAve7fh",
    "categories":[

    ],
    "parentFolderId":"AAMkADh6v5AAAAAAEOAAA=",
    "birthday":null,
    "fileAs":"",
    "displayName":"Pavel Bansky",
    "givenName":"Pavel",
    "initials":null,
    "middleName":null,
    "nickName":null,
    "surname":"Bansky",
    "title":null,
    "yomiGivenName":null,
    "yomiSurname":null,
    "yomiCompanyName":null,
    "generation":null,
    "imAddresses":[

    ],
    "jobTitle":null,
    "companyName":null,
    "department":null,
    "officeLocation":null,
    "profession":null,
    "assistantName":null,
    "manager":null,
    "spouseName":null,
    "personalNotes":"",
    "children":[

    ],
    "gender":null,
    "isFavorite":null,
    "emailAddresses":[
        {
            "type":"personal",
            "name":"Pavel Bansky",
            "address":"pavelb@adatum.onmicrosoft.com"
        },
        {
            "type":"other",
            "otherLabel":"Volunteer work",
            "name":"Pavel Bansky",
            "address":"pavelb@fabrikam.onmicrosoft.com"
        }
    ],
    "websites":[

    ],
    "phones":[
        {
            "type":"business",
            "number":"+1 732 555 0102"
        }
    ],
    "postalAddresses":[

    ],
    "flag":{
        "flagStatus":"notFlagged"
    }
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
  "description": "Update contact",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
