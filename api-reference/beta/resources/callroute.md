---
title: Тип ресурса Каллрауте
description: Тип Каллрауте.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9978bffd55f62f0646f84d2405df70eba6232d68
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974061"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="ed90f-103">Тип ресурса Каллрауте</span><span class="sxs-lookup"><span data-stu-id="ed90f-103">callRoute resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed90f-104">Тип Каллрауте.</span><span class="sxs-lookup"><span data-stu-id="ed90f-104">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="ed90f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ed90f-105">Properties</span></span>

| <span data-ttu-id="ed90f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ed90f-106">Property</span></span>            | <span data-ttu-id="ed90f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ed90f-107">Type</span></span>                          | <span data-ttu-id="ed90f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ed90f-108">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="ed90f-109">Наконец</span><span class="sxs-lookup"><span data-stu-id="ed90f-109">final</span></span>               | [<span data-ttu-id="ed90f-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="ed90f-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="ed90f-111">Идентификатор, разрешенный в вызове.</span><span class="sxs-lookup"><span data-stu-id="ed90f-111">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="ed90f-112">Исходный текст</span><span class="sxs-lookup"><span data-stu-id="ed90f-112">original</span></span>            | [<span data-ttu-id="ed90f-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="ed90f-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="ed90f-114">Идентификатор, который изначально использовался при вызове.</span><span class="sxs-lookup"><span data-stu-id="ed90f-114">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="ed90f-115">Раутингтипе</span><span class="sxs-lookup"><span data-stu-id="ed90f-115">routingType</span></span>         | <span data-ttu-id="ed90f-116">String</span><span class="sxs-lookup"><span data-stu-id="ed90f-116">String</span></span>                        | <span data-ttu-id="ed90f-117">Возможные значения: `forwarded`, `lookup`, `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="ed90f-117">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="ed90f-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ed90f-118">JSON representation</span></span>

<span data-ttu-id="ed90f-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ed90f-119">The following is a JSON representation of the resource.</span></span>

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
