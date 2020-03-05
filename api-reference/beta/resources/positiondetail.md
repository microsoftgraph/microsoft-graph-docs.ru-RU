---
title: Тип ресурса Поситиондетаил
description: Тип ресурса Поситиондетаил
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6c77c116f013000ec4d419ec20c1e45c07187a22
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521595"
---
# <a name="positiondetail-resource-type"></a><span data-ttu-id="3e615-103">Тип ресурса Поситиондетаил</span><span class="sxs-lookup"><span data-stu-id="3e615-103">positionDetail resource type</span></span>

<span data-ttu-id="3e615-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3e615-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e615-105">Представляет сведения о позициях, связанных с сущностями в [профиле](profile.md)пользователя.</span><span class="sxs-lookup"><span data-stu-id="3e615-105">Represents information about positions related to entities within a user's [profile](profile.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3e615-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e615-106">Properties</span></span>

| <span data-ttu-id="3e615-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e615-107">Property</span></span>       | <span data-ttu-id="3e615-108">Тип</span><span class="sxs-lookup"><span data-stu-id="3e615-108">Type</span></span>                             | <span data-ttu-id="3e615-109">Описание</span><span class="sxs-lookup"><span data-stu-id="3e615-109">Description</span></span>                                            |
|:---------------|:---------------------------------|:-------------------------------------------------------|
|<span data-ttu-id="3e615-110">внутрихолдинговом</span><span class="sxs-lookup"><span data-stu-id="3e615-110">company</span></span>         |[<span data-ttu-id="3e615-111">компанидетаил</span><span class="sxs-lookup"><span data-stu-id="3e615-111">companyDetail</span></span>](companydetail.md) | <span data-ttu-id="3e615-112">Подробные сведения о компании или работодателе.</span><span class="sxs-lookup"><span data-stu-id="3e615-112">Detail about the company or employer.</span></span>                  |
|<span data-ttu-id="3e615-113">description</span><span class="sxs-lookup"><span data-stu-id="3e615-113">description</span></span>     |<span data-ttu-id="3e615-114">String</span><span class="sxs-lookup"><span data-stu-id="3e615-114">String</span></span>                            | <span data-ttu-id="3e615-115">Описание интересующей должности.</span><span class="sxs-lookup"><span data-stu-id="3e615-115">Description of the position in question.</span></span>               |
|<span data-ttu-id="3e615-116">ендмонсеар</span><span class="sxs-lookup"><span data-stu-id="3e615-116">endMonthYear</span></span>    |<span data-ttu-id="3e615-117">Дата</span><span class="sxs-lookup"><span data-stu-id="3e615-117">Date</span></span>                              | <span data-ttu-id="3e615-118">По завершении должности.</span><span class="sxs-lookup"><span data-stu-id="3e615-118">When the position ended.</span></span>                               |
|<span data-ttu-id="3e615-119">jobTitle;</span><span class="sxs-lookup"><span data-stu-id="3e615-119">jobTitle</span></span>        |<span data-ttu-id="3e615-120">String</span><span class="sxs-lookup"><span data-stu-id="3e615-120">String</span></span>                            | <span data-ttu-id="3e615-121">Заголовок, хранящийся в этой позиции.</span><span class="sxs-lookup"><span data-stu-id="3e615-121">The title held when in that position.</span></span>                  |
|<span data-ttu-id="3e615-122">role</span><span class="sxs-lookup"><span data-stu-id="3e615-122">role</span></span>            |<span data-ttu-id="3e615-123">String</span><span class="sxs-lookup"><span data-stu-id="3e615-123">String</span></span>                            | <span data-ttu-id="3e615-124">Роль, к которой присвоено место.</span><span class="sxs-lookup"><span data-stu-id="3e615-124">The role the position entailed.</span></span>                        |
|<span data-ttu-id="3e615-125">стартмонсеар</span><span class="sxs-lookup"><span data-stu-id="3e615-125">startMonthYear</span></span>  |<span data-ttu-id="3e615-126">Дата</span><span class="sxs-lookup"><span data-stu-id="3e615-126">Date</span></span>                              | <span data-ttu-id="3e615-127">Начальный месяц и год позиции.</span><span class="sxs-lookup"><span data-stu-id="3e615-127">The start month and year of the position.</span></span>              |
|<span data-ttu-id="3e615-128">summary</span><span class="sxs-lookup"><span data-stu-id="3e615-128">summary</span></span>         |<span data-ttu-id="3e615-129">String</span><span class="sxs-lookup"><span data-stu-id="3e615-129">String</span></span>                            |<span data-ttu-id="3e615-130">Краткое описание положения.</span><span class="sxs-lookup"><span data-stu-id="3e615-130">Short summary of the position.</span></span>                          |

## <a name="json-representation"></a><span data-ttu-id="3e615-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e615-131">JSON representation</span></span>

<span data-ttu-id="3e615-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e615-132">The following is a JSON representation of the resource.</span></span>

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