---
title: Обновление Девицехеалсскриптрунсуммари
description: Обновление свойств объекта Девицехеалсскриптрунсуммари.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0ce21ae48b1bcc6053eb88af38eda4b69d6eccef
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49235051"
---
# <a name="update-devicehealthscriptrunsummary"></a>Обновление Девицехеалсскриптрунсуммари

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md) .

## <a name="prerequisites"></a>Необходимые компоненты
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке убывания привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Приложение|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All|

## <a name="http-request"></a>HTTP-запрос
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Авторизация|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md) в формате JSON.

В следующей таблице приведены свойства, необходимые при создании [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md).

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключевой объект сводки запуска сценария работоспособности устройства. Это свойство доступно только для чтения.|
|ноиссуедетектеддевицекаунт|Int32|Количество устройств, для которых сценарий обнаружения не обнаружил проблему, и устройство находится в работоспособном состоянии.|
|иссуедетектеддевицекаунт|Int32|Количество устройств, для которых обнаружена ошибка сценария обнаружения|
|детектионскриптеррордевицекаунт|Int32|Количество устройств, на которых возникла ошибка при выполнении сценария обнаружения и который не был выполнен|
|детектионскриптпендингдевицекаунт|Int32|Количество устройств, на которых еще не выполнялась последняя версия сценария работоспособности устройства|
|иссуеремедиатеддевицекаунт|Int32|Количество устройств, для которых сценарий исправления мог разрешить обнаруженную проблему|
|ремедиатионскиппеддевицекаунт|Int32|Количество устройств, для которых было пропущено исправление|
|иссуереоккурреддевицекаунт|Int32|Количество устройств, для которых сценарий исправления успешно выполнен, но не удалось разрешить обнаруженную проблему|
|ремедиатионскриптеррордевицекаунт|Int32|Количество устройств, для которых при выполнении сценария исправления возникла ошибка и оно не было завершено|
|ластскриптрундатетиме|DateTimeOffset|Время последнего запуска сценария на всех устройствах|
|иссуеремедиатедкумулативедевицекаунт|Int32|Количество устройств, которые были исправлены за последние 30 дней|



## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает `200 OK` код отклика и обновленный объект [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md) в тексте отклика.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
Content-type: application/json
Content-length: 494

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "issueRemediatedDeviceCount": 10,
  "remediationSkippedDeviceCount": 13,
  "issueReoccurredDeviceCount": 10,
  "remediationScriptErrorDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00",
  "issueRemediatedCumulativeDeviceCount": 4
}
```

### <a name="response"></a>Отклик
Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 543

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "8221b043-b043-8221-43b0-218243b02182",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "issueRemediatedDeviceCount": 10,
  "remediationSkippedDeviceCount": 13,
  "issueReoccurredDeviceCount": 10,
  "remediationScriptErrorDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00",
  "issueRemediatedCumulativeDeviceCount": 4
}
```




