---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Shared
localization_priority: Normal
ms.openlocfilehash: 33b12ea8e530fd862619c9c20e77a76989efb619
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507700"
---
# <a name="shared-resource-type"></a>Тип ресурса Shared

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс Shared указывает, что к элементу DriveItem был предоставлен доступ другим пользователям. Ресурс содержит сведения о способе предоставления совместного доступа к элементу.

Если у элемента [**Driveitem**](driveitem.md) есть аспект **shared**, имеющий значение, отличное от null, это значит, что к элементу предоставлен общий доступ.

## <a name="json-representation"></a>Представление в формате JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.shared",
  "optionalProperties": [ "sharedBy", "sharedDateTime" ]
}-->

```json
{
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "scope": "anonymous | organization | users",
  "sharedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "sharedDateTime": "datetime"
}
```

## <a name="properties"></a>Свойства

| Свойство       | Тип                          | Описание
| :------------- |:------------------------------|:----------------------------
| owner          | [IdentitySet](identityset.md) | Удостоверение владельца общего элемента. Только для чтения.
| scope          | Строка                        | Указывает область, в рамках которой предоставлен доступ к общему элементу: `anonymous`, `organization` или `users`. Только для чтения.
| sharedBy       | [identitySet](identityset.md) | Удостоверение пользователя, предоставившего общий доступ к элементу. Только для чтения.
| sharedDateTime | DateTimeOffset                | Дата и время предоставления общего доступа к элементу в формате UTC. Только для чтения.

## <a name="scope-values"></a>Значения областей

| Значение          | Описание                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | Доступ к элементу предоставляется с помощью ссылки. Любой пользователь, у которого есть такая ссылка, может получить доступ к элементу.               |
| `organization` | Доступ к элементу предоставляется с помощью ссылки. Любой пользователь в организации владельца элемента, располагающий такой ссылкой, может получить доступ к элементу. |
| `users`        | Доступ к элементу предоставляется только определенным пользователям.                                          |

## <a name="remarks"></a>Заметки

Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [**driveItem**](driveitem.md).

<!--
{
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared",
  "suppressions": [
    "Error: /api-reference/beta/resources/shared.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
