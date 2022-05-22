---
title: 'cloudPCSnapshot: getSubscriptions'
description: Список всех подписок, которые можно использовать для хранения моментальных снимков или моментальных снимков облачного компьютера для проведения экспертного анализа.
author: xhan2077
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 879f6f6bfd382173958eca84a556571e58ae5f0b
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629302"
---
# <a name="get-cloudpcsubscription"></a>Получение cloudPcSubscription
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Список всех подписок [cloudPcSubscription](../resources/cloudpcsubscription.md) , которые можно использовать для хранения моментальных снимков или моментальных снимков облачного компьютера для проведения экспертного анализа.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|CloudPC.Read.All, CloudPC.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|CloudPC.Read.All, CloudPC.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/virtualEndpoint/snapshots/getSubscriptions
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает `200 OK` код отклика и ноль или несколько объектов [cloudPcSubscription](../resources/cloudpcsnapshot.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcsubscription"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/snapshots/getSubscriptions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcsubscription-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcsubscription-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcsubscription-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcsubscription-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-cloudpcsubscription-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcSubscription"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#cloudPcSubscriptions",
    "value":[
        {
            "subscriptionId": "8fd04a0b-ed49-46c0-a62d-e7980d829058",
            "subscriptionName":"Cloud PC Service INT"
        },
        {
            "subscriptionId": "618f7b25-b146-4c0e-a21b-2f1c67e78648",
            "subscriptionName":"Cloud PC HOBO Test1"
        }
    ]
}
```

