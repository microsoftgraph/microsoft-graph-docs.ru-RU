---
title: Тип ресурса Инкомингконтекст
description: Контекст, связанный с входящим вызовом.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0afe972be631a2048b2a1970b1fda41e8cb72920
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636899"
---
# <a name="incomingcontext-resource-type"></a><span data-ttu-id="376ff-103">Тип ресурса Инкомингконтекст</span><span class="sxs-lookup"><span data-stu-id="376ff-103">incomingContext resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="376ff-104">Контекст, связанный с входящим вызовом.</span><span class="sxs-lookup"><span data-stu-id="376ff-104">The context associated with an incoming call.</span></span>

## <a name="properties"></a><span data-ttu-id="376ff-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="376ff-105">Properties</span></span>

| <span data-ttu-id="376ff-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="376ff-106">Property</span></span>              | <span data-ttu-id="376ff-107">Тип</span><span class="sxs-lookup"><span data-stu-id="376ff-107">Type</span></span>                          | <span data-ttu-id="376ff-108">Описание</span><span class="sxs-lookup"><span data-stu-id="376ff-108">Description</span></span>                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| <span data-ttu-id="376ff-109">обсерведпартиЦипантид</span><span class="sxs-lookup"><span data-stu-id="376ff-109">observedParticipantId</span></span> | <span data-ttu-id="376ff-110">String</span><span class="sxs-lookup"><span data-stu-id="376ff-110">String</span></span>                        | <span data-ttu-id="376ff-111">Идентификатор участника, который находится под наблюдением.</span><span class="sxs-lookup"><span data-stu-id="376ff-111">The id of the participant that is under observation.</span></span> <span data-ttu-id="376ff-112">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="376ff-112">Read-only.</span></span>         |
| <span data-ttu-id="376ff-113">онбехалфоф</span><span class="sxs-lookup"><span data-stu-id="376ff-113">onBehalfOf</span></span>            | [<span data-ttu-id="376ff-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="376ff-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="376ff-115">Идентификатор, который вызывается от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="376ff-115">The identity that the call is happening on behalf of.</span></span>                   |
| <span data-ttu-id="376ff-116">саурцепартиЦипантид</span><span class="sxs-lookup"><span data-stu-id="376ff-116">sourceParticipantId</span></span>   | <span data-ttu-id="376ff-117">String</span><span class="sxs-lookup"><span data-stu-id="376ff-117">String</span></span>                        | <span data-ttu-id="376ff-118">Идентификатор участника, который инициировал входящий вызов.</span><span class="sxs-lookup"><span data-stu-id="376ff-118">The id of the participant that triggered the incoming call.</span></span> <span data-ttu-id="376ff-119">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="376ff-119">Read-only.</span></span>  |
| <span data-ttu-id="376ff-120">получатель</span><span class="sxs-lookup"><span data-stu-id="376ff-120">transferor</span></span>            | [<span data-ttu-id="376ff-121">identitySet</span><span class="sxs-lookup"><span data-stu-id="376ff-121">identitySet</span></span>](identityset.md) | <span data-ttu-id="376ff-122">Удостоверение, которое передал вызов.</span><span class="sxs-lookup"><span data-stu-id="376ff-122">The identity that transferred the call.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="376ff-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="376ff-123">JSON representation</span></span>

<span data-ttu-id="376ff-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="376ff-124">The following is a JSON representation of the resource.</span></span>

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
