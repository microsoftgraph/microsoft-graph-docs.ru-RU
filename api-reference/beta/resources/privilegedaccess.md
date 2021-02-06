---
title: Тип ресурса privilegedAccess
description: " например, `privilegedAccess/azureResources` представляет PIM, управляющее привилегированным доступом к ресурсам Azure."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 8a144ba13974a728b4e89fc661f34f20e8157689
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136621"
---
# <a name="privilegedaccess-resource-type"></a>Тип ресурса privilegedAccess

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет группу функций, предоставляемых службой Privileged Identity Management (PIM). Разные экземпляры представляют различных поставщиков, управляемых `privilegedAccess` PIM; например, представляет PIM, управляющую привилегированным доступом `privilegedAccess/azureResources` к ресурсам Azure.


`privilegedAccess` в настоящее время находится только для чтения. Нет, не поддерживаются операции или `POST` операции для `PUT` набора `PATCH` `DELETE` `privilegedAccess` суностей.

## <a name="properties"></a>Свойства
| Свойство  | Тип      |Описание|
|:----------|:----------|:----------|
|id         |Строка     |ИД поставщика, управляемого PIM.|
|displayName|Строка     |Отображаемого имени поставщика, управляемого PIM.|


## <a name="relationships"></a>Связи
| Связь   | Тип                                         |Описание|
|:---------------|:---------------------------------------------|:----------|
|resources       |[коллекция governanceResource](../resources/governanceresource.md)            |Коллекция ресурсов для поставщика.|
|roleAssignments |[Коллекция governanceRoleAssignment](../resources/governanceroleassignment.md)|Коллекция назначений ролей для поставщика.|
|roleDefinitions |[Коллекция governanceRoleDefinition](../resources/governanceroledefinition.md)|Коллекция отозванных ролей для поставщика.|
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


