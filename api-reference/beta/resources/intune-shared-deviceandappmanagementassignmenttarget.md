---
title: Тип ресурса deviceAndAppManagementAssignmentTarget
description: Базовый тип для объектов назначения.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4194d5afb7f7c90f658c558d8609badef2d89cfc
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793495"
---
# <a name="deviceandappmanagementassignmenttarget-resource-type"></a>Тип ресурса deviceAndAppManagementAssignmentTarget

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый тип для объектов назначения.

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|девицеандаппманажементассигнментфилтерид|String|Идентификатор фильтра для назначения назначения.|
|девицеандаппманажементассигнментфилтертипе|[девицеандаппманажементассигнментфилтертипе](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|Тип фильтра целевого назначения, например, Exclude или include. Возможные значения: `none`, `include`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String"
}
```



