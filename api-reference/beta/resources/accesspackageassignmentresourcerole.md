---
title: тип ресурса accessPackageAssignmentResourceRole
description: Роль ресурса назначения пакета доступа указывает на роль, определенную для ресурса, которую субъекту было назначено с помощью назначения пакета доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4473c303a74cbf9e8e0c17d6c9060960590a3405
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433283"
---
# <a name="accesspackageassignmentresourcerole-resource-type"></a>тип ресурса accessPackageAssignmentResourceRole

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В управлении правами [Azure AD](entitlementmanagement-root.md)роль ресурса назначения пакета доступа указывает на роль, определенную для ресурса, которую субъекту было назначено с помощью назначения пакета доступа.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получите accessPackageAssignmentResourceRole](../api/accesspackageassignmentresourcerole-get.md) | [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)  | Извлечение объекта accessPackageAssignmentResourceRole. |
| [Список accessPackageAssignmentResourceRoles](../api/accesspackageassignmentresourcerole-list.md) | [коллекция accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md) | Извлечение списка объектов accessPackageAssignmentResourceRole. |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String| Только для чтения.|
|OriginId|String|Уникальный идентификатор относительно системы происхождения, соответствующий свойству originId [accessPackageResourceRole.](accesspackageresourcerole.md) |
|originSystem|String|Система, в которой назначение ролей должно быть создано или создано для назначения пакета доступа, например, или , соответствующего свойству `SharePointOnline` `AadGroup` `AadApplication` [originSystem accessPackageResourceRole.](accesspackageresourcerole.md)|
|status|String|Значение — когда назначение пакета доступа еще не доставлено в систему происхождения и когда назначение пакета доступа было доставлено в `PendingFulfillment` `Fulfilled` систему происхождения.|

## <a name="relationships"></a>Связи

| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|accessPackageAssignments|[коллекция accessPackageAssignment](accesspackageassignment.md)| Назначения пакета доступа, в результате чего это назначение роли. Только для чтения. Допускается значение null.|
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


