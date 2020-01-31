---
title: Список Команажементелигибледевицеентити
description: Список свойств и связей объектов Команажементелигибледевицеентити.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 39d7a92c5914107cdd5ecfebb9b4b7948bc8b8b0
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636317"
---
# <a name="list-comanagementeligibledeviceentity"></a>Список Команажементелигибледевицеентити

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Список свойств и связей объектов Команажементелигибледевицеентити.

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/comanagementEligibleReports
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Ответ
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов команажементелигибледевицеентити в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/comanagementEligibleReports
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1303

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.comanagementEligibleDeviceEntity",
      "id": "659554f2-54f2-6595-f254-9565f2549565",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "deviceType": "Device Type value",
      "clientRegistrationStatus": "Client Registration Status value",
      "ownerType": "Owner Type value",
      "managementAgents": "Management Agent value",
      "managementState": "Management State value",
      "referenceId": "Reference Id value",
      "mdmStatus": "MDM Status value",
      "osVersion": "OS Version value",
      "serialNumber": "Serial Number value",
      "manufacturer": "Manufacture value",
      "model": "Model value",
      "osDescription": "OS Description value",
      "entitySource": 1024,
      "userId": "User Id value",
      "upn": "UPN value",
      "userEmail": "User Email value",
      "userName": "User name value",
      "coManageEligibleStatus": "CO Manage Eligible Status value"
    }
  ]
}
```



