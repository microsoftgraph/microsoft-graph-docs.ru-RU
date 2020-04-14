---
title: Тип ресурса deviceCompliancePolicyAssignment
description: Назначение политики соответствия устройств требованиям.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0732cd8314e6eeb4fb7afc30b7c7fe3d705d07e8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469547"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a>Тип ресурса deviceCompliancePolicyAssignment

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Назначение политики соответствия устройств требованиям.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceCompliancePolicyAssignment](../api/intune-deviceconfig-devicecompliancepolicyassignment-list.md)|Коллекция [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|Список свойств и связей объектов [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).|
|[Получение объекта deviceCompliancePolicyAssignment](../api/intune-deviceconfig-devicecompliancepolicyassignment-get.md)|[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md);|Чтение свойств и связей объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).|
|[Создание объекта deviceCompliancePolicyAssignment](../api/intune-deviceconfig-devicecompliancepolicyassignment-create.md)|[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md);|Создание объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).|
|[Удаление объекта deviceCompliancePolicyAssignment](../api/intune-deviceconfig-devicecompliancepolicyassignment-delete.md)|Нет|Удаляет объект [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).|
|[Обновление объекта deviceCompliancePolicyAssignment](../api/intune-deviceconfig-devicecompliancepolicyassignment-update.md)|[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)|Обновление свойств объекта [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Цель для назначения политики соответствия.|
|source|[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md)|Источник назначения для политики соответствия требованиям устройств, Direct или в упаковке/политике. Возможные значения: `direct`, `policySets`.|
|Идентификатор|String|Идентификатор источника назначения.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "source": "String",
  "sourceId": "String"
}
```



