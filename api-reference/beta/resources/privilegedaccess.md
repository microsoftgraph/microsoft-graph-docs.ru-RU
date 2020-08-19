---
title: Тип ресурса Привилежедакцесс
description: " Например, `privilegedAccess/azureResources` представляет PIM управление привилегированным доступом к ресурсам Azure."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: shauliu
ms.openlocfilehash: c57dd911d105ba4d096a09f9262b847db5240fa1
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/19/2020
ms.locfileid: "46811454"
---
# <a name="privilegedaccess-resource-type"></a>Тип ресурса Привилежедакцесс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет группу функциональных возможностей, предоставляемых службой управления привилегированными удостоверениями (PIM). Различные экземпляры `privilegedAccess` представляют разных поставщиков, УПРАВЛЯЕМЫХ PIM; например, `privilegedAccess/azureResources` представляет PIM управление привилегированным доступом к ресурсам Azure.


`privilegedAccess` в настоящее время доступен только для чтения. `POST` `PUT` `PATCH` `DELETE` В наборе сущностей поддерживаются не поддерживаемые операции, а также операции `privilegedAccess` .

## <a name="properties"></a>Свойства
| Свойство  | Тип      |Описание|
|:----------|:----------|:----------|
|id         |String     |Идентификатор поставщика, управляемого службой PIM.|
|displayName|String     |Отображаемое имя поставщика, управляемого службой PIM.|


## <a name="relationships"></a>Отношения
| Связь   | Тип                                         |Описание|
|:---------------|:---------------------------------------------|:----------|
|resources       |Коллекция [governanceResource](../resources/governanceresource.md)            |Коллекция ресурсов для поставщика.|
|roleAssignments |Коллекция [governanceRoleAssignment](../resources/governanceroleassignment.md)|Коллекция назначений ролей для поставщика.|
|roleDefinitions |Коллекция [говернанцероледефинитион](../resources/governanceroledefinition.md)|Коллекция ролей дефинтионс для поставщика.|
|ролеассигнментрекуестс |Коллекция [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Коллекция запросов назначений ролей для поставщика.|
|ролесеттингс |Коллекция [говернанцеролесеттинг](../resources/governancerolesetting.md)|Коллекция параметров роли для поставщика.|


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
