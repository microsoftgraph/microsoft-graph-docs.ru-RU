---
title: Действие triggerDeviceScopeAction
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 535ba2e4aeaf404d10b20612806452c07b8b1eff
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858873"
---
# <a name="triggerdevicescopeaction-action"></a>Действие triggerDeviceScopeAction

Пространство имен: microsoft.graph

> **Важно:** API Graph Майкрософт в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пока не задокументировано.

## <a name="prerequisites"></a>Предварительные условия
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированное (рабочая или учебная учетная запись)|DeviceManagementConfiguration.Read.All, DeviceManagementManagedDevices.Read.All|
|Делегированное (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.Read.All, DeviceManagementManagedDevices.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsDeviceScope/triggerDeviceScopeAction
POST /deviceManagement/userExperienceAnalyticsDeviceScopes/{userExperienceAnalyticsDeviceScopeId}/triggerDeviceScopeAction
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тело запроса добавьте параметры в формате JSON.

В приведенной ниже таблице указаны параметры, которые можно использовать с этим действием.

|Свойство|Тип|Описание|
|:---|:---|:---|
|actionName|[deviceScopeAction](../resources/intune-devices-devicescopeaction.md)|Пока не задокументировано.|
|deviceScopeId|String|Пока не задокументировано.|



## <a name="response"></a>Ответ
В случае успешного выполнения это действие возвращает код `200 OK` отклика и [deviceScopeActionResult](../resources/intune-devices-devicescopeactionresult.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceScope/triggerDeviceScopeAction

Content-type: application/json
Content-length: 69

{
  "actionName": "",
  "deviceScopeId": "Device Scope Id value"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 236

{
  "value": {
    "@odata.type": "microsoft.graph.deviceScopeActionResult",
    "deviceScopeAction": "String",
    "deviceScopeId": "Device Scope Id value",
    "status": "succeeded",
    "failedMessage": "Failed Message value"
  }
}
```




