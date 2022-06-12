---
author: JeremyKelley
title: Тип общего ресурса
ms.localizationpriority: medium
description: Общий ресурс указывает, что driveItem был предоставлен другим пользователям.
ms.prod: files
doc_type: resourcePageType
ms.openlocfilehash: 7dc698106ffcb619e9e5e8e28845841084f59702
ms.sourcegitcommit: 423e698a580c3b902f2816b0216ab9d5b91e6d20
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2022
ms.locfileid: "66034392"
---
# <a name="shared-resource-type"></a>Тип общего ресурса

Пространство имен: microsoft.graph

Общий **ресурс** указывает, что **driveItem** был предоставлен другим пользователям.
Ресурс содержит сведения о способе предоставления совместного доступа к элементу.

Если у [**элемента driveitem**](driveitem.md) есть общий аспект, отличный от **NULL,** элемент является общим.

## <a name="json-representation"></a>Представление JSON

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

## <a name="scope-options"></a>Параметры области

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

