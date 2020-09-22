---
title: Тип ресурса Scopedrolemembership изменен
description: Членство в роли с областью описывает членство пользователя в роли каталога, для которого применяется административная единица (AU).  Это обеспечивает механизм, позволяющий компании, админсистратор на уровне клиента, делегировать административные привилегии пользователю для управления пользователями и группами в подмножестве Организации (подмножества, определяемого службой автоматического управления).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: abhijeetsinha
ms.openlocfilehash: 47d4ee4fb481b46631c83efe952c3cf3a9c5f7b5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47990478"
---
# <a name="scopedrolemembership-resource-type"></a>Тип ресурса Scopedrolemembership изменен

Пространство имен: microsoft.graph

Членство в роли с областью описывает членство пользователя в роли каталога, для которого применяется административная единица (AU).  Это предоставляет механизм, позволяющий администратору компании на уровне клиента делегировать административные права пользователю для управления пользователями и группами в подмножестве Организации (подмножества, определяемого службой автоматического управления).

## <a name="methods"></a>Методы
Прямые запросы к этому ресурсу не поддерживаются.  В разделе " [административные единицы](administrativeunit.md) " представлены сведения о том, как запрашивать сведения о членстве в пределах ролей, а также добавлять и удалять членство в ролях.

## <a name="properties"></a>Свойства
| Свойство   | Тип | Описание |
|:---------------|:--------|:----------|
|административеунитид|string|Уникальный идентификатор административной единицы, на которую распространяется роль каталога|
|id|string| Уникальный идентификатор для членства в пределах ролей. Только для чтения.|
|roleId|string| Уникальный идентификатор роли каталога, в которой находится член.|
|roleMemberInfo|[identity](identity.md)| Сведения об удостоверении участника роли. Представляет пользователя, который является членом этой области с областью действия.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedRoleMembership"
}-->

```json
{
  "administrativeUnitId": "string",
  "id": "string (identifier)",
  "roleId": "string",
  "roleMemberInfo": {"@odata.type": "microsoft.graph.identity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
