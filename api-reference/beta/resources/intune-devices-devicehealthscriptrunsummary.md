---
title: тип ресурса deviceHealthScriptRunSummary
description: Содержит свойства для сводки запуска скрипта управления устройствами.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3c8e001772e886d1d9d5fa0835d8ace5e30c560e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59124135"
---
# <a name="devicehealthscriptrunsummary-resource-type"></a>тип ресурса deviceHealthScriptRunSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для сводки запуска скрипта управления устройствами.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get deviceHealthScriptRunSummary](../api/intune-devices-devicehealthscriptrunsummary-get.md)|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|Чтение свойств и связей [объекта deviceHealthScriptRunSummary.](../resources/intune-devices-devicehealthscriptrunsummary.md)|
|[Обновление устройстваHealthScriptRunSummary](../api/intune-devices-devicehealthscriptrunsummary-update.md)|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|Обновление свойств объекта [deviceHealthScriptRunSummary.](../resources/intune-devices-devicehealthscriptrunsummary.md)|

## <a name="properties"></a>Свойства
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

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "String (identifier)",
  "noIssueDetectedDeviceCount": 1024,
  "issueDetectedDeviceCount": 1024,
  "detectionScriptErrorDeviceCount": 1024,
  "detectionScriptPendingDeviceCount": 1024,
  "detectionScriptNotApplicableDeviceCount": 1024,
  "issueRemediatedDeviceCount": 1024,
  "remediationSkippedDeviceCount": 1024,
  "issueReoccurredDeviceCount": 1024,
  "remediationScriptErrorDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)",
  "issueRemediatedCumulativeDeviceCount": 1024
}
```



