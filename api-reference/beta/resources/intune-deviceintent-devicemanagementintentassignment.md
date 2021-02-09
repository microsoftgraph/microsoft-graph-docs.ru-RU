---
title: Тип ресурса deviceManagementIntentAssignment
description: Сущность назначения намерения
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5dc2fc81635f3c5e4c61fb70a3bab5f176ee09a8
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161511"
---
# <a name="devicemanagementintentassignment-resource-type"></a>Тип ресурса deviceManagementIntentAssignment

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Сущность назначения намерения

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementIntentAssignments](../api/intune-deviceintent-devicemanagementintentassignment-list.md)|[Коллекция deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Список свойств и связей объектов [deviceManagementIntentAssignment.](../resources/intune-deviceintent-devicemanagementintentassignment.md)|
|[Get deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-get.md)|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Чтение свойств и связей объекта [deviceManagementIntentAssignment.](../resources/intune-deviceintent-devicemanagementintentassignment.md)|
|[Создание deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-create.md)|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Создание объекта [deviceManagementIntentAssignment.](../resources/intune-deviceintent-devicemanagementintentassignment.md)|
|[Удаление deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-delete.md)|Нет|Удаляет [deviceManagementIntentAssignment.](../resources/intune-deviceintent-devicemanagementintentassignment.md)|
|[Обновление deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-update.md)|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Обновление свойств объекта [deviceManagementIntentAssignment.](../resources/intune-deviceintent-devicemanagementintentassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ИД назначения|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Целевой объект назначения|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




