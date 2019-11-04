---
title: Тип ресурса Поситиондетаил
description: Тип ресурса Поситиондетаил
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: f4094da9c3ffc6a000fc0f7954ca8838a2d659af
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939798"
---
# <a name="positiondetail-resource-type"></a><span data-ttu-id="24c3e-103">Тип ресурса Поситиондетаил</span><span class="sxs-lookup"><span data-stu-id="24c3e-103">positionDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24c3e-104">Представляет сведения о позициях, связанных с сущностями в [профиле](profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="24c3e-104">Represents information about positions related to entities within a user's [profile](profile.md).</span></span>

## <a name="properties"></a><span data-ttu-id="24c3e-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="24c3e-105">Properties</span></span>

| <span data-ttu-id="24c3e-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="24c3e-106">Property</span></span>       | <span data-ttu-id="24c3e-107">Тип</span><span class="sxs-lookup"><span data-stu-id="24c3e-107">Type</span></span>                             | <span data-ttu-id="24c3e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="24c3e-108">Description</span></span>                                            |
|:---------------|:---------------------------------|:-------------------------------------------------------|
|<span data-ttu-id="24c3e-109">внутрихолдинговом</span><span class="sxs-lookup"><span data-stu-id="24c3e-109">company</span></span>         |[<span data-ttu-id="24c3e-110">компанидетаил</span><span class="sxs-lookup"><span data-stu-id="24c3e-110">companyDetail</span></span>](companydetail.md) | <span data-ttu-id="24c3e-111">Подробные сведения о компании или работодателе.</span><span class="sxs-lookup"><span data-stu-id="24c3e-111">Detail about the company or employer.</span></span>                  |
|<span data-ttu-id="24c3e-112">description</span><span class="sxs-lookup"><span data-stu-id="24c3e-112">description</span></span>     |<span data-ttu-id="24c3e-113">String</span><span class="sxs-lookup"><span data-stu-id="24c3e-113">String</span></span>                            | <span data-ttu-id="24c3e-114">Описание интересующей должности.</span><span class="sxs-lookup"><span data-stu-id="24c3e-114">Description of the position in question.</span></span>               |
|<span data-ttu-id="24c3e-115">ендмонсеар</span><span class="sxs-lookup"><span data-stu-id="24c3e-115">endMonthYear</span></span>    |<span data-ttu-id="24c3e-116">Дата</span><span class="sxs-lookup"><span data-stu-id="24c3e-116">Date</span></span>                              | <span data-ttu-id="24c3e-117">По завершении должности.</span><span class="sxs-lookup"><span data-stu-id="24c3e-117">When the position ended.</span></span>                               |
|<span data-ttu-id="24c3e-118">jobTitle;</span><span class="sxs-lookup"><span data-stu-id="24c3e-118">jobTitle</span></span>        |<span data-ttu-id="24c3e-119">String</span><span class="sxs-lookup"><span data-stu-id="24c3e-119">String</span></span>                            | <span data-ttu-id="24c3e-120">Заголовок, хранящийся в этой позиции.</span><span class="sxs-lookup"><span data-stu-id="24c3e-120">The title held when in that position.</span></span>                  |
|<span data-ttu-id="24c3e-121">role</span><span class="sxs-lookup"><span data-stu-id="24c3e-121">role</span></span>            |<span data-ttu-id="24c3e-122">Строка</span><span class="sxs-lookup"><span data-stu-id="24c3e-122">String</span></span>                            | <span data-ttu-id="24c3e-123">Роль, к которой присвоено место.</span><span class="sxs-lookup"><span data-stu-id="24c3e-123">The role the position entailed.</span></span>                        |
|<span data-ttu-id="24c3e-124">стартмонсеар</span><span class="sxs-lookup"><span data-stu-id="24c3e-124">startMonthYear</span></span>  |<span data-ttu-id="24c3e-125">Дата</span><span class="sxs-lookup"><span data-stu-id="24c3e-125">Date</span></span>                              | <span data-ttu-id="24c3e-126">Начальный месяц и год позиции.</span><span class="sxs-lookup"><span data-stu-id="24c3e-126">The start month and year of the position.</span></span>              |
|<span data-ttu-id="24c3e-127">summary</span><span class="sxs-lookup"><span data-stu-id="24c3e-127">summary</span></span>         |<span data-ttu-id="24c3e-128">Строка</span><span class="sxs-lookup"><span data-stu-id="24c3e-128">String</span></span>                            |<span data-ttu-id="24c3e-129">Краткое описание положения.</span><span class="sxs-lookup"><span data-stu-id="24c3e-129">Short summary of the position.</span></span>                          |

## <a name="json-representation"></a><span data-ttu-id="24c3e-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24c3e-130">JSON representation</span></span>

<span data-ttu-id="24c3e-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24c3e-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.positionDetail",
  "baseType": null
}-->

```json
{
  "company": {"@odata.type": "microsoft.graph.companyDetail"},
  "description": "String",
  "endMonthYear": "String (timestamp)",
  "jobTitle": "String",
  "role": "String",
  "startMonthYear": "String (timestamp)",
  "summary": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "positionDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->