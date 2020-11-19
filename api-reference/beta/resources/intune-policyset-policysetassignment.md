---
title: Тип ресурса Полицисетассигнмент
description: Класс, содержащий свойства, которые используются для назначения политик.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 51cce7ad66c1374f27c861b1db602ffe6122088c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288028"
---
# <a name="policysetassignment-resource-type"></a>Тип ресурса Полицисетассигнмент

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, которые используются для назначения политик.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Полицисетассигнментс](../api/intune-policyset-policysetassignment-list.md)|Коллекция [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md)|Список свойств и связей объектов [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) .|
|[Получение Полицисетассигнмент](../api/intune-policyset-policysetassignment-get.md)|[policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Чтение свойств и связей объекта [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) .|
|[Создание Полицисетассигнмент](../api/intune-policyset-policysetassignment-create.md)|[policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Создание нового объекта [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) .|
|[Удаление Полицисетассигнмент](../api/intune-policyset-policysetassignment-delete.md)|Нет|Удаляет объект [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md).|
|[Обновление Полицисетассигнмент](../api/intune-policyset-policysetassignment-update.md)|[policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Обновление свойств объекта [полицисетассигнмент](../resources/intune-policyset-policysetassignment.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ Полицисетассигнмент.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения Полицисетассигнмент.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Целевая группа Полицисетассигнмент|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.policySetAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.policySetAssignment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String"
  }
}
```




