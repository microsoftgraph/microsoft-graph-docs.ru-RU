---
title: Список servicePlans
description: Список планов служб, поддерживаемых облачными КОМПЬЮТЕРами для клиента.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 685148ac79e52ca5c0508ca8ff9edfa673fdbdf8
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696267"
---
# <a name="list-serviceplans"></a>Список servicePlans

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Список планов служб, поддерживаемых облачными КОМПЬЮТЕРами для клиента.

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|CloudPC.Read.All, CloudPC.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Application|CloudPC.Read.All, CloudPC.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/servicePlans
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов

Этот метод не поддерживает параметры запроса OData для настройки ответа. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание               |
| :------------ | :------------------------ |
| Авторизация | Bearer {token}. Обязательный. |

## <a name="request-body"></a>Текст запроса

Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [cloudPcServicePlan](../resources/cloudpcserviceplan.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_servicePlans"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/servicePlans
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-serviceplans-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-serviceplans-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-serviceplans-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-serviceplans-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcServicePlan",
  "isCollection": true
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.cloudPcServicePlan",
      "id": "dea1edd3-edd3-dea1-d3ed-a1ded3eda1de",
      "displayName": "Cloud PC - Level 1 - 1vCPU/2GB",
      "type": "enterprise",
      "vCpuCount": 1,
      "ramInGB": 2,
      "storageInGB": 64,
      "userProfileInGB": 25
    }
  ]
}
```
