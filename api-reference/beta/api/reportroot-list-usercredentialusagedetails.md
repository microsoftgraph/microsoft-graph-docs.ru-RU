---
title: Список пользователейCredentialUsageDetails
description: Получите список объектов userCredentialUsageDetails для данного клиента.
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 3b2efb78529fe0a066ce17f1306574f5ff5f7691
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61011073"
---
# <a name="list-usercredentialusagedetails"></a>Список пользователейCredentialUsageDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список [объектов userCredentialUsageDetails](../resources/usercredentialusagedetails.md) для данного клиента. Сведения включают сведения о пользователях, состояние сброса и причину сбоя.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | Reports.Read.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Reports.Read.All |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
GET /reports/userCredentialUsageDetails
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Эта функция поддерживает необязательный параметр запроса **OData $filter.** Вы можете **$filter** одно или несколько следующих свойств ресурса [userCredentialUsageDetails.](../resources/usercredentialusagedetails.md)

| Свойства | Описание и пример |
|:--------- |:----------- |
| функция | Фильтрация по типу нужных данных об использовании (регистрация против сброса). Пример: `/reports/userCredentialUsageDetails?$filter=feature eq 'registration'`. Поддерживаемые операторы фильтров: `eq` |
| userDisplayName | Фильтр по имени отображения пользователя. Пример: `/reports/userCredentialUsageDetails?$filter=userDisplayName eq 'Contoso'`. Поддерживаемые операторы `eq` фильтров: и `startswith()` . Поддерживает нечувствительный случай. |
| userPrincipalName  | Фильтр по основному имени пользователя. Пример: `/reports/userCredentialUsageDetails?$filter=userPrincipalName eq 'Contoso'`.    Поддерживаемые операторы `eq` фильтров: и `startswith()` . Поддерживает нечувствительный случай. |
| isSuccess | Фильтр по статусу действия. Пример: `/reports/userCredentialUsageDetails?$filter=isSuccess eq true`. Поддерживаемые операторы `eq` фильтров: и `orderby` . |
| authMethod  | Фильтрация с помощью методов проверки подлинности, используемых во время регистрации. Пример: `/reports/userCredentialUsageDetails?$filter=authMethod eq microsoft.graph.usageAuthMethod'email'`. Поддерживаемые операторы фильтров: `eq` . |
| failureReason | Фильтр по причине сбоя (если действие не удалось). Пример: `/reports/userCredentialUsageDetails?$filter=failureReason eq 'Contoso'`. Поддерживаемые операторы `eq` фильтров: и `startswith()` . Поддерживает нечувствительный случай. |


## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Authorization | Bearer {token} |
| Content-Type | application/json |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код ответа и коллекцию объектов `200 OK` [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) в теле ответа.

## <a name="examples"></a>Примеры

В приведенном ниже примере показано, как вызывать этот API.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-usercredentialusagedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-usercredentialusagedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-usercredentialusagedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-usercredentialusagedetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-usercredentialusagedetails-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. Все свойства возвращаются с фактического вызова.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.getUserCredentialUsageDetails)",
  "value":[
    {
      "id" : "id-value",
      "feature":"registration",
      "userPrincipalName":"userPrincipalName-value",
      "userDisplayName": "userDisplayName-value",
      "isSuccess" : true,
      "authMethod": "email",
      "failureReason": "User contacted an admin after trying the email verification option",
      "eventDateTime" : "2019-04-01T00:00:00Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List userCredentialUsageDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


