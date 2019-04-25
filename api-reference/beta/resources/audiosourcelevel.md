---
title: Тип ресурса Аудиосаурцелевел
description: Настройка уровня для других источников.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c91a4c57b283f7669b2be22bba5de5d958b437ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535597"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="6b8b7-103">Тип ресурса Аудиосаурцелевел</span><span class="sxs-lookup"><span data-stu-id="6b8b7-103">audioSourceLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b8b7-104">Настройка уровня для других источников.</span><span class="sxs-lookup"><span data-stu-id="6b8b7-104">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="6b8b7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b8b7-105">Properties</span></span>

| <span data-ttu-id="6b8b7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b8b7-106">Property</span></span>               | <span data-ttu-id="6b8b7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="6b8b7-107">Type</span></span>    | <span data-ttu-id="6b8b7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="6b8b7-108">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="6b8b7-109">Дуккосерс</span><span class="sxs-lookup"><span data-stu-id="6b8b7-109">duckOthers</span></span>             | <span data-ttu-id="6b8b7-110">Логический</span><span class="sxs-lookup"><span data-stu-id="6b8b7-110">Boolean</span></span> | <span data-ttu-id="6b8b7-111">Позволяет этому источнику дукк другие источники в активном состоянии.</span><span class="sxs-lookup"><span data-stu-id="6b8b7-111">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="6b8b7-112">Если задано значение true, необходимо задать уровень дуккинг.</span><span class="sxs-lookup"><span data-stu-id="6b8b7-112">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="6b8b7-113">level</span><span class="sxs-lookup"><span data-stu-id="6b8b7-113">level</span></span>                  | <span data-ttu-id="6b8b7-114">Int64</span><span class="sxs-lookup"><span data-stu-id="6b8b7-114">Int64</span></span>   | <span data-ttu-id="6b8b7-115">Дуккинг уровень источника, если `duckOthers` задано значение. `true`</span><span class="sxs-lookup"><span data-stu-id="6b8b7-115">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="6b8b7-116">абонент</span><span class="sxs-lookup"><span data-stu-id="6b8b7-116">participant</span></span>            | <span data-ttu-id="6b8b7-117">String</span><span class="sxs-lookup"><span data-stu-id="6b8b7-117">String</span></span>  | <span data-ttu-id="6b8b7-118">Поток звука участника источника.</span><span class="sxs-lookup"><span data-stu-id="6b8b7-118">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="6b8b7-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6b8b7-119">JSON representation</span></span>

<span data-ttu-id="6b8b7-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b8b7-120">The following is a JSON representation of the resource.</span></span>

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
