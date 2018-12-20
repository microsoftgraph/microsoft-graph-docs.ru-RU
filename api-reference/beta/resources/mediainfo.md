---
title: Тип ресурса mediaInfo
description: Запрашивает сведения о мультимедиа, используемые в действиях для.
author: VinodRavichandran
ms.openlocfilehash: ea2eaa9e8e85da737df4c0c0170457fb3350820b
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380277"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="4956d-103">Тип ресурса mediaInfo</span><span class="sxs-lookup"><span data-stu-id="4956d-103">mediaInfo resource type</span></span>

> <span data-ttu-id="4956d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4956d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4956d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4956d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4956d-106">Запрашивает сведения о мультимедиа, используемые в действиях для.</span><span class="sxs-lookup"><span data-stu-id="4956d-106">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="4956d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4956d-107">Properties</span></span>
| <span data-ttu-id="4956d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4956d-108">Property</span></span>       | <span data-ttu-id="4956d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4956d-109">Type</span></span>    | <span data-ttu-id="4956d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4956d-110">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="4956d-111">resourceId</span><span class="sxs-lookup"><span data-stu-id="4956d-111">resourceId</span></span>     | <span data-ttu-id="4956d-112">String</span><span class="sxs-lookup"><span data-stu-id="4956d-112">String</span></span>  | <span data-ttu-id="4956d-113">Уникальный идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="4956d-113">Unique identity of the resource.</span></span> |
| <span data-ttu-id="4956d-114">URI</span><span class="sxs-lookup"><span data-stu-id="4956d-114">uri</span></span>            | <span data-ttu-id="4956d-115">String</span><span class="sxs-lookup"><span data-stu-id="4956d-115">String</span></span>  | <span data-ttu-id="4956d-116">Путь к ресурсу.</span><span class="sxs-lookup"><span data-stu-id="4956d-116">Path to the resource.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="4956d-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4956d-117">JSON representation</span></span>

<span data-ttu-id="4956d-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4956d-118">The following is a JSON representation of the resource.</span></span>

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