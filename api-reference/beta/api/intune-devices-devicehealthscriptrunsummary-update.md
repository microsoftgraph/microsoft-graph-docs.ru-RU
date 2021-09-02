---
title: Обновление устройстваHealthScriptRunSummary
description: Обновление свойств объекта deviceHealthScriptRunSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fedb694c2142f9826aa4da43616c84a716ad387c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819979"
---
# <a name="update-devicehealthscriptrunsummary"></a>Обновление устройстваHealthScriptRunSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Обновление свойств объекта [deviceHealthScriptRunSummary.](../resources/intune-devices-devicehealthscriptrunsummary.md)

## <a name="prerequisites"></a>Необходимые компоненты
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
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## <a name="request-headers"></a>Заголовки запроса
|Заголовок|Значение|
|:---|:---|
|Authorization|Bearer &lt;token&gt;. Обязательный.|
|Accept|application/json|

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON для [объекта deviceHealthScriptRunSummary.](../resources/intune-devices-devicehealthscriptrunsummary.md)

В следующей таблице показаны свойства, необходимые при создании [устройстваHealthScriptRunSummary.](../resources/intune-devices-devicehealthscriptrunsummary.md)

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ скрипта для службы службы устройств запустите объект сводки. Это свойство доступно только для чтения.|
|noIssueDetectedDeviceCount|Int32|Количество устройств, для которых сценарий обнаружения не нашел проблемы и устройство является здоровым|
|issueDetectedDeviceCount|Int32|Количество устройств, для которых скрипт обнаружения обнаружил проблему|
|detectionScriptErrorDeviceCount|Int32|Количество устройств, на которых при выполнении скрипта обнаружения произошла ошибка и не была завершена|
|detectionScriptPendingDeviceCount|Int32|Количество устройств, которые еще не запускают последнюю версию скрипта здоровья устройств|
|detectionScriptNotApplicableDeviceCount|Int32|Количество устройств, для которых сценарий обнаружения не был применим|
|issueRemediatedDeviceCount|Int32|Количество устройств, для которых сценарий восстановления смог устранить обнаруженную проблему|
|remediationSkippedDeviceCount|Int32|Количество устройств, для которых было пропущено исправление|
|issueReoccurredDeviceCount|Int32|Количество устройств, для которых успешно выполнен сценарий восстановления, но не удалось устранить обнаруженную проблему|
|remediationScriptErrorDeviceCount|Int32|Количество устройств, для которых при выполнении сценария восстановления произошла ошибка и не была завершена|
|lastScriptRunDateTime|DateTimeOffset|Время последнего запуска сценария на всех устройствах|
|issueRemediatedCumulativeDeviceCount|Int32|Количество устройств, которые были исправлены за последние 30 дней|



## <a name="response"></a>Отклик
В случае успешной работы этот метод возвращает код отклика и обновленный объект `200 OK` [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) в тексте ответа.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
Content-type: application/json
Content-length: 543

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "detectionScriptNotApplicableDeviceCount": 7,
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
Content-Length: 592

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "8221b043-b043-8221-43b0-218243b02182",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "detectionScriptNotApplicableDeviceCount": 7,
  "issueRemediatedDeviceCount": 10,
  "remediationSkippedDeviceCount": 13,
  "issueReoccurredDeviceCount": 10,
  "remediationScriptErrorDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00",
  "issueRemediatedCumulativeDeviceCount": 4
}
```



