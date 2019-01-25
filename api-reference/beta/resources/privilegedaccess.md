---
title: Тип ресурса privilegedAccess
description: " например `privilegedAccess/azureResources` представляет PIM управление правами доступа к ресурсам Azure."
localization_priority: Normal
ms.openlocfilehash: 9ac8ab596906509bc0303f9a70794b6484759cc2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512929"
---
# <a name="privilegedaccess-resource-type"></a>Тип ресурса privilegedAccess

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет группу функциональные возможности службы управления правами Identity (PIM). Различных экземпляров `privilegedAccess` представляют различных поставщиков, управляется PIM; например `privilegedAccess/azureResources` представляет PIM управление правами доступа к ресурсам Azure.


`privilegedAccess`доступно только для чтения в данный момент. Не `POST`, `PUT`, `PATCH`, или `DELETE` поддерживается на `privilegedAccess` набора сущностей.

## <a name="properties"></a>Свойства
| Свойство  | Тип      |Описание|
|:----------|:----------|:----------|
|id         |String     |Идентификатор поставщика, управляется PIM.|
|displayName|String     |Отображаемое имя поставщика, управляется PIM.|


## <a name="relationships"></a>Отношения
| Связь   | Тип                                         |Описание|
|:---------------|:---------------------------------------------|:----------|
|resources       |[governanceResource](../resources/governanceresource.md) коллекции            |Набор ресурсов для поставщика.|
|roleAssignments |[governanceRoleAssignment](../resources/governanceroleassignment.md) коллекции|Коллекция назначения ролей для поставщика.|
|roleDefinitions |[governanceRoleDefinition](../resources/governanceroledefinition.md) коллекции|Коллекция файлов определения ролей для поставщика.|
|roleAssignmentRequests |[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md) коллекции|Коллекция запросы назначения ролей для поставщика.|
|roleSettings |[governanceRoleSetting](../resources/governancerolesetting.md) коллекции|Коллекция параметров роли для поставщика.|


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
