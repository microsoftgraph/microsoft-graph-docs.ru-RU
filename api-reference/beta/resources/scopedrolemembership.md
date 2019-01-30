---
title: Тип ресурса scopedRoleMembership
description: Членство в пределах роли описывает принадлежности пользователя к роли каталога, с дальнейшей областью действия, чтобы административные единицы (AU).  Это обеспечивает механизм, позволяющий adminsistrator клиента всей компании делегировать административные полномочия для пользователя для управления пользователями и группами в подмножества организации (подмножество, определяемым AU).
localization_priority: Normal
ms.openlocfilehash: 2d51ad696487e7daafb9b0f4fcef0934e4f6d6e2
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640793"
---
# <a name="scopedrolemembership-resource-type"></a>Тип ресурса scopedRoleMembership

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Членство в пределах роли описывает принадлежности пользователя к роли каталога, с дальнейшей областью действия, чтобы административные единицы (AU).  Это обеспечивает механизм, позволяющий adminsistrator клиента всей компании делегировать административные полномочия для пользователя для управления пользователями и группами в подмножества организации (подмножество, определяемым AU).

## <a name="methods"></a>Методы
Прямые запросы для этого ресурса не поддерживаются.  Ознакомьтесь с [единицы администрирования](administrativeunit.md) раздел для просмотра сведений о том, как для запроса областью действия роли участие в группах, а также добавление и удаление членство областью действия роли. 

## <a name="properties"></a>Свойства
| Свойство   | Тип | Описание |
|:---------------|:--------|:----------|
|administrativeUnitId|строка|Уникальный идентификатор административного подразделения, пределах роли каталога|
|id|строка| Уникальный идентификатор для членство в области определения роли. Только для чтения.|
|roleId|строка| Уникальный идентификатор для роли каталога, элемент.|
|roleMemberInfo|[identity](identity.md)| Сведения о удостоверение члена роли. Представляет пользователя, который является членом этой области определения роли.|

## <a name="relationships"></a>Связи
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
