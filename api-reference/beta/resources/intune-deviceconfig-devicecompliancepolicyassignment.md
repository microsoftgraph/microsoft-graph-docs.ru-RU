---
title: Тип ресурса deviceCompliancePolicyAssignment
description: Назначение политики соответствия устройств требованиям.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3dc0445418a4ccc0d17b607df329d3b0e16fee6a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979461"
---
# <a name="devicecompliancepolicyassignment-resource-type"></a>Тип ресурса deviceCompliancePolicyAssignment

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
  }
}
```





