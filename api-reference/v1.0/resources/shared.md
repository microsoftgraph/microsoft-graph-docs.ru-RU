---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Shared
ms.openlocfilehash: 1d828310a226edd0443ff3b5f60156df1e7c98cb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="shared-resource-type"></a><span data-ttu-id="fe8b0-102">Тип ресурса Shared</span><span class="sxs-lookup"><span data-stu-id="fe8b0-102">Shared resource type</span></span>

<span data-ttu-id="fe8b0-103">Ресурс **Shared** указывает, что к элементу DriveItem был предоставлен доступ другим пользователям.</span><span class="sxs-lookup"><span data-stu-id="fe8b0-103">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>
<span data-ttu-id="fe8b0-104">Ресурс содержит сведения о способе предоставления совместного доступа к элементу.</span><span class="sxs-lookup"><span data-stu-id="fe8b0-104">The Shared resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="fe8b0-105">Если у элемента [**Driveitem**](driveitem.md) есть аспект **shared**, имеющий значение, отличное от null, это значит, что к элементу предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="fe8b0-105">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe8b0-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fe8b0-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="fe8b0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe8b0-107">Properties</span></span>

| <span data-ttu-id="fe8b0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe8b0-108">Property</span></span>       | <span data-ttu-id="fe8b0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fe8b0-109">Type</span></span>                          | <span data-ttu-id="fe8b0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fe8b0-110">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="fe8b0-111">owner</span><span class="sxs-lookup"><span data-stu-id="fe8b0-111">owner</span></span>          | [<span data-ttu-id="fe8b0-112">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="fe8b0-112">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="fe8b0-p102">Удостоверение владельца общего элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe8b0-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="fe8b0-115">scope</span><span class="sxs-lookup"><span data-stu-id="fe8b0-115">scope</span></span>          | <span data-ttu-id="fe8b0-116">Строка</span><span class="sxs-lookup"><span data-stu-id="fe8b0-116">String</span></span>                        | <span data-ttu-id="fe8b0-117">Указывает область, в рамках которой предоставлен доступ к общему элементу: `anonymous`, `organization` или `users`.</span><span class="sxs-lookup"><span data-stu-id="fe8b0-117">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`.</span></span> <span data-ttu-id="fe8b0-118">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe8b0-118">Read-only.</span></span>
| <span data-ttu-id="fe8b0-119">sharedBy</span><span class="sxs-lookup"><span data-stu-id="fe8b0-119">sharedBy</span></span>       | [<span data-ttu-id="fe8b0-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="fe8b0-120">identitySet</span></span>](identityset.md) | <span data-ttu-id="fe8b0-p104">Удостоверение пользователя, предоставившего общий доступ к элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe8b0-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="fe8b0-123">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe8b0-123">sharedDateTime</span></span> | <span data-ttu-id="fe8b0-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe8b0-124">DateTimeOffset</span></span>                | <span data-ttu-id="fe8b0-p105">Дата и время предоставления общего доступа к элементу в формате UTC. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe8b0-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-values"></a><span data-ttu-id="fe8b0-127">Значения областей</span><span class="sxs-lookup"><span data-stu-id="fe8b0-127">Scope values</span></span>

| <span data-ttu-id="fe8b0-128">Значение</span><span class="sxs-lookup"><span data-stu-id="fe8b0-128">Value</span></span>          | <span data-ttu-id="fe8b0-129">Описание</span><span class="sxs-lookup"><span data-stu-id="fe8b0-129">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="fe8b0-130">Доступ к элементу предоставляется с помощью ссылки. Любой пользователь, у которого есть такая ссылка, может получить доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="fe8b0-130">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="fe8b0-131">Доступ к элементу предоставляется с помощью ссылки. Любой пользователь в организации владельца элемента, располагающий такой ссылкой, может получить доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="fe8b0-131">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="fe8b0-132">Доступ к элементу предоставляется только определенным пользователям.</span><span class="sxs-lookup"><span data-stu-id="fe8b0-132">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="fe8b0-133">Заметки</span><span class="sxs-lookup"><span data-stu-id="fe8b0-133">Remarks</span></span>

<span data-ttu-id="fe8b0-134">Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="fe8b0-134">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared"
} -->
