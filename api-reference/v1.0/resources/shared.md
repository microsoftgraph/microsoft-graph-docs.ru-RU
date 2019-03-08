---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Shared
localization_priority: Normal
ms.openlocfilehash: af426d5e51f87b9fd8894c6e956947cc75f1a38d
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481799"
---
# <a name="shared-resource-type"></a><span data-ttu-id="6abc6-102">Тип ресурса Shared</span><span class="sxs-lookup"><span data-stu-id="6abc6-102">Shared resource type</span></span>

<span data-ttu-id="6abc6-p101">Ресурс **Shared** указывает, что к элементу DriveItem был предоставлен доступ другим пользователям. Ресурс содержит сведения о способе предоставления совместного доступа к элементу.</span><span class="sxs-lookup"><span data-stu-id="6abc6-p101">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="6abc6-105">Если у элемента [**Driveitem**](driveitem.md) есть аспект **shared**, имеющий значение, отличное от null, это значит, что к элементу предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="6abc6-105">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6abc6-106">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6abc6-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6abc6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6abc6-107">Properties</span></span>

| <span data-ttu-id="6abc6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6abc6-108">Property</span></span>       | <span data-ttu-id="6abc6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6abc6-109">Type</span></span>                          | <span data-ttu-id="6abc6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6abc6-110">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="6abc6-111">owner</span><span class="sxs-lookup"><span data-stu-id="6abc6-111">owner</span></span>          | [<span data-ttu-id="6abc6-112">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="6abc6-112">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="6abc6-p102">Удостоверение владельца общего элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6abc6-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="6abc6-115">scope</span><span class="sxs-lookup"><span data-stu-id="6abc6-115">scope</span></span>          | <span data-ttu-id="6abc6-116">String</span><span class="sxs-lookup"><span data-stu-id="6abc6-116">String</span></span>                        | <span data-ttu-id="6abc6-p103">Указывает область, в рамках которой предоставлен доступ к общему элементу: `anonymous`, `organization` или `users`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6abc6-p103">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="6abc6-119">sharedBy</span><span class="sxs-lookup"><span data-stu-id="6abc6-119">sharedBy</span></span>       | [<span data-ttu-id="6abc6-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="6abc6-120">identitySet</span></span>](identityset.md) | <span data-ttu-id="6abc6-p104">Удостоверение пользователя, предоставившего общий доступ к элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6abc6-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="6abc6-123">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="6abc6-123">sharedDateTime</span></span> | <span data-ttu-id="6abc6-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6abc6-124">DateTimeOffset</span></span>                | <span data-ttu-id="6abc6-p105">Дата и время предоставления общего доступа к элементу в формате UTC. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6abc6-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-options"></a><span data-ttu-id="6abc6-127">Параметры области</span><span class="sxs-lookup"><span data-stu-id="6abc6-127">Scope options</span></span>

| <span data-ttu-id="6abc6-128">Значение</span><span class="sxs-lookup"><span data-stu-id="6abc6-128">Value</span></span>          | <span data-ttu-id="6abc6-129">Описание</span><span class="sxs-lookup"><span data-stu-id="6abc6-129">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="6abc6-130">Доступ к элементу предоставляется с помощью ссылки. Любой пользователь, у которого есть такая ссылка, может получить доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="6abc6-130">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="6abc6-131">Доступ к элементу предоставляется с помощью ссылки. Любой пользователь в организации владельца элемента, располагающий такой ссылкой, может получить доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="6abc6-131">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="6abc6-132">Доступ к элементу предоставляется только определенным пользователям.</span><span class="sxs-lookup"><span data-stu-id="6abc6-132">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="6abc6-133">Заметки</span><span class="sxs-lookup"><span data-stu-id="6abc6-133">Remarks</span></span>

<span data-ttu-id="6abc6-134">Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="6abc6-134">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

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
