---
title: Тип ресурса accessPackageAssignmentResourceRole
description: Роль ресурса назначения пакета доступа указывает роль, относяющуюся к ресурсу, которая была назначена субъекту посредством назначения пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2b4893d40db8b5ac70a2ac3093d8dfbdf55c3175
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155603"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a>Тип ресурса accessPackageAssignmentResourceRole

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [управлении правами Azure AD](entitlementmanagement-root.md)роль ресурса назначения пакета доступа указывает роль, относяющуюся к ресурсу, которой субъект был назначен посредством назначения пакета доступа.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Get accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)  | Извлечение объекта accessPackageAssignmentResourceRole. |
| [Список accessPackageAssignmentResourceRoles](../api/accesspackageassignmentresourcerole-list.md) | [Коллекция accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) | Получить список объектов accessPackageAssignmentResourceRole. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Только для чтения.|
|originId|String|Уникальный идентификатор относительно системы источника, соответствующий свойству originId [объекта accessPackageResourceRole.](accesspackageresourcerole.md) |
|originSystem|String|Система, в которой должно быть создано назначение роли или создано для назначения пакета доступа, например , или ,, соответствующие свойству `SharePointOnline` `AadGroup` `AadApplication` originSystem [accessPackageResourceRole](accesspackageresourcerole.md).|
|status|String|Значением является то, когда назначение пакета доступа еще не было доставлено в систему источника и когда назначение пакета доступа было доставлено в систему `PendingFulfillment` `Fulfilled` источника.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackageAssignments|[Коллекция accessPackageAssignment](accesspackageassignment.md)| Назначения пакета доступа, в результате чего это назначение роли. Только для чтения. Допускается значение null.|
|accessPackageResourceRole|[accessPackageResourceRole](accesspackageresourcerole.md)| Только для чтения. Допускается значение null.|
|accessPackageResourceScope|[accessPackageResourceScope](accesspackageresourcescope.md)| Только для чтения. Допускается значение null.|
|accessPackageSubject|[accessPackageSubject](accesspackagesubject.md)| Только для чтения. Допускается значение null.|


## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "originId": "String",
  "originSystem": "String",
  "status": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignmentResourceRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


