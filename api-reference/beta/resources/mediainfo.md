---
title: Тип ресурса Медиаинфо
description: Сведения о мультимедиа, используемые в действиях для запросов.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4c6f8e4f4ceea184f9663c433672d0892ed92467
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342648"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="7aa24-103">Тип ресурса Медиаинфо</span><span class="sxs-lookup"><span data-stu-id="7aa24-103">mediaInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7aa24-104">Сведения о мультимедиа, используемые в действиях для запросов.</span><span class="sxs-lookup"><span data-stu-id="7aa24-104">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="7aa24-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="7aa24-105">Properties</span></span>
| <span data-ttu-id="7aa24-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="7aa24-106">Property</span></span>       | <span data-ttu-id="7aa24-107">Тип</span><span class="sxs-lookup"><span data-stu-id="7aa24-107">Type</span></span>    | <span data-ttu-id="7aa24-108">Описание</span><span class="sxs-lookup"><span data-stu-id="7aa24-108">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="7aa24-109">resourceId</span><span class="sxs-lookup"><span data-stu-id="7aa24-109">resourceId</span></span>     | <span data-ttu-id="7aa24-110">String</span><span class="sxs-lookup"><span data-stu-id="7aa24-110">String</span></span>  | <span data-ttu-id="7aa24-111">Уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="7aa24-111">Unique identity of the resource.</span></span> |
| <span data-ttu-id="7aa24-112">URI</span><span class="sxs-lookup"><span data-stu-id="7aa24-112">uri</span></span>            | <span data-ttu-id="7aa24-113">String</span><span class="sxs-lookup"><span data-stu-id="7aa24-113">String</span></span>  | <span data-ttu-id="7aa24-114">Путь к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="7aa24-114">Path to the resource.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="7aa24-115">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7aa24-115">JSON representation</span></span>

<span data-ttu-id="7aa24-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7aa24-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
