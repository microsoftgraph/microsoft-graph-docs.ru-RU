---
title: Список domainNameReferences
description: Извлечение списка directoryObject со ссылкой на домен.
author: adimitui
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 061139bb6672b9d1f1327122df5c2d86e85f0a88
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224820"
---
# <a name="list-domainnamereferences"></a>Список domainNameReferences

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Извлечение списка [directoryObject](../resources/directoryobject.md) со ссылкой на домен. Возвращенный список будет содержать все объекты каталога, которые имеют зависимость от домена.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).


|Тип разрешения      | Разрешения (в порядке повышения привилегий)              |
|:--------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись) | Domain.Read.All, Domain.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается.    |
|Application | Domain.Read.All, Domain.ReadWrite.All |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

## <a name="optional-query-parameters"></a>Необязательные параметры запроса

Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация  | Bearer {токен}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [directoryObject](../resources/directoryobject.md) в тексте отклика.

## <a name="example"></a>Пример
##### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/domains/contoso.com/domainNameReferences
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domainnamereferences-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domainnamereferences-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domainnamereferences-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domainnamereferences-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-domainnamereferences-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "value": [
    {
      "@odata.type": "#microsoft.graph.user",
      "@odata.id": "https://graph.microsoft.com/v2/927c6607-8060-4f4a-a5f8-34964ac78d70/directoryObjects/fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f/Microsoft.DirectoryServices.User",
      "id": "fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f",
      "accountEnabled": true,
      "city": "Nairobi",
      "createdDateTime": "2021-04-14T05:26:16Z",
      "country": "Kenya",
      "displayName": "Adele Vance",
      "givenName": "Adele",
      "mail": "AdeleV@Contoso.com",
      "mailNickname": "AdeleV"
    },
    {
      "@odata.type": "#microsoft.graph.group",
      "@odata.id": "https://graph.microsoft.com/v2/927c6607-8060-4f4a-a5f8-34964ac78d70/directoryObjects/eac82bd3-931c-4d47-9e68-735595a8eb8a/Microsoft.DirectoryServices.Group",
      "id": "eac82bd3-931c-4d47-9e68-735595a8eb8a",
      "createdDateTime": "2021-04-14T06:59:47Z",
      "createdByAppId": "00000005-0000-0ff1-ce00-000000000000",
      "organizationId": "927c6607-8060-4f4a-a5f8-34964ac78d70",
      "description": "Contribute your ideas and ask your questions to our leadership team. And tune in for regular Employee Q & A live events. You can learn more about what",
      "displayName": "CEO Connection",
      "expirationDateTime": "2021-10-11T06:59:47Z",
      "groupTypes": [
        "Unified"
      ],
      "mail": "ceoconnection@Contoso.com",
      "mailEnabled": true,
      "mailNickname": "ceoconnection",
      "resourceBehaviorOptions": [
        "CalendarMemberReadOnly"
      ],
      "visibility": "Public",
      "writebackConfiguration": {
        "isEnabled": null,
        "onPremisesGroupType": null
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
