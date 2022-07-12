---
title: Shared
author: JeremyKelley
description: Ресурс Shared указывает, что к элементу DriveItem был предоставлен доступ другим пользователям.
ms.date: 09/10/2017
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: files
ms.openlocfilehash: f814ce4d6f395784c987da997e7a8b6f3f201b17
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66731920"
---
# <a name="shared-resource-type"></a>Тип ресурса Shared

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Ресурс **Shared** указывает, что к элементу DriveItem был предоставлен доступ другим пользователям. Ресурс содержит сведения о способе предоставления совместного доступа к элементу.

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
| scope          | String                        | Указывает область, в рамках которой предоставлен доступ к общему элементу: `anonymous`, `organization` или `users`. Только для чтения.
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
  "suppressions": []
}
-->


