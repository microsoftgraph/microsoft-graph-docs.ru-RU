---
title: Тип ресурса Инкомингконтекст
description: Контекст, связанный с входящим звонком.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 4ade91c621dabdb7867ff5a4586276265d73ca81
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913529"
---
# <a name="incomingcontext-resource-type"></a><span data-ttu-id="5e266-103">Тип ресурса Инкомингконтекст</span><span class="sxs-lookup"><span data-stu-id="5e266-103">incomingContext resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e266-104">Контекст, связанный с входящим звонком.</span><span class="sxs-lookup"><span data-stu-id="5e266-104">The context associated with an incoming call.</span></span>

## <a name="properties"></a><span data-ttu-id="5e266-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5e266-105">Properties</span></span>

| <span data-ttu-id="5e266-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5e266-106">Property</span></span>              | <span data-ttu-id="5e266-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5e266-107">Type</span></span>                          | <span data-ttu-id="5e266-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5e266-108">Description</span></span>                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| <span data-ttu-id="5e266-109">обсерведпартиЦипантид</span><span class="sxs-lookup"><span data-stu-id="5e266-109">observedParticipantId</span></span> | <span data-ttu-id="5e266-110">String</span><span class="sxs-lookup"><span data-stu-id="5e266-110">String</span></span>                        | <span data-ttu-id="5e266-111">Идентификатор участника, который находится под наблюдением.</span><span class="sxs-lookup"><span data-stu-id="5e266-111">The id of the participant that is under observation.</span></span> <span data-ttu-id="5e266-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e266-112">Read-only.</span></span>         |
| <span data-ttu-id="5e266-113">онбехалфоф</span><span class="sxs-lookup"><span data-stu-id="5e266-113">onBehalfOf</span></span>            | [<span data-ttu-id="5e266-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="5e266-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="5e266-115">Идентификатор, который вызывается от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="5e266-115">The identity that the call is happening on behalf of.</span></span>                   |
| <span data-ttu-id="5e266-116">саурцепартиЦипантид</span><span class="sxs-lookup"><span data-stu-id="5e266-116">sourceParticipantId</span></span>   | <span data-ttu-id="5e266-117">String</span><span class="sxs-lookup"><span data-stu-id="5e266-117">String</span></span>                        | <span data-ttu-id="5e266-118">Идентификатор участника, который инициировал входящий вызов.</span><span class="sxs-lookup"><span data-stu-id="5e266-118">The id of the participant that triggered the incoming call.</span></span> <span data-ttu-id="5e266-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5e266-119">Read-only.</span></span>  |
| <span data-ttu-id="5e266-120">получатель</span><span class="sxs-lookup"><span data-stu-id="5e266-120">transferor</span></span>            | [<span data-ttu-id="5e266-121">identitySet</span><span class="sxs-lookup"><span data-stu-id="5e266-121">identitySet</span></span>](identityset.md) | <span data-ttu-id="5e266-122">Удостоверение, которое передал вызов.</span><span class="sxs-lookup"><span data-stu-id="5e266-122">The identity that transferred the call.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="5e266-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5e266-123">JSON representation</span></span>

<span data-ttu-id="5e266-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5e266-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "observedParticipantId",
    "onBehalfOf",
    "transferor"
  ],
  "@odata.type": "microsoft.graph.incomingContext"
}-->
```json
{
  "observedParticipantId": "String",
  "onBehalfOf": {"@odata.type": "#microsoft.graph.identitySet"},
  "sourceParticipantId": "String",
  "transferor": {"@odata.type": "#microsoft.graph.identitySet"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "incomingContext resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
