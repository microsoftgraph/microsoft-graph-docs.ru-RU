---
title: Тип ресурса scopedRoleMembership
description: Членство с ролью с областью действия описывает членство пользователя в роли каталога, которая дополнительно имеет область действия административной единицы (AU).  Это предоставляет механизм, позволяющий администратору компании на клиенте делегировать права администратора пользователю для управления пользователями и группами в подмножестве организаций (подмножество определяется au).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: abhijeetsinha
ms.openlocfilehash: ffd1e616d94ccf959b8535f46f79a2c7c57e00c2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134710"
---
# <a name="scopedrolemembership-resource-type"></a>Тип ресурса scopedRoleMembership

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Членство с ролью с областью действия описывает членство пользователя в роли каталога, которая дополнительно имеет область действия административной единицы (AU).  Это предоставляет механизм, позволяющий администратору компании на клиенте делегировать права администратора пользователю для управления пользователями и группами в подмножество организации (подмножество, определяемого au).

## <a name="methods"></a>Методы
Прямые запросы к этому ресурсу не поддерживаются.  См. [раздел](administrativeunit.md) об административных единицах, чтобы узнать, как запрашивать участие в роли с заданной областью, а также добавлять и удалять членство с ролью с заданной областью.

## <a name="properties"></a>Свойства
| Свойство   | Тип | Описание |
|:---------------|:--------|:----------|
|administrativeUnitId|string|Уникальный идентификатор административной единицы, областью действия роли каталога|
|id|string| Уникальный идентификатор членства с ролью с за областью действия. Только для чтения.|
|roleId|string| Уникальный идентификатор роли каталога, в котором находится участник.|
|roleMemberInfo|[identity](identity.md)| Сведения об удостоверении участника роли. Представляет пользователя, который является членом этой роли с заданной областью действия.|

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


