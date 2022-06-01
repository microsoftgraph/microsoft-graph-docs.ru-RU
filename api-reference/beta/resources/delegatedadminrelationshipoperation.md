---
title: Тип ресурса delegatedAdminRelationshipOperation
description: Представляет долго выполняющуюся операцию, связанную с делегированным отношением администратора.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: bf369451c3a2b0d5ab4ca01894a4c7d546f7e630
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820940"
---
# <a name="delegatedadminrelationshipoperation-resource-type"></a>Тип ресурса delegatedAdminRelationshipOperation

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет долго выполняющуюся операцию, связанную с делегированным отношением администратора. Примером длительной операции может быть обновление объекта [delegatedAdminAccessAssignment](delegatedAdminAccessAssignment.md) .

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление delegatedAdminRelationshipOperations](../api/delegatedadminrelationship-list-operations.md)|[Коллекция delegatedAdminRelationshipOperation](delegatedadminrelationshipoperation.md)|Получение списка объектов **delegatedAdminRelationshipOperation и** их свойств.|
|[Получение delegatedAdminRelationshipOperation](../api/delegatedadminrelationshipoperation-get.md)|[delegatedAdminRelationshipOperation](delegatedadminrelationshipoperation.md)|Чтение свойств и связей объекта **delegatedAdminRelationshipOperation** .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Время создания длительной операции в формате ISO 8601 и времени в формате UTC. Только для чтения.|
|data|Строка|Данные (полезные данные) для операции. Только для чтения.|
|id|Строка|Уникальный идентификатор длительной операции делегированного администратора. Только для чтения. Наследуется от [сущности](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения длительной операции в формате ISO 8601 и времени в формате UTC. Только для чтения.|
|operationType|delegatedAdminRelationshipOperationType|Тип длительной операции. Возможные значения: `delegatedAdminAccessAssignmentUpdate`, `unknownFutureValue`. Только для чтения.|
|status|longRunningOperationStatus|Состояние операции. Только для чтения. Допустимые значения: `notStarted`, `running`, `succeeded`, `failed`, `unknownFutureValue`. Только для чтения. Поддерживает `$orderBy`.|

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
