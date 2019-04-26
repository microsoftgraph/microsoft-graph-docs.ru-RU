---
title: Тип ресурса Scopedrolemembership изменен
description: Членство В роли С областью описывает членство пользователя в роли каталога, для которого применяется административная единица (AU).  Это обеспечивает механизм, позволяющий компании, админсистратор на уровне клиента, делегировать административные привилегии пользователю для управления пользователями и группами в подмножестве Организации (подмножества, определяемого службой автоматического управления).
localization_priority: Normal
ms.openlocfilehash: 2d51ad696487e7daafb9b0f4fcef0934e4f6d6e2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562981"
---
# <a name="scopedrolemembership-resource-type"></a>Тип ресурса Scopedrolemembership изменен

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Членство В роли С областью описывает членство пользователя в роли каталога, для которого применяется административная единица (AU).  Это обеспечивает механизм, позволяющий компании, админсистратор на уровне клиента, делегировать административные привилегии пользователю для управления пользователями и группами в подмножестве Организации (подмножества, определяемого службой автоматического управления).

## <a name="methods"></a>Методы
Прямые запросы к этому ресурсу не поддерживаются.  Ознакомьтесь с разделом [админстративе Units](administrativeunit.md) , чтобы узнать, как запрашивать участие в ролях для ролей, а также добавлять и удалять сведения об участии в ролях. 

## <a name="properties"></a>Свойства
| Свойство   | Тип | Описание |
|:---------------|:--------|:----------|
|Административеунитид|string|Уникальный идентификатор административной единицы, на которую распространяется роль каталога|
|id|string| Уникальный идентификатор для членства в пределах ролей. Только для чтения.|
|roleId|string| Уникальный идентификатор роли каталога, в которой находится член.|
|roleMemberInfo|[identity](identity.md)| Сведения об удостоверении участника роли. Представляет пользователя, который является членом этой области с областью действия.|

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedrolemembership"
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
  "suppressions": [
    "Error: /api-reference/beta/resources/scopedrolemembership.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
