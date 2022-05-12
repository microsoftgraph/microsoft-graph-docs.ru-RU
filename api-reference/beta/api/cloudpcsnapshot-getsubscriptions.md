---
title: 'cloudPCSnapshot: getSubscriptions'
description: Список всех подписок, которые можно использовать для хранения моментальных снимков или моментальных снимков облачного компьютера для проведения экспертного анализа.
author: xhan2077
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 0ac94f330d8d398a4e203644844aa894d101ee7a
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/12/2022
ms.locfileid: "65366340"
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
|Для приложений|CloudPC.Read.All, CloudPC.ReadWrite.All|

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

<!-- {
  "blockType": "request",
  "name": "get_cloudpcsubscription"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/snapshots/getSubscriptions
```

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

