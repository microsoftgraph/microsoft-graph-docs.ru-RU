---
title: Список credentialUserRegistrationDetails
description: Получите список объектов credentialUserRegistrationDetails для данного клиента.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: bf6e99722c44ff0054869056be09314d6befac59
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136670"
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

Эта функция поддерживает необязательный параметр запроса OData **$filter.** Вы можете **применить $filter** к одному или более из следующих свойств ресурса [credentialUserRegistrationDetails.](../resources/credentialuserregistrationdetails.md)

| Свойства | Описание и пример |
| --------- | ----------------------- |
| userDisplayName | Фильтрация по имени пользователя. Пример: `/reports/credentialUserRegistrationDetails?$filter=userDisplayName eq 'Contoso'`. Поддерживаемые операторы фильтра: `eq` и `startswith()` . Поддерживается безчувствительности к делу. |
| userPrincipalName | Фильтрация по имени основного пользователя. Пример: `/reports/credentialUserRegistrationDetails?$filter=userPrincipalName eq 'Contoso'`. Поддерживаемые операторы фильтра: `eq` и `startswith()` . Поддерживается безчувствительности к делу. |
| authMethods | Фильтрация по методам проверки подлинности, используемым во время регистрации. Пример: `/reports/credentialUserRegistrationDetails?$filter=authMethods/any(t:t eq microsoft.graph.registrationAuthMethod'email')`. Поддерживаемые операторы фильтра: `eq` . |
| isRegistered | Фильтрация для пользователей, которые зарегистрировались для самостоятельного сброса пароля (SSPR). Пример: `/reports/credentialUserRegistrationDetails?$filter=isRegistered eq true`. Поддерживаемые операторы фильтра: `eq` . |
| isEnabled | Фильтрация для пользователей, для которых включена SSPR. Пример: `/reports/credentialUserRegistrationDetails?$filter=isEnabled eq true`. Поддерживаемые операторы filtter: `eq` . |
| isCapable | Фильтрация для пользователей, которые готовы выполнить сброс пароля или многофакторную проверку подлинности (MFA). Пример: `/reports/credentialUserRegistrationDetails?$filter=isCapable eq true`. Поддерживаемые операторы фильтров: `eq` |
| isMfaRegistered | Фильтрация для пользователей, зарегистрированных на MFA. Пример: `/reports/credentialUserRegistrationDetails?$filter=isMfaRegistered eq true`. Поддерживаемые операторы фильтра: `eq` . |

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Bearer {token} |
| Content-Type | application/json |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) в тексте отклика.

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

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости. Все свойства возвращаются при фактическом вызове.

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


