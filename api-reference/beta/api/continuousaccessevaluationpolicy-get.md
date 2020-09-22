---
title: Получение Континуаусакцессевалуатионполици
description: Чтение свойств объекта Континуаусакцессевалуатионполици.
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bea54ea801ee9d41314f1fbd2c87070ac4e92773
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023541"
---
# <a name="get-continuousaccessevaluationpolicy"></a>Получение Континуаусакцессевалуатионполици
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Чтение свойств и связей объекта [континуаусакцессевалуатионполици](../resources/continuousaccessevaluationpolicy.md) .

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)     | Policy.Read.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Для приложений                            | Policy.Read.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {  "blockType": "ignored"} -->
``` http
GET /identity/continuousAccessEvaluationPolicy
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметр запроса OData "$select" для настройки ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [континуаусакцессевалуатионполици](../resources/continuousaccessevaluationpolicy.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "get_continuousaccessevaluationpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/continuousAccessEvaluationPolicy
```


### <a name="response"></a>Отклик

Ниже приведен пример ответа.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.continuousAccessEvaluationPolicy"
} -->

``` http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/continuousAccessEvaluationPolicy/$entity",
  "id": "00000000-0000-0000-0000-000000000006",
  "description": "Continuous Access Evaluation automatically blocks access to resources and applications in near real time when a user's access is removed or a client IP address changes.",
  "displayName": "Continuous Access Evaluation",
  "isEnabled": true,
  "users": [ "1608be63-df14-42a4-8932-1c9d963b026f" ],
  "groups": [ "4308b567-df14-0000-8932-1c9d963b026f" ]
}
```
