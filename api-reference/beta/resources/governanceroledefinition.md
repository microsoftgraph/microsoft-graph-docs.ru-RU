---
title: Тип ресурса Говернанцероледефинитион
description: Представляет определения ролей. Для ресурсов Azure он может представлять роли Azure RBAC, такие как Owner, Reader, корреспондент и т. д.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 1435e8326536aa1a8943e46799d6a5612485a425
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845745"
---
# <a name="governanceroledefinition-resource-type"></a>Тип ресурса Говернанцероледефинитион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Представляет определения ролей. Для ресурсов Azure он может представлять роли Azure RBAC, такие как Owner, Reader, корреспондент и т. д.


## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:---------------|:--------|:--------|
|[Список](../api/governanceroledefinition-list.md) | Коллекция [говернанцероледефинитион](../resources/governanceroledefinition.md) |Перечисление коллекции определений ролей для ресурса.|
|[получение](../api/governanceroledefinition-get.md); | [governanceRoleDefinition](../resources/governanceroledefinition.md) |Считывание свойств и связей объекта определения роли, указанного по идентификатору.|

Нет `POST` , `PUT` , `PATCH` , `DELETE` поддерживается в `roleDefinitions` наборе сущностей для Now.

## <a name="properties"></a>Свойства
| Свойство    | Тип   | Описание                                                           |
|:------------|:-------|:----------------------------------------------------------------------|
| id          | Строка | Идентификатор определения роли.                                        |
| resourceId  | String | Обязательный. Идентификатор ресурса, связанного с определением роли. |
| externalId  | String | Внешний идентификатор определения роли.                               |
| displayName | Строка | Отображаемое имя определения роли.                              |
| templateId  | String |                                                                       |

## <a name="relationships"></a>Отношения
| Связь | Тип   |Описание|
|:---------------|:--------|:----------|
|resource|[governanceResource](../resources/governanceresource.md)|Только для чтения. Связанный ресурс для определения роли.|
|ролесеттинг|[governanceRoleSetting](../resources/governancerolesetting.md)|Связанный параметр роли для определения роли.|

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
