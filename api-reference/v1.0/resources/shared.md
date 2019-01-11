---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Shared
localization_priority: Normal
ms.openlocfilehash: 3478a8911a402bf86a04f196d87409e7cddb246e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868077"
---
# <a name="shared-resource-type"></a><span data-ttu-id="18577-102">Тип ресурса Shared</span><span class="sxs-lookup"><span data-stu-id="18577-102">Shared resource type</span></span>

<span data-ttu-id="18577-p101">Ресурс **Shared** указывает, что к элементу DriveItem был предоставлен доступ другим пользователям. Ресурс содержит сведения о способе предоставления совместного доступа к элементу.</span><span class="sxs-lookup"><span data-stu-id="18577-p101">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="18577-105">Если у элемента [**Driveitem**](driveitem.md) есть аспект **shared**, имеющий значение, отличное от null, это значит, что к элементу предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="18577-105">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="18577-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="18577-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="18577-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="18577-107">Properties</span></span>

| <span data-ttu-id="18577-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="18577-108">Property</span></span>       | <span data-ttu-id="18577-109">Тип</span><span class="sxs-lookup"><span data-stu-id="18577-109">Type</span></span>                          | <span data-ttu-id="18577-110">Описание</span><span class="sxs-lookup"><span data-stu-id="18577-110">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="18577-111">owner</span><span class="sxs-lookup"><span data-stu-id="18577-111">owner</span></span>          | [<span data-ttu-id="18577-112">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="18577-112">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="18577-p102">Удостоверение владельца общего элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18577-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="18577-115">scope</span><span class="sxs-lookup"><span data-stu-id="18577-115">scope</span></span>          | <span data-ttu-id="18577-116">Строка</span><span class="sxs-lookup"><span data-stu-id="18577-116">String</span></span>                        | <span data-ttu-id="18577-p103">Указывает область, в рамках которой предоставлен доступ к общему элементу: `anonymous`, `organization` или `users`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18577-p103">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="18577-119">sharedBy</span><span class="sxs-lookup"><span data-stu-id="18577-119">sharedBy</span></span>       | [<span data-ttu-id="18577-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="18577-120">identitySet</span></span>](identityset.md) | <span data-ttu-id="18577-p104">Удостоверение пользователя, предоставившего общий доступ к элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18577-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="18577-123">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="18577-123">sharedDateTime</span></span> | <span data-ttu-id="18577-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="18577-124">DateTimeOffset</span></span>                | <span data-ttu-id="18577-p105">Дата и время предоставления общего доступа к элементу в формате UTC. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="18577-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-options"></a><span data-ttu-id="18577-127">Параметры области</span><span class="sxs-lookup"><span data-stu-id="18577-127">Scope options</span></span>

| <span data-ttu-id="18577-128">Значение</span><span class="sxs-lookup"><span data-stu-id="18577-128">Value</span></span>          | <span data-ttu-id="18577-129">Описание</span><span class="sxs-lookup"><span data-stu-id="18577-129">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="18577-130">Доступ к элементу предоставляется с помощью ссылки. Любой пользователь, у которого есть такая ссылка, может получить доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="18577-130">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="18577-131">Доступ к элементу предоставляется с помощью ссылки. Любой пользователь в организации владельца элемента, располагающий такой ссылкой, может получить доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="18577-131">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="18577-132">Доступ к элементу предоставляется только определенным пользователям.</span><span class="sxs-lookup"><span data-stu-id="18577-132">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="18577-133">Заметки</span><span class="sxs-lookup"><span data-stu-id="18577-133">Remarks</span></span>

<span data-ttu-id="18577-134">Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="18577-134">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

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
