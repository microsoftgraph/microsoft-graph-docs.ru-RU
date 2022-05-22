---
title: 'managedDevice: bulkSetCloudPcReviewStatus'
description: Задайте состояние проверки нескольких облачных компьютеров с одним запросом, который включает идентификаторы Intune управляемых устройств.
author: yayang3
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: bd1d5d27581f1752ef0d2064810514d98be53420
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629524"
---
# <a name="manageddevice-bulksetcloudpcreviewstatus"></a>managedDevice: bulkSetCloudPcReviewStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Задайте состояние проверки нескольких облачных компьютеров с одним запросом, который включает идентификаторы Intune управляемых устройств.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|CloudPC.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|CloudPC.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/bulkSetCloudPcReviewStatus
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление параметров в формате JSON.

В следующей таблице указаны параметры, которые можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|managedDeviceIds|Коллекция строк|Идентификаторы управляемых устройств облачных компьютеров.|
|reviewStatus|[cloudPcReviewStatus](../resources/cloudpcreviewstatus.md)|Новое состояние проверки для устройств с облачными компьютерами. |


## <a name="response"></a>Отклик

В случае успешного выполнения это действие возвращает код `200 OK` отклика и объект [cloudPcBulkRemoteActionResult](../resources/cloudpcbulkremoteactionresult.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "manageddevicethis.bulksetcloudpcreviewstatus"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/bulkSetCloudPcReviewStatus
Content-Type: application/json

{
  "managedDeviceIds": [
    "30d0e128-de93-41dc-89ec-33d84bb662a0",
    "7c82a3e3-9459-44e4-94d9-b92f93bf78dd"
  ],
  "reviewStatus": {
    "inReview": true,
    "userAccessLevel": "restricted",
    "azureStorageAccountId": "/subscriptions/f68bd846-16ad-4b51-a7c6-c84944a3367c/resourceGroups/Review/providers/Microsoft.Storage/storageAccounts/snapshotsUnderReview"
  }
}
```


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.cloudPcBulkRemoteActionResult",
  "name": "manageddevicethis.bulksetcloudpcreviewstatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "microsoft.graph.cloudPcBulkRemoteActionResult",
  "successfulDeviceIds": [
    "30d0e128-de93-41dc-89ec-33d84bb662a0"
  ],
  "failedDeviceIds": [
    "7c82a3e3-9459-44e4-94d9-b92f93bf78dd"
  ],
  "notFoundDeviceIds": [],
  "notSupportedDeviceIds": []
}
```

