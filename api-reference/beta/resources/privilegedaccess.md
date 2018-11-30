---
title: Тип ресурса privilegedAccess
description: " например `privilegedAccess/azureResources` представляет PIM управление правами доступа к ресурсам Azure."
ms.openlocfilehash: af109c0cc355bfb282630d21cd02bb463b944f38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082437"
---
# <a name="privilegedaccess-resource-type"></a>Тип ресурса privilegedAccess

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет группу функциональные возможности службы управления правами Identity (PIM). Различных экземпляров `privilegedAccess` представляют различных поставщиков, управляется PIM; например `privilegedAccess/azureResources` представляет PIM управление правами доступа к ресурсам Azure.


`privilegedAccess`доступно только для чтения в данный момент. Не `POST`, `PUT`, `PATCH`, или `DELETE` поддерживается на `privilegedAccess` набора сущностей.

## <a name="properties"></a>Свойства
| Свойство  | Тип      |Описание|
|:----------|:----------|:----------|
|id         |String     |Идентификатор поставщика, управляется PIM.|
|displayName|String     |Отображаемое имя поставщика, управляется PIM.|


## <a name="relationships"></a>Связи
| Связь   | Тип                                         |Description|
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
