---
title: Тип ресурса Девицехеалсскриптрунсуммари
description: Содержит свойства сводки по запуску сценария управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d6e06ba1937d5a18b798dbca7702d37aa64bc71f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695000"
---
# <a name="devicehealthscriptrunsummary-resource-type"></a>Тип ресурса Девицехеалсскриптрунсуммари

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства сводки по запуску сценария управления устройствами.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Девицехеалсскриптрунсуммари](../api/intune-devices-devicehealthscriptrunsummary-get.md)|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|Чтение свойств и связей объекта [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md) .|
|[Обновление Девицехеалсскриптрунсуммари](../api/intune-devices-devicehealthscriptrunsummary-update.md)|[deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md)|Обновление свойств объекта [девицехеалсскриптрунсуммари](../resources/intune-devices-devicehealthscriptrunsummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключевой объект сводки запуска сценария работоспособности устройства. Это свойство доступно только для чтения.|
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
  "issueRemediatedDeviceCount": 1024,
  "remediationSkippedDeviceCount": 1024,
  "issueReoccurredDeviceCount": 1024,
  "remediationScriptErrorDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)",
  "issueRemediatedCumulativeDeviceCount": 1024
}
```





