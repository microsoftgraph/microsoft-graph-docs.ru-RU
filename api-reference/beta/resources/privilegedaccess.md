---
title: Тип ресурса Привилежедакцесс
description: " Например, `privilegedAccess/azureResources` представляет PIM управление привилегированным доступом к ресурсам Azure."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 1c8388c8ba9fd79b44e0d037496313cf67774bdf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521560"
---
# <a name="privilegedaccess-resource-type"></a>Тип ресурса Привилежедакцесс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет группу функциональных возможностей, предоставляемых службой управления привилегированными удостоверениями (PIM). Различные экземпляры `privilegedAccess` представляют разных поставщиков, УПРАВЛЯЕМЫХ службой PIM; Например, `privilegedAccess/azureResources` представляет PIM управление привилегированным доступом к ресурсам Azure.


`privilegedAccess`в настоящее время доступен только для чтения. `PUT` `POST` `privilegedAccess` В наборе сущностей `DELETE` поддерживаются не поддерживаемые операции, а также операции. `PATCH`

## <a name="properties"></a>Свойства
| Свойство  | Тип      |Описание|
|:----------|:----------|:----------|
|id         |String     |Идентификатор поставщика, управляемого службой PIM.|
|displayName|Строка     |Отображаемое имя поставщика, управляемого службой PIM.|


## <a name="relationships"></a>Связи
| Связь   | Тип                                         |Описание|
|:---------------|:---------------------------------------------|:----------|
|resources       |Коллекция [governanceResource](../resources/governanceresource.md)            |Коллекция ресурсов для поставщика.|
|roleAssignments |Коллекция [governanceRoleAssignment](../resources/governanceroleassignment.md)|Коллекция назначений ролей для поставщика.|
|roleDefinitions |Коллекция [говернанцероледефинитион](../resources/governanceroledefinition.md)|Коллекция ролей дефинтионс для поставщика.|
|ролеассигнментрекуестс |Коллекция [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)|Коллекция запросов назначений ролей для поставщика.|
|ролесеттингс |Коллекция [говернанцеролесеттинг](../resources/governancerolesetting.md)|Коллекция параметров роли для поставщика.|


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
