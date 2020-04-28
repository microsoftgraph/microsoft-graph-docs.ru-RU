---
title: Тип ресурса Едукатионалактивитидетаил
description: Тип ресурса Едукатионалактивитидетаил
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ccacf02184bbf54e49949d7671d34dde93b3859f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502825"
---
# <a name="educationalactivitydetail-resource-type"></a><span data-ttu-id="76d5b-103">Тип ресурса Едукатионалактивитидетаил</span><span class="sxs-lookup"><span data-stu-id="76d5b-103">educationalActivityDetail resource type</span></span>

<span data-ttu-id="76d5b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76d5b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76d5b-105">Представляет дополнительные сведения о выпуске, выпускнике, степени выпуске или других образовательных действиях, выполняемых пользователем и используемом в ресурсе [едукатионалактивити](educationalActivity.md) .</span><span class="sxs-lookup"><span data-stu-id="76d5b-105">Represents additional detail about an undergraduate, graduate, postgraduate degree or other educational activity that a user has undertaken and is used within an [educationalActivity](educationalActivity.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="76d5b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="76d5b-106">Properties</span></span>

| <span data-ttu-id="76d5b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="76d5b-107">Property</span></span>     | <span data-ttu-id="76d5b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="76d5b-108">Type</span></span>        | <span data-ttu-id="76d5b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="76d5b-109">Description</span></span>                                                   |
|:-------------|:------------|:--------------------------------------------------------------|
|<span data-ttu-id="76d5b-110">Аббревиатура</span><span class="sxs-lookup"><span data-stu-id="76d5b-110">abbreviation</span></span>  |<span data-ttu-id="76d5b-111">String</span><span class="sxs-lookup"><span data-stu-id="76d5b-111">String</span></span>       |<span data-ttu-id="76d5b-112">Сокращенное название степени или программы (пример: "доктор", "МБА")</span><span class="sxs-lookup"><span data-stu-id="76d5b-112">Shortened name of the degree or program (example: PhD, MBA)</span></span>    |
|<span data-ttu-id="76d5b-113">activities</span><span class="sxs-lookup"><span data-stu-id="76d5b-113">activities</span></span>    |<span data-ttu-id="76d5b-114">String</span><span class="sxs-lookup"><span data-stu-id="76d5b-114">String</span></span>       |<span data-ttu-id="76d5b-115">Действия факультативных, выполняемые вместе с программой.</span><span class="sxs-lookup"><span data-stu-id="76d5b-115">Extracurricular activities undertaken alongside the program.</span></span>   |
|<span data-ttu-id="76d5b-116">Награды</span><span class="sxs-lookup"><span data-stu-id="76d5b-116">awards</span></span>        |<span data-ttu-id="76d5b-117">String</span><span class="sxs-lookup"><span data-stu-id="76d5b-117">String</span></span>       |<span data-ttu-id="76d5b-118">Любые награды или соблюдаются, связанные с программой.</span><span class="sxs-lookup"><span data-stu-id="76d5b-118">Any awards or honors associated with the program.</span></span>              |
|<span data-ttu-id="76d5b-119">description</span><span class="sxs-lookup"><span data-stu-id="76d5b-119">description</span></span>   |<span data-ttu-id="76d5b-120">Строка</span><span class="sxs-lookup"><span data-stu-id="76d5b-120">String</span></span>       |<span data-ttu-id="76d5b-121">Краткое описание программы, предоставленной пользователем.</span><span class="sxs-lookup"><span data-stu-id="76d5b-121">Short description of the program provided by the user.</span></span>         |
|<span data-ttu-id="76d5b-122">displayName</span><span class="sxs-lookup"><span data-stu-id="76d5b-122">displayName</span></span>   |<span data-ttu-id="76d5b-123">Строка</span><span class="sxs-lookup"><span data-stu-id="76d5b-123">String</span></span>       |<span data-ttu-id="76d5b-124">Длинное имя программы, предоставленной пользователем.</span><span class="sxs-lookup"><span data-stu-id="76d5b-124">Long-form name of the program that the user has provided.</span></span>      |
|<span data-ttu-id="76d5b-125">фиелдсофстуди</span><span class="sxs-lookup"><span data-stu-id="76d5b-125">fieldsOfStudy</span></span> |<span data-ttu-id="76d5b-126">String</span><span class="sxs-lookup"><span data-stu-id="76d5b-126">String</span></span>       |<span data-ttu-id="76d5b-127">Основной и дополнительный номера, связанные с программой.</span><span class="sxs-lookup"><span data-stu-id="76d5b-127">Majors and minors associated with the program.</span></span> <span data-ttu-id="76d5b-128">(если это необходимо)</span><span class="sxs-lookup"><span data-stu-id="76d5b-128">(if applicable)</span></span> |
|<span data-ttu-id="76d5b-129">оценка</span><span class="sxs-lookup"><span data-stu-id="76d5b-129">grade</span></span>         |<span data-ttu-id="76d5b-130">String</span><span class="sxs-lookup"><span data-stu-id="76d5b-130">String</span></span>       |<span data-ttu-id="76d5b-131">Конечный уровень, класс, GPA или оценка.</span><span class="sxs-lookup"><span data-stu-id="76d5b-131">The final grade, class, GPA or score.</span></span>                          |
|<span data-ttu-id="76d5b-132">notes</span><span class="sxs-lookup"><span data-stu-id="76d5b-132">notes</span></span>         |<span data-ttu-id="76d5b-133">String</span><span class="sxs-lookup"><span data-stu-id="76d5b-133">String</span></span>       |<span data-ttu-id="76d5b-134">Дополнительные примечания, предоставленные пользователем.</span><span class="sxs-lookup"><span data-stu-id="76d5b-134">Additional notes the user has provided.</span></span>                        |
|<span data-ttu-id="76d5b-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="76d5b-135">webUrl</span></span>        |<span data-ttu-id="76d5b-136">String</span><span class="sxs-lookup"><span data-stu-id="76d5b-136">String</span></span>       |<span data-ttu-id="76d5b-137">Ссылка на страницу "степень" или "программа".</span><span class="sxs-lookup"><span data-stu-id="76d5b-137">Link to the degree or program page.</span></span>                            |

## <a name="json-representation"></a><span data-ttu-id="76d5b-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76d5b-138">JSON representation</span></span>

<span data-ttu-id="76d5b-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76d5b-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationalActivityDetail",
  "baseType": null
}-->

```json
{
  "abbreviation": "String",
  "activities": "String",
  "awards": "String",
  "description": "String",
  "displayName": "String",
  "fieldsOfStudy": "String",
  "grade": "String",
  "notes": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationalActivityDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->