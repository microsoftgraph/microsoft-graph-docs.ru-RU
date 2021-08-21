---
title: тип ресурса governanceRoleDefinition
description: Представляет определения ролей. Для ресурсов Azure он может представлять роли Azure RBAC, такие как Owner, Reader, Contributor и т.д.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu1
ms.openlocfilehash: 4f0144f4d26c8440b4e2bdc0965e88310a4f9145
ms.sourcegitcommit: 01755ac7c0ab7becf28052e05e58567caa8364cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/21/2021
ms.locfileid: "58453725"
---
# <a name="governanceroledefinition-resource-type"></a>тип ресурса governanceRoleDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Представляет определения ролей. Для ресурсов Azure он может представлять роли Azure RBAC, такие как Owner, Reader, Contributor и т.д.


## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:---------------|:--------|:--------|
|[Список](../api/governanceroledefinition-list.md) | [коллекция governanceRoleDefinition](../resources/governanceroledefinition.md) |Список коллекции определений ролей на ресурсе.|
|[получение](../api/governanceroledefinition-get.md); | [governanceRoleDefinition](../resources/governanceroledefinition.md) |Чтение свойств и связей сущности определения роли, указанной в id.|

`POST`Нет, `PUT` `PATCH` `DELETE` поддерживается в `roleDefinitions` наборе сущности на данный момент.

## <a name="properties"></a>Свойства
| Свойство    | Тип   | Описание                                                           |
|:------------|:-------|:----------------------------------------------------------------------|
| id          | String | ID определения роли.                                        |
| resourceId  | String | Обязательный. ID ресурса, связанного с определением роли. |
| externalId  | String | Внешний id определения роли.                               |
| displayName | String | Отображение имени определения роли.                              |
| templateId  | String |                                                                       |

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


