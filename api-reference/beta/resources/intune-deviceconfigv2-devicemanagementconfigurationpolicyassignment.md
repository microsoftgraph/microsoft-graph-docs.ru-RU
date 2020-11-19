---
title: Тип ресурса Девицеманажементконфигуратионполициассигнмент
description: Объект Девицеманажементконфигуратионполициассигнмент назначает определенный Девицеманажементконфигуратионполици группе AAD.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4247518598cc9094346814079be37fc5d6073286
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49242220"
---
# <a name="devicemanagementconfigurationpolicyassignment-resource-type"></a>Тип ресурса Девицеманажементконфигуратионполициассигнмент

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект Девицеманажементконфигуратионполициассигнмент назначает определенный Девицеманажементконфигуратионполици группе AAD.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементконфигуратионполициассигнментс](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-list.md)|Коллекция [девицеманажементконфигуратионполициассигнмент](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Список свойств и связей объектов [девицеманажементконфигуратионполициассигнмент](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) .|
|[Получение Девицеманажементконфигуратионполициассигнмент](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-get.md)|[девицеманажементконфигуратионполициассигнмент](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Чтение свойств и связей объекта [девицеманажементконфигуратионполициассигнмент](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) .|
|[Создание Девицеманажементконфигуратионполициассигнмент](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-create.md)|[девицеманажементконфигуратионполициассигнмент](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Создание нового объекта [девицеманажементконфигуратионполициассигнмент](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) .|
|[Удаление Девицеманажементконфигуратионполициассигнмент](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-delete.md)|Нет|Удаляет объект [девицеманажементконфигуратионполициассигнмент](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md).|
|[Обновление Девицеманажементконфигуратионполициассигнмент](../api/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment-update.md)|[девицеманажементконфигуратионполициассигнмент](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md)|Обновление свойств объекта [девицеманажементконфигуратионполициассигнмент](../resources/intune-deviceconfigv2-devicemanagementconfigurationpolicyassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ назначения.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Цель назначения для Девицеманажементконфигуратионполици.|

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
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```




