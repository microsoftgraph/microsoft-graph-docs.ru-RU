---
title: Тип ресурса configurationManagerCollectionAssignmentTarget
description: Представляет назначение коллекции Configuration Manager.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5d32813e7c5c7cdae889406d694f686630311166
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161012"
---
# <a name="configurationmanagercollectionassignmenttarget-resource-type"></a>Тип ресурса configurationManagerCollectionAssignmentTarget

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет назначение коллекции Configuration Manager.


Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceAndAppManagementAssignmentFilterId|String|ИД фильтра для целевого назначения. Наследуется [от deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|
|deviceAndAppManagementAssignmentFilterType|[deviceAndAppManagementAssignmentFilterType](../resources/intune-shared-deviceandappmanagementassignmentfiltertype.md)|Тип фильтра целевого назначения, например Exclude или Include. Наследуется [от deviceAndAppManagementAssignmentTarget.](../resources/intune-shared-deviceandappmanagementassignmenttarget.md) Возможные значения: `none`, `include`, `exclude`.|
|collectionId|String|ИД коллекции, которая является целевым объектом назначения.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerCollectionAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "String",
  "collectionId": "String"
}
```




