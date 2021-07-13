---
title: Get cloudPcDevice
description: Ознакомьтесь с свойствами и отношениями объекта cloudPcDevice.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 26d9b438bf366a0a3b4b367bc96ea74441d5324d
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402496"
---
# <a name="get-cloudpcdevice"></a>Get cloudPcDevice
Пространство имен: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ознакомьтесь с свойствами и отношениями объекта [cloudPcDevice.](../resources/managedtenants-cloudpcdevice.md)

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|CloudPC.Read.All, CloudPC.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/cloudPcDevices/{cloudPcDeviceId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {токен}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект cloudPcDevice](../resources/managedtenants-cloudpcdevice.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "get_cloudpcdevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/cloudPcDevices/{cloudPcDeviceId}
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.cloudPcDevice"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.managedTenants.cloudPcDevice",
    "id": "1307ab1b-63ee-4942-bdef-bcd4f415c635",
    "lastUpdated": "2021-07-10T23:05:03.2564744Z",
    "policyId": "",
    "displayName": "device01",
    "managedDeviceId": "",
    "managedDeviceName": "",
    "userPrincipalName": "sally@lucernepublishing001.onmicrosoft.com",
    "servicePlanName": "CloudPC_Standard",
    "status": "NotProvisioned",
    "tenantId": "aa060093-1e81-45b4-bebc-652713194ef7",
    "tenantDisplayName": "Lucerne Publishing",
    "lastRefreshedDateTime": "2021-07-10T23:05:03.2564744Z",
    "provisioningPolicyId": "",
    "cloudPcStatus": "NotProvisioned"
}
```
