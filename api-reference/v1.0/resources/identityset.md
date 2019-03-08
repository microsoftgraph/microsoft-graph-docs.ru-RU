---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Identity
localization_priority: Normal
ms.openlocfilehash: 369068dd48b9173032542303e3fd9831d25e6e9e
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480294"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="6ba87-102">Тип ресурса IdentitySet</span><span class="sxs-lookup"><span data-stu-id="6ba87-102">IdentitySet resource type</span></span>

<span data-ttu-id="6ba87-p101">Ресурс **IdentitySet** представляет собой коллекцию ресурсов [identity](identity.md) с ключами. Он представляет набор удостоверений, связанных с различными событиями для элемента, например _созданием_ или _последним изменением_.</span><span class="sxs-lookup"><span data-stu-id="6ba87-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ba87-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ba87-105">JSON representation</span></span>

<span data-ttu-id="6ba87-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ba87-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="6ba87-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ba87-107">Properties</span></span>

| <span data-ttu-id="6ba87-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ba87-108">Property</span></span>    | <span data-ttu-id="6ba87-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6ba87-109">Type</span></span>                    | <span data-ttu-id="6ba87-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6ba87-110">Description</span></span>                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| <span data-ttu-id="6ba87-111">application</span><span class="sxs-lookup"><span data-stu-id="6ba87-111">application</span></span> | [<span data-ttu-id="6ba87-112">Идентификация</span><span class="sxs-lookup"><span data-stu-id="6ba87-112">Identity</span></span>](identity.md) | <span data-ttu-id="6ba87-p102">Необязательный. Приложение, связанное с данным действием.</span><span class="sxs-lookup"><span data-stu-id="6ba87-p102">Optional. The application associated with this action.</span></span> |
| <span data-ttu-id="6ba87-115">Устройство</span><span class="sxs-lookup"><span data-stu-id="6ba87-115">device</span></span>      | [<span data-ttu-id="6ba87-116">Идентификация</span><span class="sxs-lookup"><span data-stu-id="6ba87-116">Identity</span></span>](identity.md) | <span data-ttu-id="6ba87-p103">Необязательный. Устройство, связанное с данным действием.</span><span class="sxs-lookup"><span data-stu-id="6ba87-p103">Optional. The device associated with this action.</span></span>      |
| <span data-ttu-id="6ba87-119">user</span><span class="sxs-lookup"><span data-stu-id="6ba87-119">user</span></span>        | [<span data-ttu-id="6ba87-120">Identity</span><span class="sxs-lookup"><span data-stu-id="6ba87-120">Identity</span></span>](identity.md) | <span data-ttu-id="6ba87-p104">Необязательный. Пользователь, связанный с данным действием.</span><span class="sxs-lookup"><span data-stu-id="6ba87-p104">Optional. The user associated with this action.</span></span>        |

## <a name="remarks"></a><span data-ttu-id="6ba87-123">Заметки</span><span class="sxs-lookup"><span data-stu-id="6ba87-123">Remarks</span></span> 

<span data-ttu-id="6ba87-124">Сведения об использовании ресурсов **IdentitySet** см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="6ba87-124">See [DriveItem](driveitem.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
