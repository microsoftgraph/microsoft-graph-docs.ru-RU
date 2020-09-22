---
title: Тип ресурса Поситиондетаил
description: Тип ресурса Поситиондетаил
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: fbd013292754dea43dd69b645dcd2ab735559b69
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47971484"
---
# <a name="positiondetail-resource-type"></a><span data-ttu-id="a0629-103">Тип ресурса Поситиондетаил</span><span class="sxs-lookup"><span data-stu-id="a0629-103">positionDetail resource type</span></span>

<span data-ttu-id="a0629-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0629-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0629-105">Представляет сведения о позициях, связанных с сущностями в [профиле](profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="a0629-105">Represents information about positions related to entities within a user's [profile](profile.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a0629-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a0629-106">Properties</span></span>

| <span data-ttu-id="a0629-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a0629-107">Property</span></span>       | <span data-ttu-id="a0629-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a0629-108">Type</span></span>                             | <span data-ttu-id="a0629-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a0629-109">Description</span></span>                                            |
|:---------------|:---------------------------------|:-------------------------------------------------------|
|<span data-ttu-id="a0629-110">внутрихолдинговом</span><span class="sxs-lookup"><span data-stu-id="a0629-110">company</span></span>         |[<span data-ttu-id="a0629-111">компанидетаил</span><span class="sxs-lookup"><span data-stu-id="a0629-111">companyDetail</span></span>](companydetail.md) | <span data-ttu-id="a0629-112">Подробные сведения о компании или работодателе.</span><span class="sxs-lookup"><span data-stu-id="a0629-112">Detail about the company or employer.</span></span>                  |
|<span data-ttu-id="a0629-113">description</span><span class="sxs-lookup"><span data-stu-id="a0629-113">description</span></span>     |<span data-ttu-id="a0629-114">String</span><span class="sxs-lookup"><span data-stu-id="a0629-114">String</span></span>                            | <span data-ttu-id="a0629-115">Описание интересующей должности.</span><span class="sxs-lookup"><span data-stu-id="a0629-115">Description of the position in question.</span></span>               |
|<span data-ttu-id="a0629-116">ендмонсеар</span><span class="sxs-lookup"><span data-stu-id="a0629-116">endMonthYear</span></span>    |<span data-ttu-id="a0629-117">Дата</span><span class="sxs-lookup"><span data-stu-id="a0629-117">Date</span></span>                              | <span data-ttu-id="a0629-118">По завершении должности.</span><span class="sxs-lookup"><span data-stu-id="a0629-118">When the position ended.</span></span>                               |
|<span data-ttu-id="a0629-119">jobTitle;</span><span class="sxs-lookup"><span data-stu-id="a0629-119">jobTitle</span></span>        |<span data-ttu-id="a0629-120">String</span><span class="sxs-lookup"><span data-stu-id="a0629-120">String</span></span>                            | <span data-ttu-id="a0629-121">Заголовок, хранящийся в этой позиции.</span><span class="sxs-lookup"><span data-stu-id="a0629-121">The title held when in that position.</span></span>                  |
|<span data-ttu-id="a0629-122">role</span><span class="sxs-lookup"><span data-stu-id="a0629-122">role</span></span>            |<span data-ttu-id="a0629-123">String</span><span class="sxs-lookup"><span data-stu-id="a0629-123">String</span></span>                            | <span data-ttu-id="a0629-124">Роль, к которой присвоено место.</span><span class="sxs-lookup"><span data-stu-id="a0629-124">The role the position entailed.</span></span>                        |
|<span data-ttu-id="a0629-125">стартмонсеар</span><span class="sxs-lookup"><span data-stu-id="a0629-125">startMonthYear</span></span>  |<span data-ttu-id="a0629-126">Дата</span><span class="sxs-lookup"><span data-stu-id="a0629-126">Date</span></span>                              | <span data-ttu-id="a0629-127">Начальный месяц и год позиции.</span><span class="sxs-lookup"><span data-stu-id="a0629-127">The start month and year of the position.</span></span>              |
|<span data-ttu-id="a0629-128">summary</span><span class="sxs-lookup"><span data-stu-id="a0629-128">summary</span></span>         |<span data-ttu-id="a0629-129">String</span><span class="sxs-lookup"><span data-stu-id="a0629-129">String</span></span>                            |<span data-ttu-id="a0629-130">Краткое описание положения.</span><span class="sxs-lookup"><span data-stu-id="a0629-130">Short summary of the position.</span></span>                          |

## <a name="json-representation"></a><span data-ttu-id="a0629-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a0629-131">JSON representation</span></span>

<span data-ttu-id="a0629-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a0629-132">The following is a JSON representation of the resource.</span></span>

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

