---
title: тип ресурса privilegedAccess
description: " например, представляет `privilegedAccess/azureResources` собой управление привилегированным доступом PIM к ресурсам Azure."
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: japere
ms.openlocfilehash: f90b76ca24a4bded8c2206a4a5f45ebcfde4d825
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64509555"
---
# <a name="privilegedaccess-resource-type"></a>тип ресурса privilegedAccess

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет группу функциональных возможностей, предоставляемых службой управление привилегированными пользователями (PIM). Различные экземпляры представляют `privilegedAccess` различных поставщиков, управляемых PIM; например, `privilegedAccess/azureResources` представляет PIM, управляющую привилегированным доступом к ресурсам Azure.


`privilegedAccess` только для чтения на данный момент. Нет `POST`, `PUT`или `PATCH`операции `DELETE` поддерживаются в наборе `privilegedAccess` сущности.

## <a name="properties"></a>Свойства
| Свойство  | Тип      |Описание|
|:----------|:----------|:----------|
|id         |Строка     |ID поставщика, управляемого PIM.|
|displayName|Строка     |Отображает имя поставщика, управляемого PIM.|


## <a name="relationships"></a>Связи
| Связь   | Тип                                         |Описание|
|:---------------|:---------------------------------------------|:----------|
|resources       |[коллекция governanceResource](../resources/governanceresource.md)            |Коллекция ресурсов для поставщика.|
|roleAssignments |[коллекция governanceRoleAssignment](../resources/governanceroleassignment.md)|Коллекция назначений ролей для поставщика.|
|roleDefinitions |[коллекция governanceRoleDefinition](../resources/governanceroledefinition.md)|Коллекция порочаций ролей для поставщика.|
|roleAssignmentRequests |[коллекция governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Коллекция запросов на назначение ролей для поставщика.|
|roleSettings |[коллекция governanceRoleSetting](../resources/governancerolesetting.md)|Коллекция параметров ролей для поставщика.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.privilegedAccess"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


