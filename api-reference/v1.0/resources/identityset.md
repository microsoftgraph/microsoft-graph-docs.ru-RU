---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: IdentitySet
ms.openlocfilehash: 4d2bb5d92ebe06e79a68d69b949baec19a33a4c6
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/28/2017
---
# <a name="identityset-resource-type"></a><span data-ttu-id="3db5d-102">Тип ресурса IdentitySet</span><span class="sxs-lookup"><span data-stu-id="3db5d-102">IdentitySet resource type</span></span>

<span data-ttu-id="3db5d-p101">Ресурс **IdentitySet** представляет собой коллекцию ресурсов [identity](identity.md) с ключами. Он представляет набор удостоверений, связанных с различными событиями для элемента, например _созданием_ или _последним изменением_.</span><span class="sxs-lookup"><span data-stu-id="3db5d-p101">The **IdentitySet** resource is a keyed collection of [identity](identity.md) resources. It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3db5d-105">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3db5d-105">JSON representation</span></span>

<span data-ttu-id="3db5d-106">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3db5d-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="3db5d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3db5d-107">Properties</span></span>

| <span data-ttu-id="3db5d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3db5d-108">Property</span></span>    | <span data-ttu-id="3db5d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3db5d-109">Type</span></span>                    | <span data-ttu-id="3db5d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3db5d-110">Description</span></span>                                            |
|:------------|:------------------------|:-------------------------------------------------------|
| <span data-ttu-id="3db5d-111">application</span><span class="sxs-lookup"><span data-stu-id="3db5d-111">application</span></span> | [<span data-ttu-id="3db5d-112">Identity</span><span class="sxs-lookup"><span data-stu-id="3db5d-112">Identity</span></span>](identity.md) | <span data-ttu-id="3db5d-p102">Необязательный. Приложение, связанное с данным действием.</span><span class="sxs-lookup"><span data-stu-id="3db5d-p102">Optional. The application associated with this action.</span></span> |
| <span data-ttu-id="3db5d-115">Устройство
</span><span class="sxs-lookup"><span data-stu-id="3db5d-115">device</span></span>      | [<span data-ttu-id="3db5d-116">Identity</span><span class="sxs-lookup"><span data-stu-id="3db5d-116">Identity</span></span>](identity.md) | <span data-ttu-id="3db5d-p103">Необязательный. Устройство, связанное с данным действием.</span><span class="sxs-lookup"><span data-stu-id="3db5d-p103">Optional. The device associated with this action.</span></span>      |
| <span data-ttu-id="3db5d-119">ПОЛЬЗОВАТЕЛЬ</span><span class="sxs-lookup"><span data-stu-id="3db5d-119">user</span></span>        | [<span data-ttu-id="3db5d-120">Identity</span><span class="sxs-lookup"><span data-stu-id="3db5d-120">Identity</span></span>](identity.md) | <span data-ttu-id="3db5d-p104">Необязательный. Пользователь, связанный с данным действием.</span><span class="sxs-lookup"><span data-stu-id="3db5d-p104">Optional. The user associated with this action.</span></span>        |

## <a name="remarks"></a><span data-ttu-id="3db5d-123">Заметки</span><span class="sxs-lookup"><span data-stu-id="3db5d-123">Remarks</span></span> 

<span data-ttu-id="3db5d-124">Сведения об использовании ресурсов **IdentitySet** см. в описании типа [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="3db5d-124">See [DriveItem](driveitem.md) for usage of **IdentitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
