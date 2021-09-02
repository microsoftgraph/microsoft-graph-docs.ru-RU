---
title: тип ресурса deviceManagementConfigurationPolicyAssignment
description: Объект DeviceManagementConfigurationPolicyAssignment назначает группе AAD определенную группу DeviceManagementConfigurationPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 848e1829f22128d11893f13ed02d299381ff3676
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58792584"
---
# <a name="devicemanagementconfigurationpolicyassignment-resource-type"></a>тип ресурса deviceManagementConfigurationPolicyAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект DeviceManagementConfigurationPolicyAssignment назначает группе AAD определенную группу DeviceManagementConfigurationPolicy.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementConfigurationPolicyAssignments](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-list.md)|[коллекция deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Список свойств и связей [объектов deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|
|[Get deviceManagementConfigurationPolicyAssignment](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-get.md)|[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Чтение свойств и связей [объекта deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|
|[Создание deviceManagementConfigurationPolicyAssignment](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-create.md)|[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Создание нового [объекта deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|
|[Удаление deviceManagementConfigurationPolicyAssignment](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-delete.md)|Нет|Удаляет [устройствоManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md).|
|[Обновление deviceManagementConfigurationPolicyAssignment](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-update.md)|[deviceManagementConfigurationPolicyAssignment](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Обновление свойств объекта [deviceManagementConfigurationPolicyAssignment.](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ назначения.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Цель назначения для DeviceManagementConfigurationPolicy.|
|source|[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|Источник назначения для политики соответствия требованиям устройств, прямой или пакетной или политикиSet. Возможные значения: `direct`, `policySets`.|
|sourceId|String|Идентификатор источника назначения.|

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
  },
  "source": "String",
  "sourceId": "String"
}
```



