---
title: Тип ресурса Инкомингконтекст
description: Представляет контекст, связанный с входящим вызовом.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6acd1928b223789df7580a5f74eefc723570ca93
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962569"
---
# <a name="incomingcontext-resource-type"></a><span data-ttu-id="d7124-103">Тип ресурса Инкомингконтекст</span><span class="sxs-lookup"><span data-stu-id="d7124-103">incomingContext resource type</span></span>

<span data-ttu-id="d7124-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7124-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d7124-105">Представляет контекст, связанный с входящим вызовом.</span><span class="sxs-lookup"><span data-stu-id="d7124-105">Represents the context associated with an incoming call.</span></span>

## <a name="properties"></a><span data-ttu-id="d7124-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d7124-106">Properties</span></span>

| <span data-ttu-id="d7124-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d7124-107">Property</span></span>              | <span data-ttu-id="d7124-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d7124-108">Type</span></span>                          | <span data-ttu-id="d7124-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d7124-109">Description</span></span>                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| <span data-ttu-id="d7124-110">саурцепартиЦипантид</span><span class="sxs-lookup"><span data-stu-id="d7124-110">sourceParticipantId</span></span>   | <span data-ttu-id="d7124-111">String</span><span class="sxs-lookup"><span data-stu-id="d7124-111">String</span></span>                        | <span data-ttu-id="d7124-112">Идентификатор участника, который инициировал входящий вызов.</span><span class="sxs-lookup"><span data-stu-id="d7124-112">The ID of the participant that triggered the incoming call.</span></span> <span data-ttu-id="d7124-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7124-113">Read-only.</span></span>  |
| <span data-ttu-id="d7124-114">обсерведпартиЦипантид</span><span class="sxs-lookup"><span data-stu-id="d7124-114">observedParticipantId</span></span> | <span data-ttu-id="d7124-115">String</span><span class="sxs-lookup"><span data-stu-id="d7124-115">String</span></span>                        | <span data-ttu-id="d7124-116">Идентификатор участника, который находится под наблюдением.</span><span class="sxs-lookup"><span data-stu-id="d7124-116">The ID of the participant that is under observation.</span></span> <span data-ttu-id="d7124-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d7124-117">Read-only.</span></span>         |
| <span data-ttu-id="d7124-118">онбехалфоф</span><span class="sxs-lookup"><span data-stu-id="d7124-118">onBehalfOf</span></span>            | [<span data-ttu-id="d7124-119">identitySet</span><span class="sxs-lookup"><span data-stu-id="d7124-119">identitySet</span></span>](identityset.md) | <span data-ttu-id="d7124-120">Идентификатор, который вызывается от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="d7124-120">The identity that the call is happening on behalf of.</span></span>                   |
| <span data-ttu-id="d7124-121">получатель</span><span class="sxs-lookup"><span data-stu-id="d7124-121">transferor</span></span>            | [<span data-ttu-id="d7124-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="d7124-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="d7124-123">Удостоверение, которое передал вызов.</span><span class="sxs-lookup"><span data-stu-id="d7124-123">The identity that transferred the call.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="d7124-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d7124-124">JSON representation</span></span>

<span data-ttu-id="d7124-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d7124-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "sourceParticipantId",
    "observedParticipantId",
    "onBehalfOf",
    "transferor"
  ],
  "@odata.type": "microsoft.graph.incomingContext"
}-->
```json
{
  "sourceParticipantId": "String",
  "observedParticipantId": "String",
  "onBehalfOf": {"@odata.type": "#microsoft.graph.identitySet"},
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
