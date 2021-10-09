---
title: 'directoryObject: getMemberGroups'
description: Верни все группы, в которые входит указанный пользователь, группа, руководитель службы или объект каталога. Это транзитивная функция.
ms.localizationpriority: medium
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 28b72a5df66e6708906fc83016bfb186519499a3
ms.sourcegitcommit: 11be55b40804b07f4c422f09f601afa97c7d31ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2021
ms.locfileid: "60256321"
---
# <a name="directoryobject-getmembergroups"></a>directoryObject: getMemberGroups

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Верни все группы, в которые входит указанный пользователь, группа, руководитель службы или объект каталога. Это транзитивная функция.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | User.ReadBasic.All и GroupMember.Read.All, User.Read.All и GroupMember.Read.All, User.ReadBasic.All и Group.Read.All, User.Read.All и Group.Read.All, Directory.Read.All    |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Приложение | User.Read.All и GroupMember.Read.All, User.Read.All и Group.Read.All, Directory.Read.All |

В следующей таблице перечислены типы разрешений, которые можно использовать для различных сценариев.

| Сценарий | Разрешения |
|:-|:-|
| Для получения членства в группе для пользователя, вписаного в группу | Используйте один из следующих наборов разрешений: <br/> <li> **User.Read** и **GroupMember.Read.All** <li>**User.Read** и **Group.Read.All** |
| Для получения членства в группе для любого пользователя | Используйте один из следующих наборов разрешений: <br/> <li> **User.ReadBasic.All** и **GroupMember.Read.All** <li>**User.Read.All** и **GroupMember.Read.All** <li>**User.ReadBasic.All** и **Group.Read.All** <li>**User.Read.All** и **Group.Read.All** |
| Чтобы получить членство в группе для группы | Используйте разрешение **GroupMember.Read.All** или **Group.Read.All.** |
| Чтобы получить членство в группе для директора службы | Используйте один из следующих наборов разрешений <br/> <li>**Application.ReadWrite.All** и **GroupMember.Read.All** <li>**Application.ReadWrite.All** и **Group.Read.All** |
| Чтобы получить членство в группе для объекта каталога | Используйте **разрешение Directory.Read.All.** |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /servicePrincipals/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a>Заголовки запросов
| Имя       | Описание|
|:---------------|:--------|
| Авторизация  | Bearer {token}. Обязательный. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса
В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.

| Параметр    | Тип   |Описание|
|:---------------|:--------|:----------|
|securityEnabledOnly|Boolean| `true` чтобы указать, что должны возвращаться только группы безопасности, в которые входит объект; чтобы указать, что все роли групп и каталогов, в которые входит объект, `false` должны быть возвращены. **Примечание.** Функция может быть вызвана пользователю только в том случае, если параметр `true` . |

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и объект коллекции String в тексте отклика.

## <a name="example"></a>Пример

##### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmembergroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmembergroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmembergroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmembergroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


