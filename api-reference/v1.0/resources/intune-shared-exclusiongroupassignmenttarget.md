---
title: Тип ресурса exclusionGroupAssignmentTarget
description: Представляет группу, которую следует исключить из назначения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fbfa4e6df9dae514a99fa96aace073bd702def9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254088"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a>Тип ресурса exclusionGroupAssignmentTarget

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет группу, которую следует исключить из назначения.


Наследуется от [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|groupId|String|ИД группы, являющейся объектом назначения. Наследуется от [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```



