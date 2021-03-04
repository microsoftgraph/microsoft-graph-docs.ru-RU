---
title: Put authenticationListener
description: Замените объект authenticationListener.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 6e41dde2a8c22394fd28fe3730ac44655c7eb310
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438451"
---
# <a name="put-authenticationlistener"></a>Put authenticationListener

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Замените [проверку подлинностиListener,](../resources/authenticationlistener.md) определяемую для события onSignupStart в конвейере проверки подлинности.

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
PUT /identity/events/onSignupStart/{id}
```

## <a name="request-headers"></a>Заголовки запросов

|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса

В теле запроса поставляем представление JSON объекта [authenticationListener.](../resources/authenticationlistener.md)

В следующей таблице показаны свойства, необходимые при создании [invokeUserFlowListener.](../resources/invokeuserflowlistener.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|priority|Int32|Приоритет слушателя. Определяет порядок оценки, когда в событии имеется несколько слушателей. Приоритет оценивается от низкого до высокого.|
|sourceFilter|[authenticationSourceFilter](../resources/authenticationsourcefilter.md)|Фильтр на основе источника проверки подлинности, который используется для определения оценки прослушиваемого. В настоящее время это ограничивается оценками на основе приложения, в которое пользователь проходит проверку подлинности.|
|userFlow|[b2xIdentityUserFlow](../resources/b2xidentityuserflow.md)|Ссылка на объект потока пользователя, вызываемого в этом действии.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "put_authenticationlistener_from_"
}
-->

``` http
PUT https://graph.microsoft.com/beta/identity/events/onSignupStart/{id}
Content-Type: application/json

{
    "@odata.type": "#Microsoft.Graph.InvokeUserFlowListener",
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

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
