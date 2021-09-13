---
title: функция userExperienceAnalyticsSummarizeWorkFromAnywhereDevices
description: Пока не задокументировано.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: eacf83b2871fbc67d6cbdea8cb909d16e6b81bdf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59042363"
---
# <a name="userexperienceanalyticssummarizeworkfromanywheredevices-function"></a>функция userExperienceAnalyticsSummarizeWorkFromAnywhereDevices

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.

## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsSummarizeWorkFromAnywhereDevices
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик
В случае успешной работы эта функция возвращает код ответа и `200 OK` [userExperienceAnalyticsWorkFromAnywhereDevicesSummary](../resources/intune-devices-userexperienceanalyticsworkfromanywheredevicessummary.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsSummarizeWorkFromAnywhereDevices
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 998

{
  "value": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevicesSummary",
    "autopilotDevicesSummary": {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary",
      "devicesNotAutopilotRegistered": 13,
      "devicesWithoutAutopilotProfileAssigned": 6,
      "totalWindows10DevicesWithoutTenantAttached": 10
    },
    "cloudManagementDevicesSummary": {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudManagementDevicesSummary",
      "coManagedDeviceCount": 4,
      "intuneDeviceCount": 1,
      "tenantAttachDeviceCount": 7
    },
    "windows10DevicesSummary": {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsWindows10DevicesSummary",
      "unsupportedOSversionDeviceCount": 15
    },
    "cloudIdentityDevicesSummary": {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsCloudIdentityDevicesSummary",
      "deviceWithoutCloudIdentityCount": 15
    }
  }
}
```



