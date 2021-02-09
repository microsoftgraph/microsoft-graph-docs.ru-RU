---
title: Тип ресурса policySetAssignment
description: Класс, содержащий свойства, используемые для назначения policySet.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: da5049ecfbfd7f6516c77b1aa662cc35d648b13c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158424"
---
# <a name="policysetassignment-resource-type"></a>Тип ресурса policySetAssignment

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для назначения policySet.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список policySetAssignments](../api/intune-policyset-policysetassignment-list.md)|[Коллекция policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Список свойств и связей объектов [policySetAssignment.](../resources/intune-policyset-policysetassignment.md)|
|[Get policySetAssignment](../api/intune-policyset-policysetassignment-get.md)|[policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Чтение свойств и связей объекта [policySetAssignment.](../resources/intune-policyset-policysetassignment.md)|
|[Создание policySetAssignment](../api/intune-policyset-policysetassignment-create.md)|[policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Создание объекта [policySetAssignment.](../resources/intune-policyset-policysetassignment.md)|
|[Удаление policySetAssignment](../api/intune-policyset-policysetassignment-delete.md)|Нет|Удаляет [политикуSetAssignment.](../resources/intune-policyset-policysetassignment.md)|
|[Обновление policySetAssignment](../api/intune-policyset-policysetassignment-update.md)|[policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Обновление свойств объекта [policySetAssignment.](../resources/intune-policyset-policysetassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ policySetAssignment.|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения policySetAssignment.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Целевая группа PolicySetAssignment|

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
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "String",
    "deviceAndAppManagementAssignmentFilterType": "String",
    "collectionId": "String"
  }
}
```




