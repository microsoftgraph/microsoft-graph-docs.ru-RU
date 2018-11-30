---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: IdentitySet
ms.openlocfilehash: 71620da04ea9d7f67d69422ce175182d406d44f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077911"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="18685-102">Тип ресурса identitySet</span><span class="sxs-lookup"><span data-stu-id="18685-102">identitySet resource type</span></span>

<span data-ttu-id="18685-p101">Ресурс **IdentitySet** представляет собой коллекцию ресурсов [identity](identity.md) с ключами. Он представляет набор удостоверений, связанных с различными событиями для элемента, например _созданием_ или _последним изменением_.</span><span class="sxs-lookup"><span data-stu-id="18685-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="18685-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18685-105">JSON representation</span></span>

<span data-ttu-id="18685-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18685-106">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet",
  "optionalProperties": [
    "application",
    "applicationInstance",
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
  "application": {"@odata.type": "#microsoft.graph.identity"},
  "applicationInstance": {"@odata.type": "#microsoft.graph.identity"},
  "device": {"@odata.type": "#microsoft.graph.identity"},
  "encrypted": {"@odata.type": "#microsoft.graph.identity"},
  "guest": {"@odata.type": "#microsoft.graph.identity"},
  "phone": {"@odata.type": "#microsoft.graph.identity"},
  "user": {"@odata.type": "#microsoft.graph.identity"}
}
```

## <a name="properties"></a><span data-ttu-id="18685-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="18685-107">Properties</span></span>

| <span data-ttu-id="18685-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="18685-108">Property</span></span>    | <span data-ttu-id="18685-109">Тип</span><span class="sxs-lookup"><span data-stu-id="18685-109">Type</span></span>                    | <span data-ttu-id="18685-110">Описание</span><span class="sxs-lookup"><span data-stu-id="18685-110">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="18685-111">application</span><span class="sxs-lookup"><span data-stu-id="18685-111">application</span></span> | [<span data-ttu-id="18685-112">Identity</span><span class="sxs-lookup"><span data-stu-id="18685-112">Identity</span></span>](identity.md) | <span data-ttu-id="18685-p102">Необязательный. Приложение, связанное с данным действием.</span><span class="sxs-lookup"><span data-stu-id="18685-p102">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="18685-115">Устройство
</span><span class="sxs-lookup"><span data-stu-id="18685-115">device</span></span>      | [<span data-ttu-id="18685-116">Identity</span><span class="sxs-lookup"><span data-stu-id="18685-116">Identity</span></span>](identity.md) | <span data-ttu-id="18685-p103">Необязательный. Устройство, связанное с данным действием.</span><span class="sxs-lookup"><span data-stu-id="18685-p103">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="18685-119">phone</span><span class="sxs-lookup"><span data-stu-id="18685-119">phone</span></span>       | [<span data-ttu-id="18685-120">identity</span><span class="sxs-lookup"><span data-stu-id="18685-120">identity</span></span>](identity.md) | <span data-ttu-id="18685-121">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="18685-121">Optional.</span></span> <span data-ttu-id="18685-122">Номер телефона, связанного с этого действия.</span><span class="sxs-lookup"><span data-stu-id="18685-122">The phone number associated with this action.</span></span> |
| <span data-ttu-id="18685-123">user</span><span class="sxs-lookup"><span data-stu-id="18685-123">user</span></span>        | [<span data-ttu-id="18685-124">Identity</span><span class="sxs-lookup"><span data-stu-id="18685-124">Identity</span></span>](identity.md) | <span data-ttu-id="18685-p105">Необязательный. Пользователь, связанный с данным действием.</span><span class="sxs-lookup"><span data-stu-id="18685-p105">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="18685-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="18685-127">Remarks</span></span> 

<span data-ttu-id="18685-128">В разделе [вызова](call.md) использования ресурсов **IdentitySet** .</span><span class="sxs-lookup"><span data-stu-id="18685-128">See [Call](call.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->