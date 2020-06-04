---
title: Обновление Аусентикатионфловсполици
description: Обновление логического свойства Селфсервицесигнуп объекта Аусентикатионфловсполици.
author: linkhp
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 626e1dc8a851f2c8da6a9bb815a4e783cf44e7d2
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2020
ms.locfileid: "44556432"
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

## <a name="request-body"></a>Текст запроса
В тексте запроса вы можете предоставить представление объекта [аусентикатионфловсполици](../resources/authenticationflowspolicy.md) в формате JSON (необязательно).

В следующей таблице приведены свойства, необходимые при обновлении [аусентикатионфловсполици](../resources/authenticationflowspolicy.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|селфсервицесигнуп|[селфсервицесигнупаусентикатионфловконфигуратион](../resources/selfservicesignupauthenticationflowconfiguration.md)|Самостоятельная настройка регистрации.|

## <a name="response"></a>Отклик

При успешном выполнении этот метод возвращает код отклика `204 No Content` и пустое тело отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
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

### <a name="response"></a>Отклик
<!-- {
  "blockType": "response",
  "truncated": true
} -->
``` http
HTTP/1.1 204 No Content
```
