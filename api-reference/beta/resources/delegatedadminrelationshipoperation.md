---
title: делегирован тип ресурса delegatedAdminRelationshipOperation
description: Представляет собой долгосрочную операцию, связанную с делегированной связью администратора.
author: adtangir
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 50aaad489ba955c4d7ba2a9c0992e63b445732b5
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589800"
---
# <a name="delegatedadminrelationshipoperation-resource-type"></a>делегирован тип ресурса delegatedAdminRelationshipOperation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет собой долгосрочную операцию, связанную с делегированной связью администратора. Примером длительной операции может быть обновление объекта [делегированияAdminAccessAssignment](delegatedAdminAccessAssignment.md) .

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список делегированAdminRelationshipOperations](../api/delegatedadminrelationship-list-operations.md)|[delegatedAdminRelationshipOperation](delegatedadminrelationshipoperation.md) collection|Получите список объектов **делегированияAdminRelationshipOperation и** их свойств.|
|[ДелегированиеAdminRelationshipOperation](../api/delegatedadminrelationshipoperation-get.md)|[delegatedAdminRelationshipOperation](delegatedadminrelationshipoperation.md)|Ознакомьтесь с свойствами и отношениями объекта **делегированияAdminRelationshipOperation** .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Время в формате ISO 8601 и время создания длительной операции UTC. Только для чтения.|
|data|Строка|Данные (полезной нагрузки) для операции. Только для чтения.|
|id|String|Уникальный идентификатор делегирования длительной операции администратора. Только для чтения. Наследуется от [сущности](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Время в формате ISO 8601 и время UTC, когда в последний раз была изменена долгосрочная операция. Только для чтения.|
|operationType|delegatedAdminRelationshipOperationType|Тип длительной операции. Возможные значения: `delegatedAdminAccessAssignmentUpdate`, `unknownFutureValue`. Только для чтения.|
|status|delegatedAdminRelationshipOperationStatus|Состояние операции. Только для чтения. Допустимые значения: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`. Только для чтения. Поддерживает `$orderBy`.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.delegatedAdminRelationshipOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationshipOperation",
  "id": "String (identifier)",
  "operationType": "String",
  "data": "String",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```
