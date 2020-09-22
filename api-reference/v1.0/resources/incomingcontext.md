---
title: Тип ресурса Инкомингконтекст
description: Представляет контекст, связанный с входящим вызовом.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 02bc6117ccf8a7ab0ce0bd1905883afdf61fc542
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054912"
---
# <a name="incomingcontext-resource-type"></a><span data-ttu-id="7ca0e-103">Тип ресурса Инкомингконтекст</span><span class="sxs-lookup"><span data-stu-id="7ca0e-103">incomingContext resource type</span></span>

<span data-ttu-id="7ca0e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ca0e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7ca0e-105">Представляет контекст, связанный с входящим вызовом.</span><span class="sxs-lookup"><span data-stu-id="7ca0e-105">Represents the context associated with an incoming call.</span></span>

## <a name="properties"></a><span data-ttu-id="7ca0e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ca0e-106">Properties</span></span>

| <span data-ttu-id="7ca0e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ca0e-107">Property</span></span>              | <span data-ttu-id="7ca0e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7ca0e-108">Type</span></span>                          | <span data-ttu-id="7ca0e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7ca0e-109">Description</span></span>                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| <span data-ttu-id="7ca0e-110">саурцепартиЦипантид</span><span class="sxs-lookup"><span data-stu-id="7ca0e-110">sourceParticipantId</span></span>   | <span data-ttu-id="7ca0e-111">String</span><span class="sxs-lookup"><span data-stu-id="7ca0e-111">String</span></span>                        | <span data-ttu-id="7ca0e-112">Идентификатор участника, который инициировал входящий вызов.</span><span class="sxs-lookup"><span data-stu-id="7ca0e-112">The ID of the participant that triggered the incoming call.</span></span> <span data-ttu-id="7ca0e-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ca0e-113">Read-only.</span></span>  |
| <span data-ttu-id="7ca0e-114">обсерведпартиЦипантид</span><span class="sxs-lookup"><span data-stu-id="7ca0e-114">observedParticipantId</span></span> | <span data-ttu-id="7ca0e-115">String</span><span class="sxs-lookup"><span data-stu-id="7ca0e-115">String</span></span>                        | <span data-ttu-id="7ca0e-116">Идентификатор участника, который находится под наблюдением.</span><span class="sxs-lookup"><span data-stu-id="7ca0e-116">The ID of the participant that is under observation.</span></span> <span data-ttu-id="7ca0e-117">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7ca0e-117">Read-only.</span></span>         |
| <span data-ttu-id="7ca0e-118">онбехалфоф</span><span class="sxs-lookup"><span data-stu-id="7ca0e-118">onBehalfOf</span></span>            | [<span data-ttu-id="7ca0e-119">identitySet</span><span class="sxs-lookup"><span data-stu-id="7ca0e-119">identitySet</span></span>](identityset.md) | <span data-ttu-id="7ca0e-120">Идентификатор, который вызывается от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="7ca0e-120">The identity that the call is happening on behalf of.</span></span>                   |
| <span data-ttu-id="7ca0e-121">получатель</span><span class="sxs-lookup"><span data-stu-id="7ca0e-121">transferor</span></span>            | [<span data-ttu-id="7ca0e-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="7ca0e-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="7ca0e-123">Удостоверение, которое передал вызов.</span><span class="sxs-lookup"><span data-stu-id="7ca0e-123">The identity that transferred the call.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="7ca0e-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7ca0e-124">JSON representation</span></span>

<span data-ttu-id="7ca0e-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ca0e-125">The following is a JSON representation of the resource.</span></span>

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

