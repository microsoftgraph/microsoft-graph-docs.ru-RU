---
title: тип ресурса policySetAssignment
description: Класс, содержащий свойства, используемые для назначения PolicySet.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ed8f6cde042a4200203918fe81c29ada714e28a4a8a989243331ea50b5f3f83
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54239121"
---
# <a name="policysetassignment-resource-type"></a>тип ресурса policySetAssignment

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Класс, содержащий свойства, используемые для назначения PolicySet.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Списки политикSetAssignments](../api/intune-policyset-policysetassignment-list.md)|[коллекция policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Список свойств и связей объектов [policySetAssignment.](../resources/intune-policyset-policysetassignment.md)|
|[Get policySetAssignment](../api/intune-policyset-policysetassignment-get.md)|[policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Чтение свойств и связей [объекта policySetAssignment.](../resources/intune-policyset-policysetassignment.md)|
|[Создание политикиSetAssignment](../api/intune-policyset-policysetassignment-create.md)|[policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Создание нового [объекта policySetAssignment.](../resources/intune-policyset-policysetassignment.md)|
|[Удаление политикиSetAssignment](../api/intune-policyset-policysetassignment-delete.md)|Нет|Удаляет [политикуSetAssignment](../resources/intune-policyset-policysetassignment.md).|
|[Обновление политикиSetAssignment](../api/intune-policyset-policysetassignment-update.md)|[policySetAssignment](../resources/intune-policyset-policysetassignment.md)|Обновление свойств объекта [policySetAssignment.](../resources/intune-policyset-policysetassignment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Клавиша PolicySetAssignment.|
|lastModifiedDateTime|DateTimeOffset|Последнее измененное время policySetAssignment.|
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




