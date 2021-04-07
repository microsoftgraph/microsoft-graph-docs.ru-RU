---
title: Обновление устройстваHealthScriptDeviceState
description: Обновление свойств объекта deviceHealthScriptDeviceState.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c2520d476265ee9745efa6a017d8de23a2bc77ad
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51609495"
---
# <a name="update-devicehealthscriptdevicestate"></a>Обновление устройстваHealthScriptDeviceState

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В корпусе запроса поставляем представление JSON для [объекта deviceHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)

В следующей таблице показаны свойства, необходимые при создании [устройстваHealthScriptDeviceState.](../resources/intune-devices-devicehealthscriptdevicestate.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ состояния состояния скрипта устройства для устройства. Это свойство доступно только для чтения.|
|detectionState|[runState](../resources/intune-devices-runstate.md)|Состояние обнаружения из последнего выполнения скрипта для здоровья устройств. Возможные значения: `unknown`, `success`, `fail`, `scriptError`, `pending`, `notApplicable`.|
|lastStateUpdateDateTime|DateTimeOffset|Последний период выполнения скрипта для здоровья устройств|
|expectedStateUpdateDateTime|DateTimeOffset|Следующий период, когда ожидается выполнение сценария состояния устройства|
|lastSyncDateTime|DateTimeOffset|Последний раз, когда расширение управления Intune синхронизировали с Intune|
|preRemediationDetectionScriptOutput|String|Выход сценария обнаружения перед исправлением|
|preRemediationDetectionScriptError|String|Ошибка из сценария обнаружения перед исправлением|
|remediationScriptError|String|Выход ошибки сценария восстановления|
|postRemediationDetectionScriptOutput|String|Вывод скрипта обнаружения после устранения|
|postRemediationDetectionScriptError|String|Ошибка из сценария обнаружения после устранения|
|remediationState|[remediationState](../resources/intune-devices-remediationstate.md)|Состояние исправлений из последнего выполнения скрипта для здоровья устройств. Возможные значения: `unknown`, `skipped`, `success`, `remediationFailed`, `scriptError`.|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код ответа и обновленный объект `200 OK` [deviceHealthScriptDeviceState](../resources/intune-devices-devicehealthscriptdevicestate.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/deviceRunStates/{deviceHealthScriptDeviceStateId}
Content-type: application/json
Content-length: 762

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "detectionState": "success",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
  "preRemediationDetectionScriptError": "Pre Remediation Detection Script Error value",
  "remediationScriptError": "Remediation Script Error value",
  "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value",
  "postRemediationDetectionScriptError": "Post Remediation Detection Script Error value",
  "remediationState": "skipped"
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 811

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDeviceState",
  "id": "fd2e4505-4505-fd2e-0545-2efd05452efd",
  "detectionState": "success",
  "lastStateUpdateDateTime": "2017-01-01T00:02:58.4418045-08:00",
  "expectedStateUpdateDateTime": "2016-12-31T23:58:26.9294641-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "preRemediationDetectionScriptOutput": "Pre Remediation Detection Script Output value",
  "preRemediationDetectionScriptError": "Pre Remediation Detection Script Error value",
  "remediationScriptError": "Remediation Script Error value",
  "postRemediationDetectionScriptOutput": "Post Remediation Detection Script Output value",
  "postRemediationDetectionScriptError": "Post Remediation Detection Script Error value",
  "remediationState": "skipped"
}
```




