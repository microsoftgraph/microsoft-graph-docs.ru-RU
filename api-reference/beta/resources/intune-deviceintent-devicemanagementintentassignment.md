---
title: тип ресурса deviceManagementIntentAssignment
description: Объект назначения намерения
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8cc2ef384439c11d8be7a21ffc4965cd49d056ca
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137961"
---
# <a name="devicemanagementintentassignment-resource-type"></a>тип ресурса deviceManagementIntentAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Объект назначения намерения

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список deviceManagementIntentAssignments](../api/intune-deviceintent-devicemanagementintentassignment-list.md)|[коллекция deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Список свойств и связей [объектов deviceManagementIntentAssignment.](../resources/intune-deviceintent-devicemanagementintentassignment.md)|
|[Get deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-get.md)|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Чтение свойств и связей [объекта deviceManagementIntentAssignment.](../resources/intune-deviceintent-devicemanagementintentassignment.md)|
|[Создание deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-create.md)|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Создание нового [объекта deviceManagementIntentAssignment.](../resources/intune-deviceintent-devicemanagementintentassignment.md)|
|[Удаление deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-delete.md)|Нет|Удаляет [устройствоManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md).|
|[Обновление deviceManagementIntentAssignment](../api/intune-deviceintent-devicemanagementintentassignment-update.md)|[deviceManagementIntentAssignment](../resources/intune-deviceintent-devicemanagementintentassignment.md)|Обновление свойств объекта [deviceManagementIntentAssignment.](../resources/intune-deviceintent-devicemanagementintentassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|ID назначения|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Цель назначения|

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



