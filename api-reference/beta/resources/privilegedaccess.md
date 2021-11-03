---
title: тип ресурса privilegedAccess
description: " например, представляет собой управление привилегированным доступом PIM к ресурсам `privilegedAccess/azureResources` Azure."
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: 9f7bf8f06ae75bd082664b5efad3e5ca9c46b70e
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696954"
---
# <a name="privilegedaccess-resource-type"></a>тип ресурса privilegedAccess

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет группу функциональных возможностей, предоставляемых службой управление привилегированными пользователями (PIM). Различные экземпляры представляют различных поставщиков, управляемых `privilegedAccess` PIM; например, представляет PIM, управляющую привилегированным доступом `privilegedAccess/azureResources` к ресурсам Azure.


`privilegedAccess` только для чтения на данный момент. Нет `POST` , или операции `PUT` `PATCH` `DELETE` поддерживаются в `privilegedAccess` наборе сущности.

## <a name="properties"></a>Свойства
| Свойство  | Тип      |Описание|
|:----------|:----------|:----------|
|id         |String     |ID поставщика, управляемого PIM.|
|displayName|String     |Отображает имя поставщика, управляемого PIM.|


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


