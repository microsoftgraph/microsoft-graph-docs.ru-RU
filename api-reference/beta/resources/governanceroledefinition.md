---
title: тип ресурса governanceRoleDefinition
description: Представляет определения ролей. Для ресурсов Azure он может представлять роли Azure RBAC, такие как Owner, Reader, Contributor и т.д.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: japere
ms.openlocfilehash: 631640b8187b2fae87b28fcd6cd1b1b9b57a9bb5
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510557"
---
# <a name="governanceroledefinition-resource-type"></a>тип ресурса governanceRoleDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]


Представляет определения ролей. Для ресурсов Azure он может представлять роли Azure RBAC, такие как Owner, Reader, Contributor и т.д.


## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:---------------|:--------|:--------|
|[Список](../api/governanceroledefinition-list.md) | [коллекция governanceRoleDefinition](../resources/governanceroledefinition.md) |Список коллекции определений ролей на ресурсе.|
|[Получение](../api/governanceroledefinition-get.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) |Чтение свойств и связей сущности определения роли, указанной в id.|

Нет`POST`, `PUT`поддерживается `DELETE` `PATCH`в наборе `roleDefinitions` сущности на данный момент.

## <a name="properties"></a>Свойства
| Свойство    | Тип   | Описание                                                           |
|:------------|:-------|:----------------------------------------------------------------------|
| id          | Строка | ID определения роли.                                        |
| resourceId  | String | Обязательный. ID ресурса, связанного с определением роли. |
| externalId  | String | Внешний id определения роли.                               |
| displayName | Строка | Отображение имени определения роли.                              |
| templateId  | Строка |                                                                       |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resource|[governanceResource](../resources/governanceresource.md)|Только для чтения. Связанный ресурс для определения роли.|
|roleSetting|[governanceRoleSetting](../resources/governancerolesetting.md)|Связанный параметр роли для определения роли.|

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "externalId": "String",
  "displayName": "String",
  "templateId":"String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


