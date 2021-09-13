---
title: тип ресурса deviceManagementScriptGroupAssignment
description: Содержит свойства, используемые для назначения скрипта управления устройствами группе.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1f1a023ba87b62c143c4a7bb39aabee4015789d9
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59125967"
---
# <a name="devicemanagementscriptgroupassignment-resource-type"></a>тип ресурса deviceManagementScriptGroupAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства, используемые для назначения скрипта управления устройствами группе.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Списки deviceManagementScriptGroupAssignments](../api/intune-devices-devicemanagementscriptgroupassignment-list.md)|[коллекция deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Список свойств и связей объектов [deviceManagementScriptGroupAssignment.](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|
|[Get deviceManagementScriptGroupAssignment](../api/intune-devices-devicemanagementscriptgroupassignment-get.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Чтение свойств и связей [объекта deviceManagementScriptGroupAssignment.](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|
|[Создание deviceManagementScriptGroupAssignment](../api/intune-devices-devicemanagementscriptgroupassignment-create.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Создание нового [объекта deviceManagementScriptGroupAssignment.](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|
|[Удаление deviceManagementScriptGroupAssignment](../api/intune-devices-devicemanagementscriptgroupassignment-delete.md)|Нет|Удаляет [устройствоManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).|
|[Обновление deviceManagementScriptGroupAssignment](../api/intune-devices-devicemanagementscriptgroupassignment-update.md)|[deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|Обновление свойств объекта [deviceManagementScriptGroupAssignment.](../resources/intune-devices-devicemanagementscriptgroupassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта группового назначения скрипта управления устройствами. Это свойство доступно только для чтения.|
|targetGroupId|String|Id группы Azure Active Directory, на который мы нацелим сценарий.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```



