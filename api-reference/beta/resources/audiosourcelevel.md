---
title: Тип ресурса Аудиосаурцелевел
description: Настройка уровня для других источников.
author: ananmishr
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 35997bfcae7f33cc9bf8e62121c5dc2a724c95be
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913746"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="34bea-103">Тип ресурса Аудиосаурцелевел</span><span class="sxs-lookup"><span data-stu-id="34bea-103">audioSourceLevel resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34bea-104">Настройка уровня для других источников.</span><span class="sxs-lookup"><span data-stu-id="34bea-104">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="34bea-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="34bea-105">Properties</span></span>

| <span data-ttu-id="34bea-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="34bea-106">Property</span></span>               | <span data-ttu-id="34bea-107">Тип</span><span class="sxs-lookup"><span data-stu-id="34bea-107">Type</span></span>    | <span data-ttu-id="34bea-108">Описание</span><span class="sxs-lookup"><span data-stu-id="34bea-108">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="34bea-109">дуккосерс</span><span class="sxs-lookup"><span data-stu-id="34bea-109">duckOthers</span></span>             | <span data-ttu-id="34bea-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="34bea-110">Boolean</span></span> | <span data-ttu-id="34bea-111">Позволяет этому источнику дукк другие источники в активном состоянии.</span><span class="sxs-lookup"><span data-stu-id="34bea-111">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="34bea-112">Если задано значение true, необходимо задать уровень дуккинг.</span><span class="sxs-lookup"><span data-stu-id="34bea-112">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="34bea-113">степень</span><span class="sxs-lookup"><span data-stu-id="34bea-113">level</span></span>                  | <span data-ttu-id="34bea-114">Int64</span><span class="sxs-lookup"><span data-stu-id="34bea-114">Int64</span></span>   | <span data-ttu-id="34bea-115">Дуккинг уровень источника, если `duckOthers` задано значение. `true`</span><span class="sxs-lookup"><span data-stu-id="34bea-115">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="34bea-116">participant</span><span class="sxs-lookup"><span data-stu-id="34bea-116">participant</span></span>            | <span data-ttu-id="34bea-117">String</span><span class="sxs-lookup"><span data-stu-id="34bea-117">String</span></span>  | <span data-ttu-id="34bea-118">Поток звука участника источника.</span><span class="sxs-lookup"><span data-stu-id="34bea-118">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="34bea-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34bea-119">JSON representation</span></span>

<span data-ttu-id="34bea-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34bea-120">The following is a JSON representation of the resource.</span></span>

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
