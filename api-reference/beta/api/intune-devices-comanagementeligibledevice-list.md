---
title: Список Команажементелигибледевицес
description: Список свойств и связей объектов Команажементелигибледевице.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2aba5e3294162a6584a0f7b2f133f9fa78f6e80a
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792529"
---
# <a name="list-comanagementeligibledevices"></a>Список Команажементелигибледевицес

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей объектов [команажементелигибледевице](../resources/intune-devices-comanagementeligibledevice.md) .

## <a name="prerequisites"></a>Необходимые компоненты
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/comanagementEligibleDevices
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Тело запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [команажементелигибледевице](../resources/intune-devices-comanagementeligibledevice.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/comanagementEligibleDevices
```

### <a name="response"></a>Отклик
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 880

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
      "id": "ac20683b-683b-ac20-3b68-20ac3b6820ac",
      "deviceName": "Device Name value",
      "deviceType": "windowsRT",
      "clientRegistrationStatus": "registered",
      "ownerType": "company",
      "managementAgents": "mdm",
      "managementState": "retirePending",
      "referenceId": "Reference Id value",
      "mdmStatus": "Mdm Status value",
      "osVersion": "Os Version value",
      "serialNumber": "Serial Number value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "osDescription": "Os Description value",
      "entitySource": 12,
      "userId": "User Id value",
      "upn": "Upn value",
      "userEmail": "User Email value",
      "userName": "User Name value",
      "status": "eligible"
    }
  ]
}
```



