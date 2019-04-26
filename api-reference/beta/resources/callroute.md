---
title: Тип ресурса Каллрауте
description: Тип Каллрауте.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 06dd1a2265c5a6bda9feba0b51e7fd731d7945c3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328281"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="c1f10-103">Тип ресурса Каллрауте</span><span class="sxs-lookup"><span data-stu-id="c1f10-103">callRoute resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1f10-104">Тип Каллрауте.</span><span class="sxs-lookup"><span data-stu-id="c1f10-104">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="c1f10-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1f10-105">Properties</span></span>

| <span data-ttu-id="c1f10-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1f10-106">Property</span></span>            | <span data-ttu-id="c1f10-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c1f10-107">Type</span></span>                          | <span data-ttu-id="c1f10-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c1f10-108">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="c1f10-109">Наконец</span><span class="sxs-lookup"><span data-stu-id="c1f10-109">final</span></span>               | [<span data-ttu-id="c1f10-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="c1f10-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="c1f10-111">Идентификатор, разрешенный в вызове.</span><span class="sxs-lookup"><span data-stu-id="c1f10-111">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="c1f10-112">Исходный текст</span><span class="sxs-lookup"><span data-stu-id="c1f10-112">original</span></span>            | [<span data-ttu-id="c1f10-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="c1f10-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="c1f10-114">Идентификатор, который изначально использовался при вызове.</span><span class="sxs-lookup"><span data-stu-id="c1f10-114">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="c1f10-115">Раутингтипе</span><span class="sxs-lookup"><span data-stu-id="c1f10-115">routingType</span></span>         | <span data-ttu-id="c1f10-116">String</span><span class="sxs-lookup"><span data-stu-id="c1f10-116">String</span></span>                        | <span data-ttu-id="c1f10-117">Возможные значения: `forwarded`, `lookup`, `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="c1f10-117">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="c1f10-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1f10-118">JSON representation</span></span>

<span data-ttu-id="c1f10-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1f10-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRoute"
}-->
```json
{
  "final": {"@odata.type": "#microsoft.graph.identitySet"},
  "original": {"@odata.type": "#microsoft.graph.identitySet"},
  "routingType": "forwarded | lookup | selfFork"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "callRoute resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
