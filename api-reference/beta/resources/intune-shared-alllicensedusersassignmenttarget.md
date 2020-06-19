---
title: Тип ресурса allLicensedUsersAssignmentTarget
description: Представляет ресурс, назначенный всем лицензированным пользователям в клиенте.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4388710e079366193f2a2ca7bd842a2d7b5763cf
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793600"
---
# <a name="alllicensedusersassignmenttarget-resource-type"></a>Тип ресурса allLicensedUsersAssignmentTarget

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет ресурс, назначенный всем лицензированным пользователям в клиенте.


Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|девицеандаппманажементассигнментфилтерид|String|Идентификатор фильтра для назначения назначения. Наследуется от [девицеандаппманажементассигнменттаржет](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|
|девицеандаппманажементассигнментфилтертипе|[девицеандаппманажементассигнментфилтертипе](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|Тип фильтра целевого назначения, например, Exclude или include. Наследуется от [девицеандаппманажементассигнменттаржет](../resources/intune-shared-deviceandappmanagementassignmenttarget.md). Возможные значения: `none`, `include`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.allLicensedUsersAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String"
}
```



