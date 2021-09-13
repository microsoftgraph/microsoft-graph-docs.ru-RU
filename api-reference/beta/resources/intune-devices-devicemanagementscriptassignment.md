---
title: Тип ресурса deviceManagementScriptAssignment
description: Содержит свойства, используемые для назначения скрипта управления устройствами группе.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b6a9de04b4accb3461d9ec26612ab1df2ce6e86b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59105864"
---
# <a name="devicemanagementscriptassignment-resource-type"></a>Тип ресурса deviceManagementScriptAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для назначения скрипта управления устройствами группе.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Списки deviceManagementScriptAssignments](../api/intune-devices-devicemanagementscriptassignment-list.md)|[коллекция deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|Список свойств и связей объектов [deviceManagementScriptAssignment.](../resources/intune-devices-devicemanagementscriptassignment.md)|
|[Get deviceManagementScriptAssignment](../api/intune-devices-devicemanagementscriptassignment-get.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|Чтение свойств и связей [объекта deviceManagementScriptAssignment.](../resources/intune-devices-devicemanagementscriptassignment.md)|
|[Создание deviceManagementScriptAssignment](../api/intune-devices-devicemanagementscriptassignment-create.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|Создание нового [объекта deviceManagementScriptAssignment.](../resources/intune-devices-devicemanagementscriptassignment.md)|
|[Удаление deviceManagementScriptAssignment](../api/intune-devices-devicemanagementscriptassignment-delete.md)|Нет|Удаляет [устройствоManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md).|
|[Обновление deviceManagementScriptAssignment](../api/intune-devices-devicemanagementscriptassignment-update.md)|[deviceManagementScriptAssignment](../resources/intune-devices-devicemanagementscriptassignment.md)|Обновление свойств объекта [deviceManagementScriptAssignment.](../resources/intune-devices-devicemanagementscriptassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта группового назначения скрипта управления устройствами. Это свойство доступно только для чтения.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Id группы Azure Active Directory, на который мы нацелим сценарий.|

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



