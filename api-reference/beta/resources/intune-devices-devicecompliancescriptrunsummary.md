---
title: тип ресурса deviceComplianceScriptRunSummary
description: Содержит свойства для сводки запуска скрипта управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c63a7c9a0fba7a0d015d3770feba24084bd5bda1
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803267"
---
# <a name="devicecompliancescriptrunsummary-resource-type"></a>тип ресурса deviceComplianceScriptRunSummary

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для сводки запуска скрипта управления устройствами.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Get deviceComplianceScriptRunSummary](../api/intune-devices-devicecompliancescriptrunsummary-get.md)|[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)|Чтение свойств и связей [объекта deviceComplianceScriptRunSummary.](../resources/intune-devices-devicecompliancescriptrunsummary.md)|
|[Обновление deviceComplianceScriptRunSummary](../api/intune-devices-devicecompliancescriptrunsummary-update.md)|[deviceComplianceScriptRunSummary](../resources/intune-devices-devicecompliancescriptrunsummary.md)|Обновление свойств объекта [deviceComplianceScriptRunSummary.](../resources/intune-devices-devicecompliancescriptrunsummary.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Клавиша скрипта соответствия устройству запускать сводную сущность. Это свойство доступно только для чтения.|
|noIssueDetectedDeviceCount|Int32|Количество устройств, для которых сценарий обнаружения не нашел проблемы и устройство является здоровым. Допустимые значения 2147483648 2147483647|
|issueDetectedDeviceCount|Int32|Количество устройств, для которых скрипт обнаружения обнаружил проблему. Допустимые значения 2147483648 2147483647|
|detectionScriptErrorDeviceCount|Int32|Количество устройств, на которых при выполнении скрипта обнаружения произошла ошибка и не была завершена. Допустимые значения 2147483648 2147483647|
|detectionScriptPendingDeviceCount|Int32|Количество устройств, которые еще не запускают последнюю версию сценария соответствия требованиям. Допустимые значения 2147483648 2147483647|
|lastScriptRunDateTime|DateTimeOffset|Время последнего запуска сценария на всех устройствах|

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



