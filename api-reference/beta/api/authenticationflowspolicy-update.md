---
title: Обновление Аусентикатионфловсполици
description: Обновление логического свойства Селфсервицесигнуп объекта Аусентикатионфловсполици.
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 3408cff98cc79dbf819e077ab12fa066f7d723f7
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44680896"
---
# <a name="update-authenticationflowspolicy"></a>Обновление Аусентикатионфловсполици

Пространство имен: microsoft.graph

Обновление логического свойства **селфсервицесигнуп** объекта [аусентикатионфловсполици](../resources/authenticationflowspolicy.md) . **Идентификатор**, **тип**и **Описание** свойства не могут быть изменены.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Policy. ReadWrite. Аусентикатионфловс|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается|
|Для приложений|Policy. ReadWrite. Аусентикатионфловс|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/authenticationFlowsPolicy
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Основной текст запроса
В тексте запроса вы можете предоставить представление объекта [аусентикатионфловсполици](../resources/authenticationflowspolicy.md) в формате JSON (необязательно).

В следующей таблице приведены свойства, необходимые при обновлении [аусентикатионфловсполици](../resources/authenticationflowspolicy.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|селфсервицесигнуп|[селфсервицесигнупаусентикатионфловконфигуратион](../resources/selfservicesignupauthenticationflowconfiguration.md)|Самостоятельная настройка регистрации.|

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
PATCH https://graph.microsoft.com/beta/policies/authenticationFlowsPolicy
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

---


### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
} -->
``` http
HTTP/1.1 204 No Content
```
