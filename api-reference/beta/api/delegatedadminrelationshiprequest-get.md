---
title: Получение delegatedAdminRelationshipRequest
description: Чтение свойств и связей объекта delegatedAdminRelationshipRequest.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: apiPageType
ms.openlocfilehash: bebace0568ee12e12140c04dc9319a00210b68c2
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209166"
---
# <a name="get-delegatedadminrelationshiprequest"></a>Получение delegatedAdminRelationshipRequest
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Чтение свойств и связей объекта [delegatedAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)| DelegatedAdminRelationship.Read.All, DelegatedAdminRelationship.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт)| Не поддерживается. |
|Для приложений| Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/delegatedAdminRelationships/{delegatedAdminRelationshipId}/requests/{delegatedAdminRelationshipRequestId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметр `$select` запроса OData для получения определенных свойств пользователя, включая те, которые не возвращаются по умолчанию.

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и объект [delegatedAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_delegatedadminrelationshiprequest"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/delegatedAdminRelationships/5d027261-d21f-4aa9-b7db-7fa1f56fb163-8777b240-c6f0-4469-9e98-a3205431b836/requests/cf4a23c7-070c-4d1c-8be8-1e86085ac9d1
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-delegatedadminrelationshiprequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-delegatedadminrelationshiprequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-delegatedadminrelationshiprequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-delegatedadminrelationshiprequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-delegatedadminrelationshiprequest-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.delegatedAdminRelationshipRequest"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationshipRequest",
  "@odata.context": "https://graph.microsoft.com/beta/tenantRelationships/$metadata#requests/$entity",
  "@odata.etag": "W/\"JyIxODAwZTY4My0wMDAwLTAyMDAtMDAwMC02MTU0OWFmMDAwMDAiJw==\"",
  "id": "cf4a23c7-070c-4d1c-8be8-1e86085ac9d1",
  "action": "lockForApproval",
  "status": "created",
  "createdDateTime": "2022-02-10T10:55:47.1180588Z",
  "lastModifiedDateTime": "2022-02-10T11:26:44.9941884Z"
}
```

