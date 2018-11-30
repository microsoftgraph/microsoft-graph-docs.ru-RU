---
title: Тип ресурса audioSourceLevel
description: Конфигурации уровня для других источников.
ms.openlocfilehash: 527cb7e104817dc19287195d625bfc5f88c14e1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082117"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="cd2bb-103">Тип ресурса audioSourceLevel</span><span class="sxs-lookup"><span data-stu-id="cd2bb-103">audioSourceLevel resource type</span></span>

> <span data-ttu-id="cd2bb-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cd2bb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd2bb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd2bb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd2bb-106">Конфигурации уровня для других источников.</span><span class="sxs-lookup"><span data-stu-id="cd2bb-106">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="cd2bb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cd2bb-107">Properties</span></span>

| <span data-ttu-id="cd2bb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cd2bb-108">Property</span></span>               | <span data-ttu-id="cd2bb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cd2bb-109">Type</span></span>    | <span data-ttu-id="cd2bb-110">Description</span><span class="sxs-lookup"><span data-stu-id="cd2bb-110">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="cd2bb-111">duckOthers</span><span class="sxs-lookup"><span data-stu-id="cd2bb-111">duckOthers</span></span>             | <span data-ttu-id="cd2bb-112">Логический</span><span class="sxs-lookup"><span data-stu-id="cd2bb-112">Boolean</span></span> | <span data-ttu-id="cd2bb-113">Включение этого источника для duck другие источники при активный.</span><span class="sxs-lookup"><span data-stu-id="cd2bb-113">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="cd2bb-114">Если значение равно true, Уклонение от уровня должно быть задано.</span><span class="sxs-lookup"><span data-stu-id="cd2bb-114">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="cd2bb-115">level</span><span class="sxs-lookup"><span data-stu-id="cd2bb-115">level</span></span>                  | <span data-ttu-id="cd2bb-116">Int64</span><span class="sxs-lookup"><span data-stu-id="cd2bb-116">Int64</span></span>   | <span data-ttu-id="cd2bb-117">Уклонение от уровня источника, если `duckOthers` задано значение `true`.</span><span class="sxs-lookup"><span data-stu-id="cd2bb-117">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="cd2bb-118">Участник</span><span class="sxs-lookup"><span data-stu-id="cd2bb-118">participant</span></span>            | <span data-ttu-id="cd2bb-119">String</span><span class="sxs-lookup"><span data-stu-id="cd2bb-119">String</span></span>  | <span data-ttu-id="cd2bb-120">Источник участников аудиопотока.</span><span class="sxs-lookup"><span data-stu-id="cd2bb-120">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="cd2bb-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cd2bb-121">JSON representation</span></span>

<span data-ttu-id="cd2bb-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cd2bb-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioSourceLevel"
}-->
```json
{
  "duckOthers": true,
  "level": 100,
  "participant": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
