---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Shared
localization_priority: Normal
ms.openlocfilehash: cae69a60691d388570d29176fc20aac429907f8a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838992"
---
# <a name="shared-resource-type"></a><span data-ttu-id="c2462-102">Тип ресурса Shared</span><span class="sxs-lookup"><span data-stu-id="c2462-102">Shared resource type</span></span>

> <span data-ttu-id="c2462-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c2462-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2462-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2462-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c2462-p102">Ресурс **Shared** указывает, что к элементу DriveItem был предоставлен доступ другим пользователям. Ресурс содержит сведения о способе предоставления совместного доступа к элементу.</span><span class="sxs-lookup"><span data-stu-id="c2462-p102">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="c2462-107">Если у элемента [**Driveitem**](driveitem.md) есть аспект **shared**, имеющий значение, отличное от null, это значит, что к элементу предоставлен общий доступ.</span><span class="sxs-lookup"><span data-stu-id="c2462-107">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2462-108">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c2462-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c2462-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2462-109">Properties</span></span>

| <span data-ttu-id="c2462-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2462-110">Property</span></span>       | <span data-ttu-id="c2462-111">Тип</span><span class="sxs-lookup"><span data-stu-id="c2462-111">Type</span></span>                          | <span data-ttu-id="c2462-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c2462-112">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="c2462-113">owner</span><span class="sxs-lookup"><span data-stu-id="c2462-113">owner</span></span>          | [<span data-ttu-id="c2462-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="c2462-114">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="c2462-p103">Удостоверение владельца общего элемента. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2462-p103">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="c2462-117">scope</span><span class="sxs-lookup"><span data-stu-id="c2462-117">scope</span></span>          | <span data-ttu-id="c2462-118">Строка</span><span class="sxs-lookup"><span data-stu-id="c2462-118">String</span></span>                        | <span data-ttu-id="c2462-p104">Указывает область, в рамках которой предоставлен доступ к общему элементу: `anonymous`, `organization` или `users`. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2462-p104">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="c2462-121">sharedBy</span><span class="sxs-lookup"><span data-stu-id="c2462-121">sharedBy</span></span>       | [<span data-ttu-id="c2462-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="c2462-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="c2462-p105">Удостоверение пользователя, предоставившего общий доступ к элементу. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2462-p105">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="c2462-125">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="c2462-125">sharedDateTime</span></span> | <span data-ttu-id="c2462-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c2462-126">DateTimeOffset</span></span>                | <span data-ttu-id="c2462-p106">Дата и время предоставления общего доступа к элементу в формате UTC. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="c2462-p106">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-values"></a><span data-ttu-id="c2462-129">Значения областей</span><span class="sxs-lookup"><span data-stu-id="c2462-129">Scope values</span></span>

| <span data-ttu-id="c2462-130">Значение</span><span class="sxs-lookup"><span data-stu-id="c2462-130">Value</span></span>          | <span data-ttu-id="c2462-131">Описание</span><span class="sxs-lookup"><span data-stu-id="c2462-131">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="c2462-132">Доступ к элементу предоставляется с помощью ссылки. Любой пользователь, у которого есть такая ссылка, может получить доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="c2462-132">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="c2462-133">Доступ к элементу предоставляется с помощью ссылки. Любой пользователь в организации владельца элемента, располагающий такой ссылкой, может получить доступ к элементу.</span><span class="sxs-lookup"><span data-stu-id="c2462-133">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="c2462-134">Доступ к элементу предоставляется только определенным пользователям.</span><span class="sxs-lookup"><span data-stu-id="c2462-134">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="c2462-135">Заметки</span><span class="sxs-lookup"><span data-stu-id="c2462-135">Remarks</span></span>

<span data-ttu-id="c2462-136">Дополнительные сведения об аспектах ресурса **driveItem** см. в описании типа [**driveItem**](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="c2462-136">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared"
} -->
