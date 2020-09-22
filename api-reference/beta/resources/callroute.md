---
title: Тип ресурса Каллрауте
description: Тип Каллрауте.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 49ef6190f65adde817f3912d4133ff4a8553a88f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027218"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="6b6da-103">Тип ресурса Каллрауте</span><span class="sxs-lookup"><span data-stu-id="6b6da-103">callRoute resource type</span></span>

<span data-ttu-id="6b6da-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b6da-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b6da-105">Тип Каллрауте.</span><span class="sxs-lookup"><span data-stu-id="6b6da-105">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="6b6da-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b6da-106">Properties</span></span>

| <span data-ttu-id="6b6da-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b6da-107">Property</span></span>            | <span data-ttu-id="6b6da-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6b6da-108">Type</span></span>                          | <span data-ttu-id="6b6da-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6b6da-109">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="6b6da-110">Наконец</span><span class="sxs-lookup"><span data-stu-id="6b6da-110">final</span></span>               | [<span data-ttu-id="6b6da-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="6b6da-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="6b6da-112">Идентификатор, разрешенный в вызове.</span><span class="sxs-lookup"><span data-stu-id="6b6da-112">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="6b6da-113">Исходный текст</span><span class="sxs-lookup"><span data-stu-id="6b6da-113">original</span></span>            | [<span data-ttu-id="6b6da-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="6b6da-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="6b6da-115">Идентификатор, который изначально использовался при вызове.</span><span class="sxs-lookup"><span data-stu-id="6b6da-115">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="6b6da-116">раутингтипе</span><span class="sxs-lookup"><span data-stu-id="6b6da-116">routingType</span></span>         | <span data-ttu-id="6b6da-117">String</span><span class="sxs-lookup"><span data-stu-id="6b6da-117">String</span></span>                        | <span data-ttu-id="6b6da-118">Возможные значения: `forwarded`, `lookup`, `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="6b6da-118">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="6b6da-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b6da-119">JSON representation</span></span>

<span data-ttu-id="6b6da-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b6da-120">The following is a JSON representation of the resource.</span></span>

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


