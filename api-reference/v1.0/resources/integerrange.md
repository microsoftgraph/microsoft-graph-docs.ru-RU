---
title: тип ресурсов integerRange
description: Представляет инклюзивный диапазон наборов, описанных двумя границами Int64.
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: aee4ebfab164e6abbbecde083ba028c4c5a98723
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517403"
---
# <a name="integerrange-resource-type"></a><span data-ttu-id="a8277-103">тип ресурсов integerRange</span><span class="sxs-lookup"><span data-stu-id="a8277-103">integerRange resource type</span></span>

<span data-ttu-id="a8277-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8277-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a8277-105">Представляет инклюзивный диапазон наборов, описанных двумя границами Int64.</span><span class="sxs-lookup"><span data-stu-id="a8277-105">Represents an inclusive range of integers described by two Int64 boundaries.</span></span>

## <a name="properties"></a><span data-ttu-id="a8277-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8277-106">Properties</span></span>
| <span data-ttu-id="a8277-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8277-107">Property</span></span>     | <span data-ttu-id="a8277-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a8277-108">Type</span></span>        | <span data-ttu-id="a8277-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a8277-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a8277-110">начать</span><span class="sxs-lookup"><span data-stu-id="a8277-110">start</span></span>|<span data-ttu-id="a8277-111">Int64</span><span class="sxs-lookup"><span data-stu-id="a8277-111">Int64</span></span>|<span data-ttu-id="a8277-112">Инклюзивная нижняя граница диапазона integer.</span><span class="sxs-lookup"><span data-stu-id="a8277-112">The inclusive lower bound of the integer range.</span></span>|
|<span data-ttu-id="a8277-113">end</span><span class="sxs-lookup"><span data-stu-id="a8277-113">end</span></span>|<span data-ttu-id="a8277-114">Int64</span><span class="sxs-lookup"><span data-stu-id="a8277-114">Int64</span></span>|<span data-ttu-id="a8277-115">Инклюзивная верхняя граница диапазона integer.</span><span class="sxs-lookup"><span data-stu-id="a8277-115">The inclusive upper bound of the integer range.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8277-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8277-116">JSON representation</span></span>

<span data-ttu-id="a8277-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8277-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.integerRange"
}
-->
```json
{
    "start": 12345,
    "end": 12345
}
```