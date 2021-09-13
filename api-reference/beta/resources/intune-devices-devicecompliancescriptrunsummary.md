---
title: тип ресурса deviceComplianceScriptRunSummary
description: Содержит свойства для сводки запуска скрипта управления устройствами.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 84bd44e53266976564f2eb4bb5ea6277cba0208c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033562"
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
|id|String|Клавиша скрипта соответствия устройству запускать сводную сущность. Это свойство доступно только для чтения.|
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



