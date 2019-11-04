---
title: Тип ресурса Институтиондата
description: Тип ресурса Институтиондата
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 5724f56a5e68c059126eaac910d34999dcded632
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939455"
---
# <a name="institutiondata-resource-type"></a><span data-ttu-id="c263a-103">Тип ресурса Институтиондата</span><span class="sxs-lookup"><span data-stu-id="c263a-103">institutionData resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c263a-104">Представляет дополнительные сведения о выпуске, выпускнике, степени выпуске или других образовательных действиях, выполняемых пользователем и используемом в ресурсе [едукатионалактивити](educationalActivity.md) .</span><span class="sxs-lookup"><span data-stu-id="c263a-104">Represents additional detail about an undergraduate, graduate, postgraduate degree or other educational activity that a user has undertaken and is used within an [educationalActivity](educationalActivity.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="c263a-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="c263a-105">Properties</span></span>

| <span data-ttu-id="c263a-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="c263a-106">Property</span></span>     | <span data-ttu-id="c263a-107">Тип</span><span class="sxs-lookup"><span data-stu-id="c263a-107">Type</span></span>                                 | <span data-ttu-id="c263a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c263a-108">Description</span></span>                                              |
|:-------------|:-------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c263a-109">description</span><span class="sxs-lookup"><span data-stu-id="c263a-109">description</span></span>   |<span data-ttu-id="c263a-110">String</span><span class="sxs-lookup"><span data-stu-id="c263a-110">String</span></span>                                |<span data-ttu-id="c263a-111">Краткое описание учебного заведения, в котором пользователь изучается.</span><span class="sxs-lookup"><span data-stu-id="c263a-111">Short description of the institution the user studied at.</span></span> |
|<span data-ttu-id="c263a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c263a-112">displayName</span></span>   |<span data-ttu-id="c263a-113">Строка</span><span class="sxs-lookup"><span data-stu-id="c263a-113">String</span></span>                                |<span data-ttu-id="c263a-114">Имя учреждения, в котором пользователь изучается.</span><span class="sxs-lookup"><span data-stu-id="c263a-114">Name of the institution the user studied at.</span></span>              |
|<span data-ttu-id="c263a-115">location</span><span class="sxs-lookup"><span data-stu-id="c263a-115">location</span></span>      |[<span data-ttu-id="c263a-116">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="c263a-116">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="c263a-117">Адрес или расположение института.</span><span class="sxs-lookup"><span data-stu-id="c263a-117">Address or location of the institute.</span></span>                     |
|<span data-ttu-id="c263a-118">webUrl</span><span class="sxs-lookup"><span data-stu-id="c263a-118">webUrl</span></span>        |<span data-ttu-id="c263a-119">String</span><span class="sxs-lookup"><span data-stu-id="c263a-119">String</span></span>                                |<span data-ttu-id="c263a-120">Ссылка на домашнюю страницу "учреждение" или "Отдел".</span><span class="sxs-lookup"><span data-stu-id="c263a-120">Link to the institution or department homepage.</span></span>           |

## <a name="json-representation"></a><span data-ttu-id="c263a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c263a-121">JSON representation</span></span>

<span data-ttu-id="c263a-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c263a-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.institutionData",
  "baseType": null
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "location": {"@odata.type": "microsoft.graph.physicalAddress"},
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "institutionData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->