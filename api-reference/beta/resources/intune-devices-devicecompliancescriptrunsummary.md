---
title: Тип ресурса Девицекомплианцескриптрунсуммари
description: Содержит свойства сводки по запуску сценария управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c436261961be8938e8905bc9f19be1690c7f79c4
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44789564"
---
# <a name="devicecompliancescriptrunsummary-resource-type"></a>Тип ресурса Девицекомплианцескриптрунсуммари

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства сводки по запуску сценария управления устройствами.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение Девицекомплианцескриптрунсуммари](../api/intune-devices-devicecompliancescriptrunsummary-get.md)|[девицекомплианцескриптрунсуммари](../resources/intune-devices-devicecompliancescriptrunsummary.md)|Чтение свойств и связей объекта [девицекомплианцескриптрунсуммари](../resources/intune-devices-devicecompliancescriptrunsummary.md) .|
|[Обновление Девицекомплианцескриптрунсуммари](../api/intune-devices-devicecompliancescriptrunsummary-update.md)|[девицекомплианцескриптрунсуммари](../resources/intune-devices-devicecompliancescriptrunsummary.md)|Обновление свойств объекта [девицекомплианцескриптрунсуммари](../resources/intune-devices-devicecompliancescriptrunsummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключевой объект сводки запуска сценария соответствия устройства. Это свойство доступно только для чтения.|
|ноиссуедетектеддевицекаунт|Int32|Количество устройств, для которых сценарий обнаружения не обнаружил проблему, и устройство находится в работоспособном состоянии. Допустимые значения: от 2147483648 до 2147483647|
|иссуедетектеддевицекаунт|Int32|Количество устройств, для которых сценарий обнаружения обнаружил неполадку. Допустимые значения: от 2147483648 до 2147483647|
|детектионскриптеррордевицекаунт|Int32|Количество устройств, на которых возникла ошибка при выполнении сценария обнаружения и который не был выполнен. Допустимые значения: от 2147483648 до 2147483647|
|детектионскриптпендингдевицекаунт|Int32|Количество устройств, на которых еще не выполнялась последняя версия сценария соответствия требованиям устройства. Допустимые значения: от 2147483648 до 2147483647|
|ластскриптрундатетиме|DateTimeOffset|Время последнего запуска сценария на всех устройствах|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceScriptRunSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceScriptRunSummary",
  "id": "String (identifier)",
  "noIssueDetectedDeviceCount": 1024,
  "issueDetectedDeviceCount": 1024,
  "detectionScriptErrorDeviceCount": 1024,
  "detectionScriptPendingDeviceCount": 1024,
  "lastScriptRunDateTime": "String (timestamp)"
}
```



