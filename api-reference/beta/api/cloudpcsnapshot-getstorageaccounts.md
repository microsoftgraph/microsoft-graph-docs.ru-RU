---
title: 'cloudPCSnapshot: getStorageAccounts'
description: Список всех учетных записей хранения, которые можно использовать для хранения моментальных снимков облачного компьютера для проведения экспертного анализа.
author: xhan2077
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 7cfd272b64b07f462d57ccf0d3470454605c40eb
ms.sourcegitcommit: 3a8f6a77dd01a50adf543aaedbf6ec5a202abf93
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/12/2022
ms.locfileid: "65366343"
---
# <a name="get-cloudpcforensicstorageaccount"></a>Получение cloudPcForensicStorageAccount
Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Список всех учетных записей хранения [cloudPcForensicStorageAccount](../resources/cloudpcforensicstorageaccount.md) , которые можно использовать для хранения моментальных снимков или моментальных снимков облачного компьютера для проведения экспертного анализа.

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
GET /deviceManagement/virtualEndpoint/snapshots/getStorageAccounts(subscriptionId='{subscriptionId}')
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения `200 OK` этот метод возвращает код отклика и ноль или более объектов [cloudPcForensicStorageAccount](../resources/cloudpcsnapshot.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "get_cloudpcforensicstorageaccount"
}
-->
``` http
GET /deviceManagement/virtualEndpoint/snapshots/getStorageAccounts(subscriptionId='cb6ad4c4-8a17-4245-a644-e4436b1ee204')
```

### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcForensicStorageAccount"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context":"https://graph.microsoft.com/beta/$metadata#cloudPcForensicStorageAccounts",
    "value":[
        {
            "storageAccountId": "/subscriptions/{subscription-id}/resourceGroups/res2627/providers/Microsoft.Storage/storageAccounts/sto1125",
            "storageAccountName":"sto1125"
        },
        {
            "storageAccountId": "/subscriptions/{subscription-id}/resourceGroups/res9407/providers/Microsoft.Storage/storageAccounts/sto8596",
            "storageAccountName":"sto8596"
        }
    ]
}
```

