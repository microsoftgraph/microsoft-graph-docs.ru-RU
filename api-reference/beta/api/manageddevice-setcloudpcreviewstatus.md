---
title: 'managedDevice: setCloudPcReviewStatus'
description: Задайте состояние проверки для определенного облачного устройства.
author: yayang3
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 3b894035944f2a2962d9b28ceb7e72012ccd5ac7
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629518"
---
# <a name="manageddevice-setcloudpcreviewstatus"></a>managedDevice: setCloudPcReviewStatus

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Задайте состояние проверки для определенного облачного устройства. Используйте этот API, чтобы задать состояние проверки облачного компьютера для проверки, если вы рассматриваете облачный компьютер как подозрительный. После завершения проверки снова используйте этот API, чтобы вернуть облачный компьютер в нормальное состояние.

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
POST /deviceManagement/managedDevices/{managedDeviceId}/setCloudPcReviewStatus
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление параметров в формате JSON.

В следующей таблице показан параметр, который можно использовать с этим действием.

|Параметр|Тип|Описание|
|:---|:---|:---|
|reviewStatus|[cloudPcReviewStatus](../resources/cloudpcreviewstatus.md)|Новое состояние проверки облачного компьютера.|


## <a name="response"></a>Ответ

В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

<!-- {
  "blockType": "request",
  "name": "manageddevicethis.setcloudpcreviewstatus"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/185f01c2de954929afb129392e5d9f47/setCloudPcReviewStatus
Content-Type: application/json

{
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
  "truncated": true,
  "name": "manageddevicethis.setcloudpcreviewstatus"
}
-->
``` http
HTTP/1.1 204 No Content
```

