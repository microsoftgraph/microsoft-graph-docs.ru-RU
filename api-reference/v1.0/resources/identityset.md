---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Identity
localization_priority: Normal
description: Ресурс IdentitySet представляет собой коллекцию ресурсов identity с ключами.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f1176f133f51432899a1fb6ddab964f04e658c69
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030221"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="e9e15-103">Тип ресурса IdentitySet</span><span class="sxs-lookup"><span data-stu-id="e9e15-103">IdentitySet resource type</span></span>

<span data-ttu-id="e9e15-p101">Ресурс **IdentitySet** представляет собой коллекцию ресурсов [identity](identity.md) с ключами. Он представляет набор удостоверений, связанных с различными событиями для элемента, например _созданием_ или _последним изменением_.</span><span class="sxs-lookup"><span data-stu-id="e9e15-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9e15-106">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e9e15-106">JSON representation</span></span>

<span data-ttu-id="e9e15-107">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e9e15-107">Here is a JSON representation of the resource.</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.identitySet",
       "optionalProperties": ["user", "application", "device"],
       "openType": true } -->
```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a><span data-ttu-id="e9e15-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e9e15-108">Properties</span></span>

| <span data-ttu-id="e9e15-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e9e15-109">Property</span></span>    | <span data-ttu-id="e9e15-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e9e15-110">Type</span></span>                    | <span data-ttu-id="e9e15-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e9e15-111">Description</span></span>                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| <span data-ttu-id="e9e15-112">application</span><span class="sxs-lookup"><span data-stu-id="e9e15-112">application</span></span> | [<span data-ttu-id="e9e15-113">Идентификация</span><span class="sxs-lookup"><span data-stu-id="e9e15-113">Identity</span></span>](identity.md) | <span data-ttu-id="e9e15-p102">Необязательный. Приложение, связанное с данным действием.</span><span class="sxs-lookup"><span data-stu-id="e9e15-p102">Optional. The application associated with this action.</span></span> |
| <span data-ttu-id="e9e15-116">Устройство</span><span class="sxs-lookup"><span data-stu-id="e9e15-116">device</span></span>      | [<span data-ttu-id="e9e15-117">Идентификация</span><span class="sxs-lookup"><span data-stu-id="e9e15-117">Identity</span></span>](identity.md) | <span data-ttu-id="e9e15-p103">Необязательный. Устройство, связанное с данным действием.</span><span class="sxs-lookup"><span data-stu-id="e9e15-p103">Optional. The device associated with this action.</span></span>      |
| <span data-ttu-id="e9e15-120">user</span><span class="sxs-lookup"><span data-stu-id="e9e15-120">user</span></span>        | [<span data-ttu-id="e9e15-121">Identity</span><span class="sxs-lookup"><span data-stu-id="e9e15-121">Identity</span></span>](identity.md) | <span data-ttu-id="e9e15-p104">Необязательный. Пользователь, связанный с данным действием.</span><span class="sxs-lookup"><span data-stu-id="e9e15-p104">Optional. The user associated with this action.</span></span>        |

## <a name="remarks"></a><span data-ttu-id="e9e15-124">Заметки</span><span class="sxs-lookup"><span data-stu-id="e9e15-124">Remarks</span></span> 

<span data-ttu-id="e9e15-125">Сведения об использовании ресурсов **IdentitySet** см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="e9e15-125">See [DriveItem](driveitem.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
