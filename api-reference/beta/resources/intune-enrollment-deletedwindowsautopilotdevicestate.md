---
title: удаленный тип ресурсаWindowsAutopilotDeviceState
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 87113449f0c00722f3aa1d3a1e614873524d43a6
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/23/2021
ms.locfileid: "51146818"
---
# <a name="deletedwindowsautopilotdevicestate-resource-type"></a>удаленный тип ресурсаWindowsAutopilotDeviceState

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Н/Д

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|serialNumber|String|Серийный номер устройства автопилота|
|deviceRegistrationId|Строка|Регистрационный номер устройства ZTD .|
|deletionState|[windowsAutopilotDeviceDeletionState](../resources/intune-enrollment-windowsautopilotdevicedeletionstate.md)|Состояние удаления устройства. Возможные значения: `unknown`, `failed`, `accepted`, `error`.|
|errorMessage|Строка|Сообщение об ошибке удаления устройства.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deletedWindowsAutopilotDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deletedWindowsAutopilotDeviceState",
  "serialNumber": "String",
  "deviceRegistrationId": "String",
  "deletionState": "String",
  "errorMessage": "String"
}
```




