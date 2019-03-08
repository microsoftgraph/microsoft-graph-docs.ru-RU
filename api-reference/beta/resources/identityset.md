---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Identity
localization_priority: Normal
ms.openlocfilehash: 0a963f7158dbb812fc1f51fbff208297a2a9f076
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482198"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="d670f-102">Тип ресурса Identity</span><span class="sxs-lookup"><span data-stu-id="d670f-102">identitySet resource type</span></span>

<span data-ttu-id="d670f-p101">Ресурс **IdentitySet** представляет собой коллекцию ресурсов [identity](identity.md) с ключами. Он представляет набор удостоверений, связанных с различными событиями для элемента, например _созданием_ или _последним изменением_.</span><span class="sxs-lookup"><span data-stu-id="d670f-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d670f-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d670f-105">JSON representation</span></span>

<span data-ttu-id="d670f-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d670f-106">The following is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="d670f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d670f-107">Properties</span></span>

| <span data-ttu-id="d670f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d670f-108">Property</span></span>    | <span data-ttu-id="d670f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d670f-109">Type</span></span>                    | <span data-ttu-id="d670f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d670f-110">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="d670f-111">application</span><span class="sxs-lookup"><span data-stu-id="d670f-111">application</span></span> | [<span data-ttu-id="d670f-112">Идентификация</span><span class="sxs-lookup"><span data-stu-id="d670f-112">Identity</span></span>](identity.md) | <span data-ttu-id="d670f-p102">Необязательный. Приложение, связанное с данным действием.</span><span class="sxs-lookup"><span data-stu-id="d670f-p102">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="d670f-115">Устройство</span><span class="sxs-lookup"><span data-stu-id="d670f-115">device</span></span>      | [<span data-ttu-id="d670f-116">Идентификация</span><span class="sxs-lookup"><span data-stu-id="d670f-116">Identity</span></span>](identity.md) | <span data-ttu-id="d670f-p103">Необязательный. Устройство, связанное с данным действием.</span><span class="sxs-lookup"><span data-stu-id="d670f-p103">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="d670f-119">phone</span><span class="sxs-lookup"><span data-stu-id="d670f-119">phone</span></span>       | [<span data-ttu-id="d670f-120">identity</span><span class="sxs-lookup"><span data-stu-id="d670f-120">identity</span></span>](identity.md) | <span data-ttu-id="d670f-121">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="d670f-121">Optional.</span></span> <span data-ttu-id="d670f-122">Номер телефона, связанный с этим действием.</span><span class="sxs-lookup"><span data-stu-id="d670f-122">The phone number associated with this action.</span></span> |
| <span data-ttu-id="d670f-123">user</span><span class="sxs-lookup"><span data-stu-id="d670f-123">user</span></span>        | [<span data-ttu-id="d670f-124">Identity</span><span class="sxs-lookup"><span data-stu-id="d670f-124">Identity</span></span>](identity.md) | <span data-ttu-id="d670f-p105">Необязательный. Пользователь, связанный с данным действием.</span><span class="sxs-lookup"><span data-stu-id="d670f-p105">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="d670f-127">Заметки</span><span class="sxs-lookup"><span data-stu-id="d670f-127">Remarks</span></span> 

<span data-ttu-id="d670f-128">Ознакомьтесь со статьей [вызов](call.md) для использования ресурсов **удостоверений** .</span><span class="sxs-lookup"><span data-stu-id="d670f-128">See [Call](call.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
