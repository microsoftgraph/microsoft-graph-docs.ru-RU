---
title: Тип ресурса Едукатионалактивити
description: Тип ресурса Едукатионалактивити
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e1f4ffd3154700f59ebdd26a2213755810b561ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502846"
---
# <a name="educationalactivity-resource-type"></a><span data-ttu-id="09f23-103">Тип ресурса Едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="09f23-103">educationalActivity resource type</span></span>

<span data-ttu-id="09f23-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="09f23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09f23-105">Представляет данные, которые пользователь предоставил, относящихся к выпуску, выпускнику, выпуску или другим учебным действиям.</span><span class="sxs-lookup"><span data-stu-id="09f23-105">Represents data that a user has supplied related to undergraduate, graduate, postgraduate or other educational activities.</span></span>

<span data-ttu-id="09f23-106">Наследует свойства метаданных от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="09f23-106">Inherits metadata properties from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="09f23-107">Методы</span><span class="sxs-lookup"><span data-stu-id="09f23-107">Methods</span></span>

| <span data-ttu-id="09f23-108">Метод</span><span class="sxs-lookup"><span data-stu-id="09f23-108">Method</span></span>                                                       | <span data-ttu-id="09f23-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="09f23-109">Return Type</span></span>                                   | <span data-ttu-id="09f23-110">Описание</span><span class="sxs-lookup"><span data-stu-id="09f23-110">Description</span></span>                                                      |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="09f23-111">Получение Едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="09f23-111">Get educationalActivity</span></span>](../api/educationalactivity-get.md) | [<span data-ttu-id="09f23-112">едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="09f23-112">educationalActivity</span></span>](educationalactivity.md) | <span data-ttu-id="09f23-113">Чтение свойств и связей объекта Едукатионалактивити.</span><span class="sxs-lookup"><span data-stu-id="09f23-113">Read properties and relationships of educationalActivity object.</span></span> |
| <span data-ttu-id="09f23-114">[обновление](../api/educationalactivity-update.md).</span><span class="sxs-lookup"><span data-stu-id="09f23-114">[Update](../api/educationalactivity-update.md)</span></span>               | [<span data-ttu-id="09f23-115">едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="09f23-115">educationalActivity</span></span>](educationalactivity.md) | <span data-ttu-id="09f23-116">Обновление объекта Едукатионалактивити.</span><span class="sxs-lookup"><span data-stu-id="09f23-116">Update educationalActivity object.</span></span>                               |
| <span data-ttu-id="09f23-117">[удаление](../api/educationalactivity-delete.md);</span><span class="sxs-lookup"><span data-stu-id="09f23-117">[Delete](../api/educationalactivity-delete.md)</span></span>               | <span data-ttu-id="09f23-118">Нет</span><span class="sxs-lookup"><span data-stu-id="09f23-118">None</span></span>                                          | <span data-ttu-id="09f23-119">Удаление объекта Едукатионалактивити.</span><span class="sxs-lookup"><span data-stu-id="09f23-119">Delete educationalActivity object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="09f23-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="09f23-120">Properties</span></span>

| <span data-ttu-id="09f23-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="09f23-121">Property</span></span>           | <span data-ttu-id="09f23-122">Тип</span><span class="sxs-lookup"><span data-stu-id="09f23-122">Type</span></span>                                                      | <span data-ttu-id="09f23-123">Описание</span><span class="sxs-lookup"><span data-stu-id="09f23-123">Description</span></span>                                                                |
|:-------------------|:----------------------------------------------------------|:---------------------------------------------------------------------------|
|<span data-ttu-id="09f23-124">комплетионмонсеар</span><span class="sxs-lookup"><span data-stu-id="09f23-124">completionMonthYear</span></span> |<span data-ttu-id="09f23-125">Дата</span><span class="sxs-lookup"><span data-stu-id="09f23-125">Date</span></span>                                                       |<span data-ttu-id="09f23-126">Месяц и год, когда пользователь выполнит или выполнил действие.</span><span class="sxs-lookup"><span data-stu-id="09f23-126">The month and year the user graduated or completed the activity.</span></span>            |
|<span data-ttu-id="09f23-127">ендмонсеар</span><span class="sxs-lookup"><span data-stu-id="09f23-127">endMonthYear</span></span>        |<span data-ttu-id="09f23-128">Дата</span><span class="sxs-lookup"><span data-stu-id="09f23-128">Date</span></span>                                                       |<span data-ttu-id="09f23-129">Месяц и год, когда пользователь завершил действие учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="09f23-129">The month and year the user completed the educational activity referenced.</span></span>  |
|<span data-ttu-id="09f23-130">Организация</span><span class="sxs-lookup"><span data-stu-id="09f23-130">institution</span></span>         |[<span data-ttu-id="09f23-131">институтиондата</span><span class="sxs-lookup"><span data-stu-id="09f23-131">institutionData</span></span>](institutiondata.md)                      |<span data-ttu-id="09f23-132">Содержит подробные сведения о учебном заведения.</span><span class="sxs-lookup"><span data-stu-id="09f23-132">Contains details of the institution studied at.</span></span>                             |
|<span data-ttu-id="09f23-133">Программа</span><span class="sxs-lookup"><span data-stu-id="09f23-133">program</span></span>             |[<span data-ttu-id="09f23-134">едукатионалактивитидетаил</span><span class="sxs-lookup"><span data-stu-id="09f23-134">educationalActivityDetail</span></span>](educationalactivitydetail.md)  |<span data-ttu-id="09f23-135">Содержит расширенные сведения о программе или курсе.</span><span class="sxs-lookup"><span data-stu-id="09f23-135">Contains extended information about the program or course.</span></span>                  |
|<span data-ttu-id="09f23-136">стартмонсеар</span><span class="sxs-lookup"><span data-stu-id="09f23-136">startMonthYear</span></span>      |<span data-ttu-id="09f23-137">Дата</span><span class="sxs-lookup"><span data-stu-id="09f23-137">Date</span></span>                                                       |<span data-ttu-id="09f23-138">Месяц и год, когда пользователь присвоено указанному действию.</span><span class="sxs-lookup"><span data-stu-id="09f23-138">The month and year the user commenced the activity referenced.</span></span>              |

## <a name="relationships"></a><span data-ttu-id="09f23-139">Связи</span><span class="sxs-lookup"><span data-stu-id="09f23-139">Relationships</span></span>

<span data-ttu-id="09f23-140">Нет</span><span class="sxs-lookup"><span data-stu-id="09f23-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09f23-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="09f23-141">JSON representation</span></span>

<span data-ttu-id="09f23-142">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="09f23-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationalActivity",
  "baseType": ""
}-->

```json
{
  "completionMonthYear": "String (timestamp)",
  "endMonthYear": "String (timestamp)",
  "institution": {"@odata.type": "microsoft.graph.institutionData"},
  "program": {"@odata.type": "microsoft.graph.educationalActivityDetail"},
  "startMonthYear": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationalActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->