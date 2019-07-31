---
author: JeremyKelley
description: Ресурс Identity является коллекцией с ключом для ресурсов Identity.
ms.date: 09/10/2017
title: Identity
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c43981c1f7e79567afe901217030a0b5abed6f53
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006292"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="bd93b-103">Тип ресурса Identity</span><span class="sxs-lookup"><span data-stu-id="bd93b-103">identitySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd93b-104">Ресурс **Identity** является коллекцией с ключом для ресурсов [Identity](identity.md) .</span><span class="sxs-lookup"><span data-stu-id="bd93b-104">The **identitySet** resource is a keyed collection of [identity](identity.md) resources.</span></span>

<span data-ttu-id="bd93b-105">Он представляет набор удостоверений, связанных с различными событиями для элемента, например _созданием_ или _последним изменением_.</span><span class="sxs-lookup"><span data-stu-id="bd93b-105">It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd93b-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bd93b-106">JSON representation</span></span>

<span data-ttu-id="bd93b-107">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd93b-107">The following is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="bd93b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd93b-108">Properties</span></span>

| <span data-ttu-id="bd93b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd93b-109">Property</span></span>    | <span data-ttu-id="bd93b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bd93b-110">Type</span></span>                    | <span data-ttu-id="bd93b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bd93b-111">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="bd93b-112">application</span><span class="sxs-lookup"><span data-stu-id="bd93b-112">application</span></span> | [<span data-ttu-id="bd93b-113">Идентификация</span><span class="sxs-lookup"><span data-stu-id="bd93b-113">Identity</span></span>](identity.md) | <span data-ttu-id="bd93b-p101">Необязательный. Приложение, связанное с данным действием.</span><span class="sxs-lookup"><span data-stu-id="bd93b-p101">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="bd93b-116">conversation</span><span class="sxs-lookup"><span data-stu-id="bd93b-116">conversation</span></span>| [<span data-ttu-id="bd93b-117">Identity</span><span class="sxs-lookup"><span data-stu-id="bd93b-117">Identity</span></span>](identity.md) | <span data-ttu-id="bd93b-118">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="bd93b-118">Optional.</span></span> <span data-ttu-id="bd93b-119">Группа или канал, связанные с этим действием.</span><span class="sxs-lookup"><span data-stu-id="bd93b-119">The team or channel associated with this action.</span></span>       |
| <span data-ttu-id="bd93b-120">Конверсатионидентититипе</span><span class="sxs-lookup"><span data-stu-id="bd93b-120">conversationIdentityType</span></span>| [<span data-ttu-id="bd93b-121">Identity</span><span class="sxs-lookup"><span data-stu-id="bd93b-121">Identity</span></span>](identity.md) | <span data-ttu-id="bd93b-122">Необязательный.</span><span class="sxs-lookup"><span data-stu-id="bd93b-122">Optional.</span></span> <span data-ttu-id="bd93b-123">Указывает, идентифицирует \*\*\*\* ли свойство беседы группу или канал.</span><span class="sxs-lookup"><span data-stu-id="bd93b-123">Indicates whether the **conversation** property identifies a team or channel.</span></span>|
| <span data-ttu-id="bd93b-124">Устройство</span><span class="sxs-lookup"><span data-stu-id="bd93b-124">device</span></span>      | [<span data-ttu-id="bd93b-125">Идентификация</span><span class="sxs-lookup"><span data-stu-id="bd93b-125">Identity</span></span>](identity.md) | <span data-ttu-id="bd93b-p104">Необязательный. Устройство, связанное с данным действием.</span><span class="sxs-lookup"><span data-stu-id="bd93b-p104">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="bd93b-128">phone</span><span class="sxs-lookup"><span data-stu-id="bd93b-128">phone</span></span>       | [<span data-ttu-id="bd93b-129">identity</span><span class="sxs-lookup"><span data-stu-id="bd93b-129">identity</span></span>](identity.md) | <span data-ttu-id="bd93b-130">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="bd93b-130">Optional.</span></span> <span data-ttu-id="bd93b-131">Номер телефона, связанный с этим действием.</span><span class="sxs-lookup"><span data-stu-id="bd93b-131">The phone number associated with this action.</span></span> |
| <span data-ttu-id="bd93b-132">user</span><span class="sxs-lookup"><span data-stu-id="bd93b-132">user</span></span>        | [<span data-ttu-id="bd93b-133">Identity</span><span class="sxs-lookup"><span data-stu-id="bd93b-133">Identity</span></span>](identity.md) | <span data-ttu-id="bd93b-p106">Необязательный. Пользователь, связанный с данным действием.</span><span class="sxs-lookup"><span data-stu-id="bd93b-p106">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="bd93b-136">Заметки</span><span class="sxs-lookup"><span data-stu-id="bd93b-136">Remarks</span></span> 

<span data-ttu-id="bd93b-137">Ознакомьтесь со статьей [вызов](call.md) для использования ресурсов **удостоверений** .</span><span class="sxs-lookup"><span data-stu-id="bd93b-137">See [Call](call.md) for usage of **identitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
