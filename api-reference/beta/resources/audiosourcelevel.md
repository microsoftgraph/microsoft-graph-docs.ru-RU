---
title: Тип ресурса audioSourceLevel
description: Конфигурации уровня для других источников.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c91a4c57b283f7669b2be22bba5de5d958b437ad
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528377"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="1d884-103">Тип ресурса audioSourceLevel</span><span class="sxs-lookup"><span data-stu-id="1d884-103">audioSourceLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1d884-104">Конфигурации уровня для других источников.</span><span class="sxs-lookup"><span data-stu-id="1d884-104">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="1d884-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="1d884-105">Properties</span></span>

| <span data-ttu-id="1d884-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="1d884-106">Property</span></span>               | <span data-ttu-id="1d884-107">Тип</span><span class="sxs-lookup"><span data-stu-id="1d884-107">Type</span></span>    | <span data-ttu-id="1d884-108">Описание</span><span class="sxs-lookup"><span data-stu-id="1d884-108">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1d884-109">duckOthers</span><span class="sxs-lookup"><span data-stu-id="1d884-109">duckOthers</span></span>             | <span data-ttu-id="1d884-110">Логическое</span><span class="sxs-lookup"><span data-stu-id="1d884-110">Boolean</span></span> | <span data-ttu-id="1d884-111">Включение этого источника для duck другие источники при активный.</span><span class="sxs-lookup"><span data-stu-id="1d884-111">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="1d884-112">Если значение равно true, Уклонение от уровня должно быть задано.</span><span class="sxs-lookup"><span data-stu-id="1d884-112">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="1d884-113">level</span><span class="sxs-lookup"><span data-stu-id="1d884-113">level</span></span>                  | <span data-ttu-id="1d884-114">Int64</span><span class="sxs-lookup"><span data-stu-id="1d884-114">Int64</span></span>   | <span data-ttu-id="1d884-115">Уклонение от уровня источника, если `duckOthers` задано значение `true`.</span><span class="sxs-lookup"><span data-stu-id="1d884-115">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="1d884-116">Участник</span><span class="sxs-lookup"><span data-stu-id="1d884-116">participant</span></span>            | <span data-ttu-id="1d884-117">String</span><span class="sxs-lookup"><span data-stu-id="1d884-117">String</span></span>  | <span data-ttu-id="1d884-118">Источник участников аудиопотока.</span><span class="sxs-lookup"><span data-stu-id="1d884-118">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="1d884-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1d884-119">JSON representation</span></span>

<span data-ttu-id="1d884-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1d884-120">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "audioSourceLevel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/audiosourcelevel.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
