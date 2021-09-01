---
title: тип ресурса policySetAssignment
description: Класс, содержащий свойства, используемые для назначения PolicySet.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f59de080a61f16a71c376853202ac630fd6b53c8
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58802427"
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
|id|Строка|Клавиша PolicySetAssignment.|
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



