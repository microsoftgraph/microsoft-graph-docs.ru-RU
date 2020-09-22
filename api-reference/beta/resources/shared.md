---
author: JeremyKelley
description: Ресурс Shared указывает, что к элементу DriveItem был предоставлен доступ другим пользователям.
ms.date: 09/10/2017
title: Shared
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: dc867120028f1f36672f429ace0738779e9f9d48
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973689"
---
# <a name="shared-resource-type"></a><span data-ttu-id="46b7f-103">Тип ресурса Shared</span><span class="sxs-lookup"><span data-stu-id="46b7f-103">Shared resource type</span></span>

<span data-ttu-id="46b7f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46b7f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46b7f-p101">Ресурс **Shared** указывает, что к элементу DriveItem был предоставлен доступ другим пользователям. Ресурс содержит сведения о способе предоставления совместного доступа к элементу.</span><span class="sxs-lookup"><span data-stu-id="46b7f-p101">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="46b7f-107">Если у элемента [**Driveitem**](driveitem.md) есть аспект **shared**, имеющий значение, отличное от null, это значит, что к элементу предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="46b7f-107">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="46b7f-108">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="46b7f-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="46b7f-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="46b7f-109">Properties</span></span>

| <span data-ttu-id="46b7f-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="46b7f-110">Property</span></span>       | <span data-ttu-id="46b7f-111">Тип</span><span class="sxs-lookup"><span data-stu-id="46b7f-111">Type</span></span>                          | <span data-ttu-id="46b7f-112">Описание</span><span class="sxs-lookup"><span data-stu-id="46b7f-112">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="46b7f-113">owner</span><span class="sxs-lookup"><span data-stu-id="46b7f-113">owner</span></span>          | [<span data-ttu-id="46b7f-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="46b7f-114">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="46b7f-p102">Удостоверение владельца общего элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46b7f-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="46b7f-117">scope</span><span class="sxs-lookup"><span data-stu-id="46b7f-117">scope</span></span>          | <span data-ttu-id="46b7f-118">String</span><span class="sxs-lookup"><span data-stu-id="46b7f-118">String</span></span>                        | <span data-ttu-id="46b7f-p103">Указывает область, в рамках которой предоставлен доступ к общему элементу: `anonymous`, `organization` или `users`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46b7f-p103">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="46b7f-121">sharedBy</span><span class="sxs-lookup"><span data-stu-id="46b7f-121">sharedBy</span></span>       | [<span data-ttu-id="46b7f-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="46b7f-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="46b7f-p104">Удостоверение пользователя, предоставившего общий доступ к элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46b7f-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="46b7f-125">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="46b7f-125">sharedDateTime</span></span> | <span data-ttu-id="46b7f-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="46b7f-126">DateTimeOffset</span></span>                | <span data-ttu-id="46b7f-p105">Дата и время предоставления общего доступа к элементу в формате UTC. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="46b7f-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-values"></a><span data-ttu-id="46b7f-129">Значения областей</span><span class="sxs-lookup"><span data-stu-id="46b7f-129">Scope values</span></span>

| <span data-ttu-id="46b7f-130">Значение</span><span class="sxs-lookup"><span data-stu-id="46b7f-130">Value</span></span>          | <span data-ttu-id="46b7f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="46b7f-131">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="46b7f-132">Доступ к элементу предоставляется с помощью ссылки. Любой пользователь, у которого есть такая ссылка, может получить доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="46b7f-132">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="46b7f-133">Доступ к элементу предоставляется с помощью ссылки. Любой пользователь в организации владельца элемента, располагающий такой ссылкой, может получить доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="46b7f-133">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="46b7f-134">Доступ к элементу предоставляется только определенным пользователям.</span><span class="sxs-lookup"><span data-stu-id="46b7f-134">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="46b7f-135">Заметки</span><span class="sxs-lookup"><span data-stu-id="46b7f-135">Remarks</span></span>

<span data-ttu-id="46b7f-136">Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="46b7f-136">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

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


