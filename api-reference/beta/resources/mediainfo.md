---
title: Тип ресурса mediaInfo
description: Запрашивает сведения о мультимедиа, используемые в действиях для.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 217b9a5aaa88a1bbf343447fad344b322cfeb611
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924533"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="0a68d-103">Тип ресурса mediaInfo</span><span class="sxs-lookup"><span data-stu-id="0a68d-103">mediaInfo resource type</span></span>

> <span data-ttu-id="0a68d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0a68d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a68d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a68d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0a68d-106">Запрашивает сведения о мультимедиа, используемые в действиях для.</span><span class="sxs-lookup"><span data-stu-id="0a68d-106">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="0a68d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a68d-107">Properties</span></span>
| <span data-ttu-id="0a68d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a68d-108">Property</span></span>       | <span data-ttu-id="0a68d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0a68d-109">Type</span></span>    | <span data-ttu-id="0a68d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0a68d-110">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="0a68d-111">resourceId</span><span class="sxs-lookup"><span data-stu-id="0a68d-111">resourceId</span></span>     | <span data-ttu-id="0a68d-112">String</span><span class="sxs-lookup"><span data-stu-id="0a68d-112">String</span></span>  | <span data-ttu-id="0a68d-113">Уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="0a68d-113">Unique identity of the resource.</span></span> |
| <span data-ttu-id="0a68d-114">URI</span><span class="sxs-lookup"><span data-stu-id="0a68d-114">uri</span></span>            | <span data-ttu-id="0a68d-115">Строка</span><span class="sxs-lookup"><span data-stu-id="0a68d-115">String</span></span>  | <span data-ttu-id="0a68d-116">Путь к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="0a68d-116">Path to the resource.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="0a68d-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a68d-117">JSON representation</span></span>

<span data-ttu-id="0a68d-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a68d-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
