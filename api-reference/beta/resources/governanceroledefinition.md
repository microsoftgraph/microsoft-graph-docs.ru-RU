---
title: Тип ресурса Говернанцероледефинитион
description: Представляет определения ролей. Для ресурсов Azure он может представлять роли Azure RBAC, такие как Owner, Reader, корреспондент и т. д.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: b6ff2edcfd1725b31051d1fc73c04539acf73e56
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217927"
---
# <a name="governanceroledefinition-resource-type"></a>Тип ресурса Говернанцероледефинитион

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Представляет определения ролей. Для ресурсов Azure он может представлять роли Azure RBAC, такие как Owner, Reader, корреспондент и т. д.


## <a name="methods"></a>Методы

| Метод          | Возвращаемый тип |Описание|
|:---------------|:--------|:--------|
|[List](../api/governanceroledefinition-list.md) | Коллекция [говернанцероледефинитион](../resources/governanceroledefinition.md) |Перечисление коллекции определений ролей для ресурса.|
|[получение](../api/governanceroledefinition-get.md); | [governanceRoleDefinition](../resources/governanceroledefinition.md) |Считывание свойств и связей объекта определения роли, указанного по идентификатору.|

Нет `POST`, `PUT`, `PATCH`, `DELETE` поддерживается в `roleDefinitions` наборе сущностей для Now.

## <a name="properties"></a>Свойства
| Свойство  | Тип      |Описание|
|:----|:----------|:----------|:----------|
|id         |Строка     |Идентификатор определения роли. |
|resourceId |String     |Обязательный. Идентификатор ресурса, связанного с определением роли. |
|externalId   |String     |Внешний идентификатор определения роли.|
|displayName|Строка     |Отображаемое имя определения роли.|
|templateId | Строка | |

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
