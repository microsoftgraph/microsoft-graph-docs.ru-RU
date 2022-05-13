---
title: Тип ресурса privilegedAccess
description: " Например, представляет `privilegedAccess/azureResources` PIM, управляющий привилегированным доступом к ресурсам Azure."
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 408f3fe7e6b0b8c05dfbb27599bc5fa7b048d869
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397957"
---
# <a name="privilegedaccess-resource-type"></a>Тип ресурса privilegedAccess

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет группу функциональных возможностей, предоставляемых службой управление привилегированными пользователями (PIM). Разные экземпляры представляют `privilegedAccess` различные поставщики, управляемые PIM. Например, `privilegedAccess/azureResources` PIM управляет привилегированным доступом к ресурсам Azure.


`privilegedAccess` пока доступен только для чтения. В `POST`наборе `PATCH``PUT`сущностей `DELETE` `privilegedAccess` не поддерживаются операции, а также операции.

## <a name="properties"></a>Свойства
| Свойство  | Тип      |Описание|
|:----------|:----------|:----------|
|id         |String     |Идентификатор поставщика, управляемого PIM.|
|displayName|String     |Отображаемое имя поставщика, управляемого PIM.|


## <a name="relationships"></a>Связи
| Связь   | Тип                                         |Описание|
|:---------------|:---------------------------------------------|:----------|
|resources       |[Коллекция governanceResource](../resources/governanceresource.md)            |Коллекция ресурсов для поставщика.|
|roleAssignments |[Коллекция governanceRoleAssignment](../resources/governanceroleassignment.md)|Коллекция назначений ролей для поставщика.|
|roleDefinitions |[Коллекция governanceRoleDefinition](../resources/governanceroledefinition.md)|Коллекция назначений ролей для поставщика.|
|roleAssignmentRequests |[Коллекция governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Коллекция запросов на назначение ролей для поставщика.|
|roleSettings |[Коллекция governanceRoleSetting](../resources/governancerolesetting.md)|Коллекция параметров роли для поставщика.|


## <a name="json-representation"></a>Представление в формате JSON

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


