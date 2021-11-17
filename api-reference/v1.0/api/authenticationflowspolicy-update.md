---
title: Обновление authenticationFlowsPolicy
description: Обновление логического свойства selfServiceSignUp объекта authenticationFlowsPolicy.
author: linkhp
ms.localizationpriority: high
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 76f31e72cc4f66eb1bb71df580cc120a5b80dd87
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029728"
---
# <a name="update-authenticationflowspolicy"></a>Обновление authenticationFlowsPolicy

Пространство имен: microsoft.graph

Обновление свойства **selfServiceSignUp** объекта [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md). Свойства **идентификатор**, **тип** и **описание** изменить невозможно.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Policy.ReadWrite.AuthenticationFlows|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Для приложений|Policy.ReadWrite.AuthenticationFlows|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В тексте запроса можно указать представление JSON объекта [authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).

Ниже показаны свойства, которые необходимо указывать при обновлении[authenticationFlowsPolicy](../resources/authenticationflowspolicy.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|selfServiceSignUp|[selfServiceSignUpAuthenticationFlowConfiguration](../resources/selfservicesignupauthenticationflowconfiguration.md)|Самостоятельная конфигурация регистрации.|

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_authenticationflowspolicy"
}
-->

```http
PATCH https://graph.microsoft.com/v1.0/policies/authenticationFlowsPolicy
Content-Type: application/json

{
  "selfServiceSignUp": {
    "isEnabled": true
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-authenticationflowspolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-authenticationflowspolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-authenticationflowspolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-authenticationflowspolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Перейти](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-authenticationflowspolicy-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
} -->

``` http
HTTP/1.1 204 No Content
```
