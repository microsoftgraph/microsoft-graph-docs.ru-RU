---
title: Тип ресурса Аудиосаурцелевел
description: Настройка уровня для других источников.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: bc2b0c11b18a3cf8120cab0bb9c745ae8880cfc6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339068"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="d138d-103">Тип ресурса Аудиосаурцелевел</span><span class="sxs-lookup"><span data-stu-id="d138d-103">audioSourceLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d138d-104">Настройка уровня для других источников.</span><span class="sxs-lookup"><span data-stu-id="d138d-104">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="d138d-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="d138d-105">Properties</span></span>

| <span data-ttu-id="d138d-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="d138d-106">Property</span></span>               | <span data-ttu-id="d138d-107">Тип</span><span class="sxs-lookup"><span data-stu-id="d138d-107">Type</span></span>    | <span data-ttu-id="d138d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d138d-108">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="d138d-109">Дуккосерс</span><span class="sxs-lookup"><span data-stu-id="d138d-109">duckOthers</span></span>             | <span data-ttu-id="d138d-110">Логический</span><span class="sxs-lookup"><span data-stu-id="d138d-110">Boolean</span></span> | <span data-ttu-id="d138d-111">Позволяет этому источнику дукк другие источники в активном состоянии.</span><span class="sxs-lookup"><span data-stu-id="d138d-111">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="d138d-112">Если задано значение true, необходимо задать уровень дуккинг.</span><span class="sxs-lookup"><span data-stu-id="d138d-112">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="d138d-113">степень</span><span class="sxs-lookup"><span data-stu-id="d138d-113">level</span></span>                  | <span data-ttu-id="d138d-114">Int64</span><span class="sxs-lookup"><span data-stu-id="d138d-114">Int64</span></span>   | <span data-ttu-id="d138d-115">Дуккинг уровень источника, если `duckOthers` задано значение. `true`</span><span class="sxs-lookup"><span data-stu-id="d138d-115">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="d138d-116">абонент</span><span class="sxs-lookup"><span data-stu-id="d138d-116">participant</span></span>            | <span data-ttu-id="d138d-117">String</span><span class="sxs-lookup"><span data-stu-id="d138d-117">String</span></span>  | <span data-ttu-id="d138d-118">Поток звука участника источника.</span><span class="sxs-lookup"><span data-stu-id="d138d-118">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="d138d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d138d-119">JSON representation</span></span>

<span data-ttu-id="d138d-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d138d-120">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
