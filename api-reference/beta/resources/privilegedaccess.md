---
title: Тип ресурса privilegedAccess
description: " например `privilegedAccess/azureResources` представляет PIM управление правами доступа к ресурсам Azure."
localization_priority: Normal
ms.openlocfilehash: f4166fb539d627730c68c7e039fd8d672ff4c785
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810054"
---
# <a name="privilegedaccess-resource-type"></a>Тип ресурса privilegedAccess

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Представляет группу функциональные возможности службы управления правами Identity (PIM). Различных экземпляров `privilegedAccess` представляют различных поставщиков, управляется PIM; например `privilegedAccess/azureResources` представляет PIM управление правами доступа к ресурсам Azure.


`privilegedAccess`доступно только для чтения в данный момент. Не `POST`, `PUT`, `PATCH`, или `DELETE` поддерживается на `privilegedAccess` набора сущностей.

## <a name="properties"></a>Свойства
| Свойство  | Тип      |Описание|
|:----------|:----------|:----------|
|id         |Строка     |Идентификатор поставщика, управляется PIM.|
|displayName|Строка     |Отображаемое имя поставщика, управляется PIM.|


## <a name="relationships"></a>Связи
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedAccess",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
