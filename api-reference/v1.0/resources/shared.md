---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Shared
localization_priority: Normal
description: Ресурс Shared указывает, что к элементу DriveItem был предоставлен доступ другим пользователям.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9058b1e3f5f8dd77c22ee253746c7eba8c1df7c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009186"
---
# <a name="shared-resource-type"></a><span data-ttu-id="74ec5-103">Тип ресурса Shared</span><span class="sxs-lookup"><span data-stu-id="74ec5-103">Shared resource type</span></span>

<span data-ttu-id="74ec5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74ec5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="74ec5-p101">Ресурс **Shared** указывает, что к элементу DriveItem был предоставлен доступ другим пользователям. Ресурс содержит сведения о способе предоставления совместного доступа к элементу.</span><span class="sxs-lookup"><span data-stu-id="74ec5-p101">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="74ec5-107">Если у элемента [**Driveitem**](driveitem.md) есть аспект **shared**, имеющий значение, отличное от null, это значит, что к элементу предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="74ec5-107">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="74ec5-108">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="74ec5-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="74ec5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="74ec5-109">Properties</span></span>

| <span data-ttu-id="74ec5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="74ec5-110">Property</span></span>       | <span data-ttu-id="74ec5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="74ec5-111">Type</span></span>                          | <span data-ttu-id="74ec5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="74ec5-112">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="74ec5-113">owner</span><span class="sxs-lookup"><span data-stu-id="74ec5-113">owner</span></span>          | [<span data-ttu-id="74ec5-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="74ec5-114">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="74ec5-p102">Удостоверение владельца общего элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74ec5-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="74ec5-117">scope</span><span class="sxs-lookup"><span data-stu-id="74ec5-117">scope</span></span>          | <span data-ttu-id="74ec5-118">String</span><span class="sxs-lookup"><span data-stu-id="74ec5-118">String</span></span>                        | <span data-ttu-id="74ec5-p103">Указывает область, в рамках которой предоставлен доступ к общему элементу: `anonymous`, `organization` или `users`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74ec5-p103">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="74ec5-121">sharedBy</span><span class="sxs-lookup"><span data-stu-id="74ec5-121">sharedBy</span></span>       | [<span data-ttu-id="74ec5-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="74ec5-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="74ec5-p104">Удостоверение пользователя, предоставившего общий доступ к элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74ec5-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="74ec5-125">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="74ec5-125">sharedDateTime</span></span> | <span data-ttu-id="74ec5-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74ec5-126">DateTimeOffset</span></span>                | <span data-ttu-id="74ec5-p105">Дата и время предоставления общего доступа к элементу в формате UTC. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="74ec5-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-options"></a><span data-ttu-id="74ec5-129">Параметры области</span><span class="sxs-lookup"><span data-stu-id="74ec5-129">Scope options</span></span>

| <span data-ttu-id="74ec5-130">Значение</span><span class="sxs-lookup"><span data-stu-id="74ec5-130">Value</span></span>          | <span data-ttu-id="74ec5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="74ec5-131">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="74ec5-132">Доступ к элементу предоставляется с помощью ссылки. Любой пользователь, у которого есть такая ссылка, может получить доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="74ec5-132">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="74ec5-133">Доступ к элементу предоставляется с помощью ссылки. Любой пользователь в организации владельца элемента, располагающий такой ссылкой, может получить доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="74ec5-133">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="74ec5-134">Доступ к элементу предоставляется только определенным пользователям.</span><span class="sxs-lookup"><span data-stu-id="74ec5-134">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="74ec5-135">Заметки</span><span class="sxs-lookup"><span data-stu-id="74ec5-135">Remarks</span></span>

<span data-ttu-id="74ec5-136">Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="74ec5-136">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

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

