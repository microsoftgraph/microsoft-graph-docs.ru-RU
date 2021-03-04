---
title: Создание authenticationListener
description: Создайте новый объект authenticationListener для события onSignUpStart.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: c24ceff80c873181799ea38fbe23c6054f876bc7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438535"
---
# <a name="create-authenticationlistener"></a>Создание authenticationListener

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый объект authenticationListener для события onSignUpStart.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Policy.ReadWrite.ApplicationConfiguration|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|Policy.ReadWrite.ApplicationConfiguration|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /identity/events/onSignupStart
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON объекта [authenticationListener.](../resources/authenticationlistener.md)

В следующей таблице показаны свойства, необходимые при создании проверки подлинности [invokeUserFlowListener.](../resources/invokeuserflowlistener.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|priority|Int32|Приоритет слушателя. Определяет порядок оценки, когда в событии имеется несколько слушателей. Приоритет оценивается от низкого до высокого.|
|sourceFilter|[authenticationSourceFilter](../resources/authenticationsourcefilter.md)|Фильтр на основе источника проверки подлинности, который используется для определения оценки прослушиваемого. В настоящее время это ограничивается оценками на основе приложения, в которое пользователь проходит проверку подлинности.|
|userFlow|[b2xIdentityUserFlow](../resources/b2xidentityuserflow.md)|Объект [b2xIdentityUserFlow,](../resources/b2xidentityuserflow.md) который будет вызываться при оценке этого действия.|

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `201 Created` объект [authenticationListener](../resources/authenticationlistener.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "create_authenticationlistener_from_"
}
-->

``` http
POST https://graph.microsoft.com/beta/identity/events/onSignupStart
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.invokeUserFlowListener",
    "priority": 101,
    "sourceFilter": {
        "includeApplications": [
            "1fc41a76-3050-4529-8095-9af8897cf63d"
        ]
    },
    "userFlow": {
        "id": "B2X_1_Partner"
    }
}
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationListener"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/events/onSignupStart/Microsoft.Graph.InvokeUserFlowListener/$entity",
    "@odata.type": "#microsoft.graph.invokeUserFlowListener",
    "id": "2be3336b-e3b4-44f3-9128-b6fd9ad39bb8",
    "priority": 101,
    "sourceFilter": {
        "includeApplications": [
            "1fc41a76-3050-4529-8095-9af8897cf63d"
        ]
    }
}
```
