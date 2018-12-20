---
title: Тип ресурса mediaPrompt
description: Тип mediaPrompt.
author: VinodRavichandran
ms.openlocfilehash: 4782772f463a613a759ad3b2b25cb05e7e160555
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380291"
---
# <a name="mediaprompt-resource-type"></a><span data-ttu-id="d3387-103">Тип ресурса mediaPrompt</span><span class="sxs-lookup"><span data-stu-id="d3387-103">mediaPrompt resource type</span></span>

> <span data-ttu-id="d3387-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d3387-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d3387-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3387-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d3387-106">Тип mediaPrompt.</span><span class="sxs-lookup"><span data-stu-id="d3387-106">The mediaPrompt type.</span></span>

## <a name="properties"></a><span data-ttu-id="d3387-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d3387-107">Properties</span></span>

| <span data-ttu-id="d3387-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d3387-108">Property</span></span>    | <span data-ttu-id="d3387-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d3387-109">Type</span></span>                      | <span data-ttu-id="d3387-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d3387-110">Description</span></span>                                                                     |
| :---------- | :------------------------ | :------------------------------------------------------------------------------ |
| <span data-ttu-id="d3387-111">цикл</span><span class="sxs-lookup"><span data-stu-id="d3387-111">loop</span></span>        | <span data-ttu-id="d3387-112">Int32</span><span class="sxs-lookup"><span data-stu-id="d3387-112">Int32</span></span>                     | <span data-ttu-id="d3387-113">Счетчик цикла.</span><span class="sxs-lookup"><span data-stu-id="d3387-113">The loop count.</span></span> <span data-ttu-id="d3387-114">значение 0 указывает цикл бесконечно.</span><span class="sxs-lookup"><span data-stu-id="d3387-114">0 value indicates to loop infinitely.</span></span> <span data-ttu-id="d3387-115">Значение по умолчанию — `1`.</span><span class="sxs-lookup"><span data-stu-id="d3387-115">The default value is `1`.</span></span> |
| <span data-ttu-id="d3387-116">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="d3387-116">mediaInfo</span></span>   | [<span data-ttu-id="d3387-117">mediaInfo</span><span class="sxs-lookup"><span data-stu-id="d3387-117">mediaInfo</span></span>](mediainfo.md) | <span data-ttu-id="d3387-118">Сведения о мультимедиа</span><span class="sxs-lookup"><span data-stu-id="d3387-118">The media information</span></span>                                                           |

## <a name="json-representation"></a><span data-ttu-id="d3387-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d3387-119">JSON representation</span></span>

<span data-ttu-id="d3387-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d3387-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->

```json
{
  "loop": 1024,
  "mediaInfo": { "@odata.type": "#microsoft.graph.mediaInfo" }
}
```

## <a name="example"></a><span data-ttu-id="d3387-121">Пример</span><span class="sxs-lookup"><span data-stu-id="d3387-121">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.mediaPrompt"
}-->
```json
{
  "mediaInfo": {
    "uri": "https://cdn.contoso.com/beep.wav",
    "resourceId": "1D6DE2D4-CD51-4309-8DAA-70768651088E"
  },
  "loop": 5
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mediaPrompt resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
