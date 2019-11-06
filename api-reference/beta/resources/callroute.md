---
title: Тип ресурса Каллрауте
description: Тип Каллрауте.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 698cf2d6c2ae8b157aee4db45219eeb0b85c73c5
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006742"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="ac542-103">Тип ресурса Каллрауте</span><span class="sxs-lookup"><span data-stu-id="ac542-103">callRoute resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac542-104">Тип Каллрауте.</span><span class="sxs-lookup"><span data-stu-id="ac542-104">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="ac542-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac542-105">Properties</span></span>

| <span data-ttu-id="ac542-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac542-106">Property</span></span>            | <span data-ttu-id="ac542-107">Тип</span><span class="sxs-lookup"><span data-stu-id="ac542-107">Type</span></span>                          | <span data-ttu-id="ac542-108">Описание</span><span class="sxs-lookup"><span data-stu-id="ac542-108">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="ac542-109">Наконец</span><span class="sxs-lookup"><span data-stu-id="ac542-109">final</span></span>               | [<span data-ttu-id="ac542-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="ac542-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="ac542-111">Идентификатор, разрешенный в вызове.</span><span class="sxs-lookup"><span data-stu-id="ac542-111">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="ac542-112">Исходный текст</span><span class="sxs-lookup"><span data-stu-id="ac542-112">original</span></span>            | [<span data-ttu-id="ac542-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="ac542-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="ac542-114">Идентификатор, который изначально использовался при вызове.</span><span class="sxs-lookup"><span data-stu-id="ac542-114">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="ac542-115">раутингтипе</span><span class="sxs-lookup"><span data-stu-id="ac542-115">routingType</span></span>         | <span data-ttu-id="ac542-116">String</span><span class="sxs-lookup"><span data-stu-id="ac542-116">String</span></span>                        | <span data-ttu-id="ac542-117">Возможные значения: `forwarded`, `lookup`, `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="ac542-117">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="ac542-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ac542-118">JSON representation</span></span>

<span data-ttu-id="ac542-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac542-119">The following is a JSON representation of the resource.</span></span>

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
