---
title: действие getDevicesScheduledToRetire
description: Пока не задокументировано.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cfab154e970f6d03ecfa37e528ec88544eb24fa3
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59103237"
---
# <a name="getdevicesscheduledtoretire-action"></a>действие getDevicesScheduledToRetire

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.

## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/getDevicesScheduledToRetire
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешного действия возвращается код ответа и коллекция `200 OK` [retireScheduledManagedDevice](../resources/intune-deviceconfig-retirescheduledmanageddevice.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/getDevicesScheduledToRetire
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 670

{
  "value": [
    {
      "@odata.type": "microsoft.graph.retireScheduledManagedDevice",
      "id": "Id value",
      "managedDeviceId": "Managed Device Id value",
      "managedDeviceName": "Managed Device Name value",
      "deviceType": "windowsRT",
      "complianceState": "notApplicable",
      "retireAfterDateTime": "2016-12-31T23:57:37.576134-08:00",
      "managementAgent": "mdm",
      "ownerType": "company",
      "deviceCompliancePolicyName": "Device Compliance Policy Name value",
      "deviceCompliancePolicyId": "Device Compliance Policy Id value",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```



