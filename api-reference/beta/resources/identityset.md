---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Identity
localization_priority: Normal
ms.openlocfilehash: b1570fc0ec0a6e28bab569dfae6992675d8b3537
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333662"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="2795f-102">Тип ресурса Identity</span><span class="sxs-lookup"><span data-stu-id="2795f-102">identitySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2795f-103">Ресурс **Identity** является коллекцией с ключом для ресурсов [Identity](identity.md) .</span><span class="sxs-lookup"><span data-stu-id="2795f-103">The **identitySet** resource is a keyed collection of [identity](identity.md) resources.</span></span>

<span data-ttu-id="2795f-104">Он представляет набор удостоверений, связанных с различными событиями для элемента, например _созданием_ или _последним изменением_.</span><span class="sxs-lookup"><span data-stu-id="2795f-104">It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2795f-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2795f-105">JSON representation</span></span>

<span data-ttu-id="2795f-106">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2795f-106">The following is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="2795f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2795f-107">Properties</span></span>

| <span data-ttu-id="2795f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2795f-108">Property</span></span>    | <span data-ttu-id="2795f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2795f-109">Type</span></span>                    | <span data-ttu-id="2795f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2795f-110">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="2795f-111">application</span><span class="sxs-lookup"><span data-stu-id="2795f-111">application</span></span> | [<span data-ttu-id="2795f-112">Идентификация</span><span class="sxs-lookup"><span data-stu-id="2795f-112">Identity</span></span>](identity.md) | <span data-ttu-id="2795f-p101">Необязательный. Приложение, связанное с данным действием.</span><span class="sxs-lookup"><span data-stu-id="2795f-p101">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="2795f-115">conversation</span><span class="sxs-lookup"><span data-stu-id="2795f-115">conversation</span></span>| [<span data-ttu-id="2795f-116">Identity</span><span class="sxs-lookup"><span data-stu-id="2795f-116">Identity</span></span>](identity.md) | <span data-ttu-id="2795f-117">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="2795f-117">Optional.</span></span> <span data-ttu-id="2795f-118">Группа или канал, связанные с этим действием.</span><span class="sxs-lookup"><span data-stu-id="2795f-118">The team or channel associated with this action.</span></span>       |
| <span data-ttu-id="2795f-119">Конверсатионидентититипе</span><span class="sxs-lookup"><span data-stu-id="2795f-119">conversationIdentityType</span></span>| [<span data-ttu-id="2795f-120">Identity</span><span class="sxs-lookup"><span data-stu-id="2795f-120">Identity</span></span>](identity.md) | <span data-ttu-id="2795f-121">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="2795f-121">Optional.</span></span> <span data-ttu-id="2795f-122">Указывает, идентифицирует \*\*\*\* ли свойство беседы группу или канал.</span><span class="sxs-lookup"><span data-stu-id="2795f-122">Indicates whether the **conversation** property identifies a team or channel.</span></span>|
| <span data-ttu-id="2795f-123">Устройство</span><span class="sxs-lookup"><span data-stu-id="2795f-123">device</span></span>      | [<span data-ttu-id="2795f-124">Идентификация</span><span class="sxs-lookup"><span data-stu-id="2795f-124">Identity</span></span>](identity.md) | <span data-ttu-id="2795f-p104">Необязательный. Устройство, связанное с данным действием.</span><span class="sxs-lookup"><span data-stu-id="2795f-p104">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="2795f-127">phone</span><span class="sxs-lookup"><span data-stu-id="2795f-127">phone</span></span>       | [<span data-ttu-id="2795f-128">identity</span><span class="sxs-lookup"><span data-stu-id="2795f-128">identity</span></span>](identity.md) | <span data-ttu-id="2795f-129">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="2795f-129">Optional.</span></span> <span data-ttu-id="2795f-130">Номер телефона, связанный с этим действием.</span><span class="sxs-lookup"><span data-stu-id="2795f-130">The phone number associated with this action.</span></span> |
| <span data-ttu-id="2795f-131">user</span><span class="sxs-lookup"><span data-stu-id="2795f-131">user</span></span>        | [<span data-ttu-id="2795f-132">Identity</span><span class="sxs-lookup"><span data-stu-id="2795f-132">Identity</span></span>](identity.md) | <span data-ttu-id="2795f-p106">Необязательный. Пользователь, связанный с данным действием.</span><span class="sxs-lookup"><span data-stu-id="2795f-p106">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="2795f-135">Заметки</span><span class="sxs-lookup"><span data-stu-id="2795f-135">Remarks</span></span> 

<span data-ttu-id="2795f-136">Ознакомьтесь со статьей [вызов](call.md) для использования ресурсов **удостоверений** .</span><span class="sxs-lookup"><span data-stu-id="2795f-136">See [Call](call.md) for usage of **identitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
