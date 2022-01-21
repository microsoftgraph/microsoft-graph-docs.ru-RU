---
title: Список credentialUserRegistrationDetails
description: Получите список объектов credentialUserRegistrationDetails для данного клиента.
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: cc884ccf95eae43d71d636acffb41389428e0b8b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115940"
---
# <a name="list-credentialuserregistrationdetails"></a>Список credentialUserRegistrationDetails

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите список объектов [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) для данного клиента.

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
GET /reports/credentialUserRegistrationDetails
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Эта функция поддерживает необязательный параметр запроса **OData $filter.** Вы можете **$filter** одно или несколько следующих свойств ресурса [credentialUserRegistrationDetails.](../resources/credentialuserregistrationdetails.md)

| Свойства | Описание и пример |
| --------- | ----------------------- |
| userDisplayName | Фильтр по имени пользователя. Пример: `/reports/credentialUserRegistrationDetails?$filter=userDisplayName eq 'Contoso'`. Поддерживаемые операторы фильтров: `eq` и `startswith()` . Поддерживает нечувствительный случай. |
| userPrincipalName | Фильтр по основному имени пользователя. Пример: `/reports/credentialUserRegistrationDetails?$filter=userPrincipalName eq 'Contoso'`. Поддерживаемые операторы `eq` фильтров: и `startswith()` . Поддерживает нечувствительный случай. |
| authMethods | Фильтрация с помощью методов проверки подлинности, используемых во время регистрации. Пример: `/reports/credentialUserRegistrationDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`. Поддерживаемые операторы фильтров: `eq` . |
| isRegistered | Фильтр для пользователей, которые зарегистрировались для сброса пароля самообслуживанной службы (SSPR). Пример: `/reports/credentialUserRegistrationDetails?$filter=isRegistered eq true`. Поддерживаемые операторы фильтров: `eq` . |
| isEnabled | Фильтр для пользователей, включенных для SSPR. Пример: `/reports/credentialUserRegistrationDetails?$filter=isEnabled eq true`. Поддерживаемые операторы filtter: `eq` . |
| isCapable | Фильтр для пользователей, готовых выполнить сброс пароля или многофакторную проверку подлинности (MFA). Пример: `/reports/credentialUserRegistrationDetails?$filter=isCapable eq true`. Поддерживаемые операторы фильтров: `eq` |
| isMfaRegistered | Фильтр для пользователей, зарегистрированных в МИД. Пример: `/reports/credentialUserRegistrationDetails?$filter=isMfaRegistered eq true`. Поддерживаемые операторы фильтров: `eq` . |

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Bearer {token} |
| Content-Type | application/json |

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) в тексте ответа.

## <a name="examples"></a>Примеры

В приведенном ниже примере показано, как вызывать этот API.

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-credentialuserregistrationdetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-credentialuserregistrationdetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-credentialuserregistrationdetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-credentialuserregistrationdetails-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-credentialuserregistrationdetails-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-credentialuserregistrationdetails-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. Все свойства возвращаются с фактического вызова.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.credentialUserRegistrationDetails",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/reports/$metadata#Collection(microsoft.graph.credentialUserRegistrationDetails)",
  "value":[
    {
      "id" : "id-value",
      "userPrincipalName":"userPrincipalName",
      "userDisplayName": "userDisplayName-value",
      "authMethods": ["email", "mobileSMS"],
      "isRegistered" : false,
      "isEnabled" : true,
      "isCapable" : false,
      "isMfaRegistered" : true
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List credentialUserRegistrationDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


