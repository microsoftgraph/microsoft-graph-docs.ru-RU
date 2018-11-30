---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Shared
ms.openlocfilehash: 0a94a1d5ddf671151cf786d9ff93ae4f9e012a7b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026501"
---
# <a name="shared-resource-type"></a><span data-ttu-id="0165d-102">Тип ресурса Shared</span><span class="sxs-lookup"><span data-stu-id="0165d-102">Shared resource type</span></span>

<span data-ttu-id="0165d-p101">Ресурс **Shared** указывает, что к элементу DriveItem был предоставлен доступ другим пользователям. Ресурс содержит сведения о способе предоставления совместного доступа к элементу.</span><span class="sxs-lookup"><span data-stu-id="0165d-p101">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="0165d-105">Если у элемента [**Driveitem**](driveitem.md) есть аспект **shared**, имеющий значение, отличное от null, это значит, что к элементу предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="0165d-105">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0165d-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0165d-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="0165d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0165d-107">Properties</span></span>

| <span data-ttu-id="0165d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0165d-108">Property</span></span>       | <span data-ttu-id="0165d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0165d-109">Type</span></span>                          | <span data-ttu-id="0165d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0165d-110">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="0165d-111">owner</span><span class="sxs-lookup"><span data-stu-id="0165d-111">owner</span></span>          | [<span data-ttu-id="0165d-112">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="0165d-112">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="0165d-p102">Удостоверение владельца общего элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0165d-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="0165d-115">scope</span><span class="sxs-lookup"><span data-stu-id="0165d-115">scope</span></span>          | <span data-ttu-id="0165d-116">Строка</span><span class="sxs-lookup"><span data-stu-id="0165d-116">String</span></span>                        | <span data-ttu-id="0165d-p103">Указывает область, в рамках которой предоставлен доступ к общему элементу: `anonymous`, `organization` или `users`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0165d-p103">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="0165d-119">sharedBy</span><span class="sxs-lookup"><span data-stu-id="0165d-119">sharedBy</span></span>       | [<span data-ttu-id="0165d-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="0165d-120">identitySet</span></span>](identityset.md) | <span data-ttu-id="0165d-p104">Удостоверение пользователя, предоставившего общий доступ к элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0165d-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="0165d-123">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="0165d-123">sharedDateTime</span></span> | <span data-ttu-id="0165d-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0165d-124">DateTimeOffset</span></span>                | <span data-ttu-id="0165d-p105">Дата и время предоставления общего доступа к элементу в формате UTC. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0165d-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-options"></a><span data-ttu-id="0165d-127">Параметры области</span><span class="sxs-lookup"><span data-stu-id="0165d-127">Scope options</span></span>

| <span data-ttu-id="0165d-128">Значение</span><span class="sxs-lookup"><span data-stu-id="0165d-128">Value</span></span>          | <span data-ttu-id="0165d-129">Описание</span><span class="sxs-lookup"><span data-stu-id="0165d-129">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="0165d-130">Доступ к элементу предоставляется с помощью ссылки. Любой пользователь, у которого есть такая ссылка, может получить доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="0165d-130">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="0165d-131">Доступ к элементу предоставляется с помощью ссылки. Любой пользователь в организации владельца элемента, располагающий такой ссылкой, может получить доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="0165d-131">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="0165d-132">Доступ к элементу предоставляется только определенным пользователям.</span><span class="sxs-lookup"><span data-stu-id="0165d-132">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="0165d-133">Заметки</span><span class="sxs-lookup"><span data-stu-id="0165d-133">Remarks</span></span>

<span data-ttu-id="0165d-134">Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="0165d-134">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

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
