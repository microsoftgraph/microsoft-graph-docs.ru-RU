---
title: Тип ресурса Инкомингконтекст
description: Контекст, связанный с входящим звонком.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a7eba09d18b2b60c3a5ae45a8ad335d8971d2c77
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496378"
---
# <a name="incomingcontext-resource-type"></a><span data-ttu-id="d4953-103">Тип ресурса Инкомингконтекст</span><span class="sxs-lookup"><span data-stu-id="d4953-103">incomingContext resource type</span></span>

<span data-ttu-id="d4953-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4953-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4953-105">Контекст, связанный с входящим звонком.</span><span class="sxs-lookup"><span data-stu-id="d4953-105">The context associated with an incoming call.</span></span>

## <a name="properties"></a><span data-ttu-id="d4953-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4953-106">Properties</span></span>

| <span data-ttu-id="d4953-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4953-107">Property</span></span>              | <span data-ttu-id="d4953-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d4953-108">Type</span></span>                          | <span data-ttu-id="d4953-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d4953-109">Description</span></span>                                                             |
|:----------------------|:------------------------------|:------------------------------------------------------------------------|
| <span data-ttu-id="d4953-110">обсерведпартиЦипантид</span><span class="sxs-lookup"><span data-stu-id="d4953-110">observedParticipantId</span></span> | <span data-ttu-id="d4953-111">String</span><span class="sxs-lookup"><span data-stu-id="d4953-111">String</span></span>                        | <span data-ttu-id="d4953-112">Идентификатор участника, который находится под наблюдением.</span><span class="sxs-lookup"><span data-stu-id="d4953-112">The id of the participant that is under observation.</span></span> <span data-ttu-id="d4953-113">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d4953-113">Read-only.</span></span>         |
| <span data-ttu-id="d4953-114">онбехалфоф</span><span class="sxs-lookup"><span data-stu-id="d4953-114">onBehalfOf</span></span>            | [<span data-ttu-id="d4953-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="d4953-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="d4953-116">Идентификатор, который вызывается от имени пользователя.</span><span class="sxs-lookup"><span data-stu-id="d4953-116">The identity that the call is happening on behalf of.</span></span>                   |
| <span data-ttu-id="d4953-117">саурцепартиЦипантид</span><span class="sxs-lookup"><span data-stu-id="d4953-117">sourceParticipantId</span></span>   | <span data-ttu-id="d4953-118">String</span><span class="sxs-lookup"><span data-stu-id="d4953-118">String</span></span>                        | <span data-ttu-id="d4953-119">Идентификатор участника, который инициировал входящий вызов.</span><span class="sxs-lookup"><span data-stu-id="d4953-119">The id of the participant that triggered the incoming call.</span></span> <span data-ttu-id="d4953-120">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="d4953-120">Read-only.</span></span>  |
| <span data-ttu-id="d4953-121">получатель</span><span class="sxs-lookup"><span data-stu-id="d4953-121">transferor</span></span>            | [<span data-ttu-id="d4953-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="d4953-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="d4953-123">Удостоверение, которое передал вызов.</span><span class="sxs-lookup"><span data-stu-id="d4953-123">The identity that transferred the call.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="d4953-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4953-124">JSON representation</span></span>

<span data-ttu-id="d4953-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4953-125">The following is a JSON representation of the resource.</span></span>

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
