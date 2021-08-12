---
author: JeremyKelley
ms.date: 09/10/2017
title: Shared
localization_priority: Normal
description: Ресурс Shared указывает, что к элементу DriveItem был предоставлен доступ другим пользователям.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7dc4eb845b1458da996a0ccbd23724b502cd899c205dca4515183b74162c6f5b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251759"
---
# <a name="shared-resource-type"></a>Тип ресурса Shared

Пространство имен: microsoft.graph

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

## <a name="scope-options"></a>Параметры Области

| Значение          | Описание                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | Доступ к элементу предоставляется с помощью ссылки. Любой пользователь, у которого есть такая ссылка, может получить доступ к элементу.               |
| `organization` | Доступ к элементу предоставляется с помощью ссылки. Любой пользователь в организации владельца элемента, располагающий такой ссылкой, может получить доступ к элементу. |
| `users`        | Доступ к элементу предоставляется только определенным пользователям.                                          |

## <a name="remarks"></a>Заметки

Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [**driveItem**](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/shared.md:
      Found potential enums in resource example that weren't defined in a table:(anonymous,organization,users) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Shared"
} -->

