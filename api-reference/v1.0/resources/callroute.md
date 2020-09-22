---
title: Тип ресурса Каллрауте
description: Представляет тип маршрута вызова.
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9ff55759e71cda0876a2ce5b0a65e47bcaf917a0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069269"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="9aac4-103">Тип ресурса Каллрауте</span><span class="sxs-lookup"><span data-stu-id="9aac4-103">callRoute resource type</span></span>

<span data-ttu-id="9aac4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9aac4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9aac4-105">Представляет тип маршрута вызова.</span><span class="sxs-lookup"><span data-stu-id="9aac4-105">Represents the call route type.</span></span>

## <a name="properties"></a><span data-ttu-id="9aac4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9aac4-106">Properties</span></span>

| <span data-ttu-id="9aac4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9aac4-107">Property</span></span>            | <span data-ttu-id="9aac4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9aac4-108">Type</span></span>                          | <span data-ttu-id="9aac4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9aac4-109">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="9aac4-110">Наконец</span><span class="sxs-lookup"><span data-stu-id="9aac4-110">final</span></span>               | [<span data-ttu-id="9aac4-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="9aac4-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="9aac4-112">Идентификатор, разрешенный в вызове.</span><span class="sxs-lookup"><span data-stu-id="9aac4-112">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="9aac4-113">Исходный текст</span><span class="sxs-lookup"><span data-stu-id="9aac4-113">original</span></span>            | [<span data-ttu-id="9aac4-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="9aac4-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="9aac4-115">Идентификатор, который изначально использовался при вызове.</span><span class="sxs-lookup"><span data-stu-id="9aac4-115">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="9aac4-116">раутингтипе</span><span class="sxs-lookup"><span data-stu-id="9aac4-116">routingType</span></span>         | <span data-ttu-id="9aac4-117">Строка</span><span class="sxs-lookup"><span data-stu-id="9aac4-117">String</span></span>                        | <span data-ttu-id="9aac4-118">Возможные значения: `forwarded`, `lookup`, `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="9aac4-118">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="9aac4-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9aac4-119">JSON representation</span></span>

<span data-ttu-id="9aac4-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9aac4-120">The following is a JSON representation of the resource.</span></span>

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

