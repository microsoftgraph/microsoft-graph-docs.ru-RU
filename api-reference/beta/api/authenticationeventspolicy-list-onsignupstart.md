---
title: Список слушателей onSignUpStart
description: Получите коллекцию ресурсов authenticationListener, поддерживаемую событием onSignupStart.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1cdf120afeb553124e18488cb0cde20b6de23056
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438556"
---
# <a name="list-onsignupstart-listeners"></a>Список слушателей onSignUpStart

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получите коллекцию ресурсов authenticationListener, поддерживаемую событием onSignupStart. Событие onSignUpStart поддерживает [тип invokeUserFlowListener.](../resources/invokeuserflowlistener.md)

При присвоении [invokeUserFlowListener](../resources/invokeuserflowlistener.md) событию onSignUpStart приложение связано с потоком пользователей, [](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) что позволяет самообслуживке зарегистрироваться на нем. После создания события проверки подлинности для обращения к потоку пользователей пользователи, которые идут в это приложение, смогут инициировать поток регистрации, который содержит учетную запись гостей.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|Policy.Read.All, Policy.ReadWrite.ApplicationConfiguration|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/events/onSignupStart
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод поддерживает параметр запроса OData для расширения сведений `$expand` об invokeUserFlowListener. Ниже приведен пример. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Тело запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [authenticationListener](../resources/authenticationlistener.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="example-1-list-authenticationlisteners-for-the-onsignupstart-event"></a>Пример 1. Список аутентификацииListeners для события onSignUpStart

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "list_authenticationlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.authenticationListener)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart",
  "value": [
    {
      "@odata.type": "#microsoft.graph.invokeUserFlowListener",
      "id": "2adb5c12-5c12-2adb-125c-db2a125cdb2a",
      "priority": 101,
      "sourceFilter": {
        "includeApplications": [
            "3dfff01b-0afb-4a07-967f-d1ccbd81102a"
        ]
      }
    },
    {
      "@odata.type": "#Microsoft.Graph.InvokeUserFlowListener",
      "id": "0a09997f-fa0c-4f3c-9d02-76762ac069c8",
      "priority": 100,
      "sourceFilter": {
          "includeApplications": [
              "b0e1638f-4c39-4cd1-82b3-91d1caef65f8"
        ]
      }
    }
  ]
}
```

### <a name="example-2-expand-invokeuserflowlisteners-in-authenticationlisteners-for-the-onsignupstart-event"></a>Пример 2. Расширение invokeUserFlowListeners в проверке подлинностиListeners для события onSignUpStart

В следующем примере перечислены слушатели, определенные для события onSignupStart, и для каждого слушателя расширяется поток пользователей, который вызывается.

#### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "list_authenticationlistener_invokeuserflowlistener"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/events/onSignupStart?$expand=microsoft.graph.invokeUserFlowListener/userFlow
```

#### <a name="response"></a>Отклик

Ниже приведен пример отклика.

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.invokeUserFlowListener)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/events/onSignUpStart(microsoft.graph.invokeUserFlowListener/userFlow())/$entity",
  "value": [
    {
      "@odata.type": "#microsoft.graph.invokeUserFlowListener",
      "id": "2adb5c12-5c12-2adb-125c-db2a125cdb2a",
      "priority": 101,
      "sourceFilter": {
        "includeApplications": [
            "3dfff01b-0afb-4a07-967f-d1ccbd81102a"
        ]
      },
      "userFlow": {
            "id": "B2X_1_Partner",
            "userFlowType": "signUpOrSignIn",
            "userFlowTypeVersion": 1
      }
    },
    {
      "@odata.type": "#microsoft.graph.InvokeUserFlowListener",
      "id": "0a09997f-fa0c-4f3c-9d02-76762ac069c8",
      "priority": 100,
      "sourceFilter": {
        "includeApplications": [
            "b0e1638f-4c39-4cd1-82b3-91d1caef65f8"
        ]
      },
      "userFlow": {
            "id": "B2X_1_Partner",
            "userFlowType": "signUpOrSignIn",
            "userFlowTypeVersion": 1
      }
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "List onSignUpStart",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: list_authenticationlistener_invokeuserflowlistener/container/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'",
    "Error: list_authenticationlistener_invokeuserflowlistener/container/userFlow/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
