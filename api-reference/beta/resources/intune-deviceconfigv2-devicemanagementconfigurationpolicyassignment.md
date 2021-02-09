---
title: Тип ресурса deviceManagementConfigurationPolicyAssignment
description: Объект DeviceManagementConfigurationPolicyAssignment назначает определенное deviceManagementConfigurationPolicy группе AAD.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5e571983c36c2832aef5c43478d1cccca7361aca
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157668"
---
# <a name="devicemanagementconfigurationpolicyassignment-resource-type"></a>Тип ресурса deviceManagementConfigurationPolicyAssignment

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект DeviceManagementConfigurationPolicyAssignment назначает определенное deviceManagementConfigurationPolicy группе AAD.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementConfigurationPolicyAssignments](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-list.md)|[Коллекция deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Список свойств и связей объектов [deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|
|[Get deviceManagementConfigurationPolicyAssignment](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-get.md)|[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Чтение свойств и связей объекта [deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|
|[Создание deviceManagementConfigurationPolicyAssignment](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-create.md)|[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Создание объекта [deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|
|[Удаление deviceManagementConfigurationPolicyAssignment](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-delete.md)|Нет|Удаляет [deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|
|[Обновление deviceManagementConfigurationPolicyAssignment](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-update.md)|[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Обновление свойств объекта [deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ назначения.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Целевой объект назначения для DeviceManagementConfigurationPolicy.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationPolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationPolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




