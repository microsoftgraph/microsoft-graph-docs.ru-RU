---
title: Тип ресурса deviceManagementScriptAssignment
description: Содержит свойства, используемые для назначения группе скрипта управления устройствами.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8eac4db0ce0bec29602b2b340e7d1604f4fa241d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158165"
---
# <a name="devicemanagementscriptassignment-resource-type"></a>Тип ресурса deviceManagementScriptAssignment

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для назначения группе скрипта управления устройствами.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementScriptAssignments](../api/intune-devices-devicemanagementscriptassignment-list.md)|[Коллекция deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|Список свойств и связей объектов [deviceManagementScriptAssignment.](../resources/intune-devices-devicemanagementscriptassignment.md)|
|[Get deviceManagementScriptAssignment](../api/intune-devices-devicemanagementscriptassignment-get.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md);|Чтение свойств и связей объекта [deviceManagementScriptAssignment.](../resources/intune-devices-devicemanagementscriptassignment.md)|
|[Создание deviceManagementScriptAssignment](../api/intune-devices-devicemanagementscriptassignment-create.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md);|Создание объекта [deviceManagementScriptAssignment.](../resources/intune-devices-devicemanagementscriptassignment.md)|
|[Удаление deviceManagementScriptAssignment](../api/intune-devices-devicemanagementscriptassignment-delete.md)|Нет|Удаляет [deviceManagementScriptAssignment.](../resources/intune-devices-devicemanagementscriptassignment.md)|
|[Обновление deviceManagementScriptAssignment](../api/intune-devices-devicemanagementscriptassignment-update.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md);|Обновление свойств объекта [deviceManagementScriptAssignment.](../resources/intune-devices-devicemanagementscriptassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта назначения группы сценариев управления устройствами. Это свойство доступно только для чтения.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|ИД группы Azure Active Directory, на который мы нацелим сценарий.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




