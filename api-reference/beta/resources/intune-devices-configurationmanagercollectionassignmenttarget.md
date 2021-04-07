---
title: тип ресурса configurationManagerCollectionAssignmentTarget
description: Представляет назначение коллекции диспетчера конфигурации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cb43c23a0eafaefea0b9265102880de58008f153
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/07/2021
ms.locfileid: "51610884"
---
# <a name="configurationmanagercollectionassignmenttarget-resource-type"></a>тип ресурса configurationManagerCollectionAssignmentTarget

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Представляет назначение коллекции диспетчера конфигурации.


Наследуется от ресурса [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|deviceAndAppManagementAssignmentFilterId|String|Id фильтра для целевого назначения. Унаследованный от [deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md)|
|deviceAndAppManagementAssignmentFilterType|[deviceAndAppManagementAssignmentFilterType](../resources/intune-devices-deviceandappmanagementassignmentfiltertype.md)|Тип фильтра целевого назначения, то есть исключить или включить. Наследуется [от deviceAndAppManagementAssignmentTarget](../resources/intune-devices-deviceandappmanagementassignmenttarget.md). Возможные значения: `none`, `include`, `exclude`.|
|collectionId|String|Ид коллекции, который является объектом назначения.|

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




