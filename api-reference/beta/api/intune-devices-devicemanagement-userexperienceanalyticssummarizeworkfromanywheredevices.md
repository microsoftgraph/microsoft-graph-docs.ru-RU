---
title: функция userExperienceAnalyticsSummarizeWorkFromAnywhereDevices
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 316faf91924c985b2798506bc96dfb6c4406fd46
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2021
ms.locfileid: "58261920"
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
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

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
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
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
Content-Length: 941

{
  "value": {
    "@odata.type": "microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevicesSummary",
    "autopilotDevicesSummary": {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsAutopilotDevicesSummary",
      "devicesNotAutopilotRegistered": 13,
      "devicesWithoutAutopilotProfileAssigned": 6
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




