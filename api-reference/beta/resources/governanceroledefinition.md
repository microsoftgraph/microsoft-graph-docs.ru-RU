---
title: Тип ресурса governanceRoleDefinition
description: Представляет определения ролей. Для ресурсов Azure он может представлять роли RBAC Azure, такие как владелец, читатель, участник и т. д.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 5cbb9cb86664407018237def427381610d898ff5
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398828"
---
# <a name="governanceroledefinition-resource-type"></a>Тип ресурса governanceRoleDefinition

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]


Представляет определения ролей. Для ресурсов Azure он может представлять роли RBAC Azure, такие как владелец, читатель, участник и т. д.


## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:---------------|:--------|:--------|
|[Перечисление](../api/governanceroledefinition-list.md) | [Коллекция governanceRoleDefinition](../resources/governanceroledefinition.md) |Вывод списка определений ролей для ресурса.|
|[Получение](../api/governanceroledefinition-get.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) |Чтение свойств и связей сущности определения роли, указанной идентификатором.|

Нет `POST`, `PUT`, `PATCH`поддерживается `DELETE` для набора `roleDefinitions` сущностей на данный момент.

## <a name="properties"></a>Свойства
| Свойство    | Тип   | Описание                                                           |
|:------------|:-------|:----------------------------------------------------------------------|
| id          | String | Идентификатор определения роли.                                        |
| resourceId  | String | Обязательный. Идентификатор ресурса, связанного с определением роли. |
| externalId  | String | Внешний идентификатор определения роли.                               |
| displayName | String | Отображаемое имя определения роли.                              |
| templateId  | String |                                                                       |

## <a name="relationships"></a>Связи
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resource|[governanceResource](../resources/governanceresource.md)|Только для чтения. Связанный ресурс для определения роли.|
|roleSetting|[governanceRoleSetting](../resources/governancerolesetting.md)|Параметр связанной роли для определения роли.|

## <a name="json-representation"></a>Представление в формате JSON

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


