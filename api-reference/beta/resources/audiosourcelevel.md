---
title: Тип ресурса Аудиосаурцелевел
description: Настройка уровня для других источников.
author: ananmishr
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: eb98e434540dd00529963c48ff3f3296e17e0c01
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998952"
---
# <a name="audiosourcelevel-resource-type"></a><span data-ttu-id="303c4-103">Тип ресурса Аудиосаурцелевел</span><span class="sxs-lookup"><span data-stu-id="303c4-103">audioSourceLevel resource type</span></span>

<span data-ttu-id="303c4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="303c4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="303c4-105">Настройка уровня для других источников.</span><span class="sxs-lookup"><span data-stu-id="303c4-105">Level configuration for other sources.</span></span>

## <a name="properties"></a><span data-ttu-id="303c4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="303c4-106">Properties</span></span>

| <span data-ttu-id="303c4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="303c4-107">Property</span></span>               | <span data-ttu-id="303c4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="303c4-108">Type</span></span>    | <span data-ttu-id="303c4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="303c4-109">Description</span></span>                                                                                         |
| :--------------------- | :------ | :---------------------------------------------------------------------------------------------------|
| <span data-ttu-id="303c4-110">дуккосерс</span><span class="sxs-lookup"><span data-stu-id="303c4-110">duckOthers</span></span>             | <span data-ttu-id="303c4-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="303c4-111">Boolean</span></span> | <span data-ttu-id="303c4-112">Позволяет этому источнику дукк другие источники в активном состоянии.</span><span class="sxs-lookup"><span data-stu-id="303c4-112">Enables this source to duck other sources while active.</span></span> <span data-ttu-id="303c4-113">Если задано значение true, необходимо задать уровень дуккинг.</span><span class="sxs-lookup"><span data-stu-id="303c4-113">If set to true, ducking level has to be set.</span></span>|
| <span data-ttu-id="303c4-114">степень</span><span class="sxs-lookup"><span data-stu-id="303c4-114">level</span></span>                  | <span data-ttu-id="303c4-115">Int64</span><span class="sxs-lookup"><span data-stu-id="303c4-115">Int64</span></span>   | <span data-ttu-id="303c4-116">Дуккинг уровень источника, если `duckOthers` задано значение `true` .</span><span class="sxs-lookup"><span data-stu-id="303c4-116">Ducking level of the source if `duckOthers` is set to `true`.</span></span>                                     |
| <span data-ttu-id="303c4-117">participant</span><span class="sxs-lookup"><span data-stu-id="303c4-117">participant</span></span>            | <span data-ttu-id="303c4-118">String</span><span class="sxs-lookup"><span data-stu-id="303c4-118">String</span></span>  | <span data-ttu-id="303c4-119">Поток звука участника источника.</span><span class="sxs-lookup"><span data-stu-id="303c4-119">The source participant audio stream.</span></span>                                                                |

## <a name="json-representation"></a><span data-ttu-id="303c4-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="303c4-120">JSON representation</span></span>

<span data-ttu-id="303c4-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="303c4-121">The following is a JSON representation of the resource.</span></span>

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


