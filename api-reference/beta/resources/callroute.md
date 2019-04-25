---
title: Тип ресурса Каллрауте
description: Тип Каллрауте.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: cfa470c4d3a03655221cab1f29baa60d00a8cf6c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543840"
---
# <a name="callroute-resource-type"></a><span data-ttu-id="5c996-103">Тип ресурса Каллрауте</span><span class="sxs-lookup"><span data-stu-id="5c996-103">callRoute resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c996-104">Тип Каллрауте.</span><span class="sxs-lookup"><span data-stu-id="5c996-104">The callRoute type.</span></span>

## <a name="properties"></a><span data-ttu-id="5c996-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5c996-105">Properties</span></span>

| <span data-ttu-id="5c996-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5c996-106">Property</span></span>            | <span data-ttu-id="5c996-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5c996-107">Type</span></span>                          | <span data-ttu-id="5c996-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5c996-108">Description</span></span>                                                  |
| :------------------ | :---------------------------- | :----------------------------------------------------------- |
| <span data-ttu-id="5c996-109">Наконец</span><span class="sxs-lookup"><span data-stu-id="5c996-109">final</span></span>               | [<span data-ttu-id="5c996-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="5c996-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="5c996-111">Идентификатор, разрешенный в вызове.</span><span class="sxs-lookup"><span data-stu-id="5c996-111">The identity that was resolved to in the call.</span></span>               |
| <span data-ttu-id="5c996-112">Исходный текст</span><span class="sxs-lookup"><span data-stu-id="5c996-112">original</span></span>            | [<span data-ttu-id="5c996-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="5c996-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="5c996-114">Идентификатор, который изначально использовался при вызове.</span><span class="sxs-lookup"><span data-stu-id="5c996-114">The identity that was originally used in the call.</span></span>           |
| <span data-ttu-id="5c996-115">Раутингтипе</span><span class="sxs-lookup"><span data-stu-id="5c996-115">routingType</span></span>         | <span data-ttu-id="5c996-116">String</span><span class="sxs-lookup"><span data-stu-id="5c996-116">String</span></span>                        | <span data-ttu-id="5c996-117">Возможные значения: `forwarded`, `lookup`, `selfFork`.</span><span class="sxs-lookup"><span data-stu-id="5c996-117">Possible values are: `forwarded`, `lookup`, `selfFork`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="5c996-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5c996-118">JSON representation</span></span>

<span data-ttu-id="5c996-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5c996-119">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/callroute.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
