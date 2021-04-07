---
title: Тип ресурса groupAssignmentTarget
description: Представляет ресурс, назначенный группе.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 437d4c8ab11a0cf095e58b56b271aecb9e42729c
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612326"
---
# <a name="groupassignmenttarget-resource-type"></a>Тип ресурса groupAssignmentTarget

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет ресурс, назначенный группе.


Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceAndAppManagementAssignmentFilterId|String|Id фильтра для целевого назначения. Унаследованный от [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)|
|deviceAndAppManagementAssignmentFilterType|[deviceAndAppManagementAssignmentFilterType](../resources/intune-devices-deviceandappmanagementassignmentfiltertype.md)|Тип фильтра целевого назначения, то есть исключить или включить. Наследуется [от deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md). Возможные значения: `none`, `include`, `exclude`.|
|groupId|String|Идентификатор группы-объекта назначения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String",
  "groupId": "String"
}
```




