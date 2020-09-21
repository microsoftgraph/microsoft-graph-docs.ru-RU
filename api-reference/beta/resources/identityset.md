---
author: JeremyKelley
description: Ресурс Identity является коллекцией с ключом для ресурсов Identity.
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 60fdb901ecd74f3826604d139cad71d9d0844221
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47966766"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="4e6c3-103">Тип ресурса Identity</span><span class="sxs-lookup"><span data-stu-id="4e6c3-103">identitySet resource type</span></span>

<span data-ttu-id="4e6c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e6c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e6c3-105">Ресурс **Identity** является коллекцией с ключом для ресурсов [Identity](identity.md) .</span><span class="sxs-lookup"><span data-stu-id="4e6c3-105">The **identitySet** resource is a keyed collection of [identity](identity.md) resources.</span></span>

<span data-ttu-id="4e6c3-106">Он представляет набор удостоверений, связанных с различными событиями для элемента, например _созданием_ или _последним изменением_.</span><span class="sxs-lookup"><span data-stu-id="4e6c3-106">It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e6c3-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e6c3-107">JSON representation</span></span>

<span data-ttu-id="4e6c3-108">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e6c3-108">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet",
  "optionalProperties": [
    "application",
    "applicationInstance",
    "conversation",
    "conversationIdentityType",
    "device",
    "encrypted",
    "guest",
    "phone",
    "user"
  ],
  "openType": true
} -->
```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "applicationInstance": {"@odata.type": "microsoft.graph.identity"},
  "conversation": {"@odata.type": "microsoft.graph.identity"},
  "conversationIdentityType": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "encrypted": {"@odata.type": "microsoft.graph.identity"},
  "guest": {"@odata.type": "microsoft.graph.identity"},
  "phone": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a><span data-ttu-id="4e6c3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e6c3-109">Properties</span></span>

| <span data-ttu-id="4e6c3-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e6c3-110">Property</span></span>    | <span data-ttu-id="4e6c3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="4e6c3-111">Type</span></span>                    | <span data-ttu-id="4e6c3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="4e6c3-112">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="4e6c3-113">application</span><span class="sxs-lookup"><span data-stu-id="4e6c3-113">application</span></span> | [<span data-ttu-id="4e6c3-114">Identity</span><span class="sxs-lookup"><span data-stu-id="4e6c3-114">Identity</span></span>](identity.md) | <span data-ttu-id="4e6c3-p101">Необязательный. Приложение, связанное с данным действием.</span><span class="sxs-lookup"><span data-stu-id="4e6c3-p101">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="4e6c3-117">conversation</span><span class="sxs-lookup"><span data-stu-id="4e6c3-117">conversation</span></span>| [<span data-ttu-id="4e6c3-118">Identity</span><span class="sxs-lookup"><span data-stu-id="4e6c3-118">Identity</span></span>](identity.md) | <span data-ttu-id="4e6c3-119">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="4e6c3-119">Optional.</span></span> <span data-ttu-id="4e6c3-120">Группа или канал, связанные с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4e6c3-120">The team or channel associated with this action.</span></span>       |
| <span data-ttu-id="4e6c3-121">конверсатионидентититипе</span><span class="sxs-lookup"><span data-stu-id="4e6c3-121">conversationIdentityType</span></span>| [<span data-ttu-id="4e6c3-122">Identity</span><span class="sxs-lookup"><span data-stu-id="4e6c3-122">Identity</span></span>](identity.md) | <span data-ttu-id="4e6c3-123">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="4e6c3-123">Optional.</span></span> <span data-ttu-id="4e6c3-124">Указывает, идентифицирует ли свойство **беседы** группу или канал.</span><span class="sxs-lookup"><span data-stu-id="4e6c3-124">Indicates whether the **conversation** property identifies a team or channel.</span></span>|
| <span data-ttu-id="4e6c3-125">Устройство</span><span class="sxs-lookup"><span data-stu-id="4e6c3-125">device</span></span>      | [<span data-ttu-id="4e6c3-126">Identity</span><span class="sxs-lookup"><span data-stu-id="4e6c3-126">Identity</span></span>](identity.md) | <span data-ttu-id="4e6c3-p104">Необязательный. Устройство, связанное с данным действием.</span><span class="sxs-lookup"><span data-stu-id="4e6c3-p104">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="4e6c3-129">phone</span><span class="sxs-lookup"><span data-stu-id="4e6c3-129">phone</span></span>       | [<span data-ttu-id="4e6c3-130">identity</span><span class="sxs-lookup"><span data-stu-id="4e6c3-130">identity</span></span>](identity.md) | <span data-ttu-id="4e6c3-131">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="4e6c3-131">Optional.</span></span> <span data-ttu-id="4e6c3-132">Номер телефона, связанный с этим действием.</span><span class="sxs-lookup"><span data-stu-id="4e6c3-132">The phone number associated with this action.</span></span> |
| <span data-ttu-id="4e6c3-133">user</span><span class="sxs-lookup"><span data-stu-id="4e6c3-133">user</span></span>        | [<span data-ttu-id="4e6c3-134">Identity</span><span class="sxs-lookup"><span data-stu-id="4e6c3-134">Identity</span></span>](identity.md) | <span data-ttu-id="4e6c3-p106">Необязательный. Пользователь, связанный с данным действием.</span><span class="sxs-lookup"><span data-stu-id="4e6c3-p106">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="4e6c3-137">Заметки</span><span class="sxs-lookup"><span data-stu-id="4e6c3-137">Remarks</span></span> 

<span data-ttu-id="4e6c3-138">Ознакомьтесь со статьей [вызов](call.md) для использования ресурсов **удостоверений** .</span><span class="sxs-lookup"><span data-stu-id="4e6c3-138">See [Call](call.md) for usage of **identitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->


