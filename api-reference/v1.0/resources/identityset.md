---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Identity
localization_priority: Normal
description: Ресурс IdentitySet представляет собой коллекцию ресурсов identity с ключами.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 09a0a48ca46f0d3a429705e5becf18f37832e5a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086671"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="3dd55-103">Тип ресурса IdentitySet</span><span class="sxs-lookup"><span data-stu-id="3dd55-103">IdentitySet resource type</span></span>

<span data-ttu-id="3dd55-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3dd55-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3dd55-p101">Ресурс **IdentitySet** представляет собой коллекцию ресурсов [identity](identity.md) с ключами. Он представляет набор удостоверений, связанных с различными событиями для элемента, например _созданием_ или _последним изменением_.</span><span class="sxs-lookup"><span data-stu-id="3dd55-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3dd55-107">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3dd55-107">JSON representation</span></span>

<span data-ttu-id="3dd55-108">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3dd55-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3dd55-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="3dd55-109">Properties</span></span>

| <span data-ttu-id="3dd55-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="3dd55-110">Property</span></span>    | <span data-ttu-id="3dd55-111">Тип</span><span class="sxs-lookup"><span data-stu-id="3dd55-111">Type</span></span>                    | <span data-ttu-id="3dd55-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3dd55-112">Description</span></span>                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| <span data-ttu-id="3dd55-113">application</span><span class="sxs-lookup"><span data-stu-id="3dd55-113">application</span></span> | [<span data-ttu-id="3dd55-114">Identity</span><span class="sxs-lookup"><span data-stu-id="3dd55-114">Identity</span></span>](identity.md) | <span data-ttu-id="3dd55-p102">Необязательный. Приложение, связанное с данным действием.</span><span class="sxs-lookup"><span data-stu-id="3dd55-p102">Optional. The application associated with this action.</span></span> |
| <span data-ttu-id="3dd55-117">Устройство</span><span class="sxs-lookup"><span data-stu-id="3dd55-117">device</span></span>      | [<span data-ttu-id="3dd55-118">Identity</span><span class="sxs-lookup"><span data-stu-id="3dd55-118">Identity</span></span>](identity.md) | <span data-ttu-id="3dd55-p103">Необязательный. Устройство, связанное с данным действием.</span><span class="sxs-lookup"><span data-stu-id="3dd55-p103">Optional. The device associated with this action.</span></span>      |
| <span data-ttu-id="3dd55-121">user</span><span class="sxs-lookup"><span data-stu-id="3dd55-121">user</span></span>        | [<span data-ttu-id="3dd55-122">Identity</span><span class="sxs-lookup"><span data-stu-id="3dd55-122">Identity</span></span>](identity.md) | <span data-ttu-id="3dd55-p104">Необязательный. Пользователь, связанный с данным действием.</span><span class="sxs-lookup"><span data-stu-id="3dd55-p104">Optional. The user associated with this action.</span></span>        |

## <a name="remarks"></a><span data-ttu-id="3dd55-125">Заметки</span><span class="sxs-lookup"><span data-stu-id="3dd55-125">Remarks</span></span> 

<span data-ttu-id="3dd55-126">Сведения об использовании ресурсов **IdentitySet** см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="3dd55-126">See [DriveItem](driveitem.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->

