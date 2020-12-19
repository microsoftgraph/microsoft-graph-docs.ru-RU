---
title: Создание authenticationListener
description: Создайте новый объект authenticationListener для события onSignUpStart.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a5d370832032c1f80fbab31ff739706e682732f5
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720304"
---
# <a name="create-authenticationlistener"></a>Создание authenticationListener

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте новый объект authenticationListener для события onSignUpStart.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|Policy.ReadWrite.ApplicationConfiguration|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
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

В теле запроса укажу представление объекта [authenticationListener](../resources/authenticationlistener.md) в JSON.

В следующей таблице показаны свойства, необходимые при создании [объекта invokeUserFlowListener](../resources/invokeuserflowlistener.md) authenticationListener.

|Свойство|Тип|Описание|
|:---|:---|:---|
|priority|Int32|Приоритет прослушиватель. Определяет порядок оценки, если событие имеет несколько прослушивателей. Приоритет оценивается от низкого до высокого.|
|sourceFilter|[authenticationSourceFilter](../resources/authenticationsourcefilter.md)|Фильтрация на основе источника проверки подлинности, используемого для определения того, оценивается ли прослушиватель. В настоящее время это ограничение ограничено оценками, основанными на приложении, в которое пользователь проходит проверку подлинности.|
|userFlow|[b2xIdentityUserFlow](../resources/b2xidentityuserflow.md)|Объект [b2xIdentityUserFlow,](../resources/b2xidentityuserflow.md) который будет вызываться при оценке этого действия.|

## <a name="response"></a>Отклик

В случае успеха этот метод возвращает код отклика и объект `201 Created` [authenticationListener](../resources/authenticationlistener.md) в тексте отклика.

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

Ниже приведен пример ответа.

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
