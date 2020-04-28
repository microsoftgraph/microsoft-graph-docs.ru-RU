---
title: Тип ресурса Scopedrolemembership изменен
description: Членство в роли с областью описывает членство пользователя в роли каталога, для которого применяется административная единица (AU).  Это обеспечивает механизм, позволяющий компании, админсистратор на уровне клиента, делегировать административные привилегии пользователю для управления пользователями и группами в подмножестве Организации (подмножества, определяемого службой автоматического управления).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d5448db2bb73146b3f3e435376ea7b5d708f0474
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520944"
---
# <a name="scopedrolemembership-resource-type"></a>Тип ресурса Scopedrolemembership изменен

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Членство в роли с областью описывает членство пользователя в роли каталога, для которого применяется административная единица (AU).  Это обеспечивает механизм, позволяющий компании, админсистратор на уровне клиента, делегировать административные привилегии пользователю для управления пользователями и группами в подмножестве Организации (подмножества, определяемого службой автоматического управления).

## <a name="methods"></a>Methods
Прямые запросы к этому ресурсу не поддерживаются.  Ознакомьтесь с разделом [админстративе Units](administrativeunit.md) , чтобы узнать, как запрашивать участие в ролях для ролей, а также добавлять и удалять сведения об участии в ролях. 

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
