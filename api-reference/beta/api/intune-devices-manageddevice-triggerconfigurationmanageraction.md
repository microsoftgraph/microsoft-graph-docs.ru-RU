---
title: действие Тригжерконфигуратионманажерактион
description: Действие триггера в клиенте Конфигуратионманажер
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d37d4d5d58cbec3a3ec14547f6f540227c29d585
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49234792"
---
# <a name="triggerconfigurationmanageraction-action"></a>действие Тригжерконфигуратионманажерактион

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Действие триггера в клиенте Конфигуратионманажер

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementManagedDevices.PriviligedOperation.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementManagedDevices.PriviligedOperation.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction
POST /deviceManagement/comanagedDevices/{managedDeviceId}/triggerConfigurationManagerAction
POST /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}/managedDevice/triggerConfigurationManagerAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/triggerConfigurationManagerAction
POST /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}/deviceRunStates/{deviceComplianceScriptDeviceStateId}/managedDevice/triggerConfigurationManagerAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction
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
|configurationManagerAction|[configurationManagerAction](../resources/intune-devices-configurationmanageraction.md)|Пока не задокументировано.|



## <a name="response"></a>Ответ
В случае успешного выполнения это действие возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/triggerConfigurationManagerAction

Content-type: application/json
Content-length: 145

{
  "configurationManagerAction": {
    "@odata.type": "microsoft.graph.configurationManagerAction",
    "action": "refreshUserPolicy"
  }
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 204 No Content
```




