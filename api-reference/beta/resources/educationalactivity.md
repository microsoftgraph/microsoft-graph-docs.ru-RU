---
title: Тип ресурса Едукатионалактивити
description: Тип ресурса Едукатионалактивити
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 8d060de55d765adb7e01e6b03842c569f03c8d4f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939623"
---
# <a name="educationalactivity-resource-type"></a><span data-ttu-id="d187d-103">Тип ресурса Едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="d187d-103">educationalActivity resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d187d-104">Представляет данные, которые пользователь предоставил, относящихся к выпуску, выпускнику, выпуску или другим учебным действиям.</span><span class="sxs-lookup"><span data-stu-id="d187d-104">Represents data that a user has supplied related to undergraduate, graduate, postgraduate or other educational activities.</span></span>

<span data-ttu-id="d187d-105">Наследует свойства метаданных от [итемфацет](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="d187d-105">Inherits metadata properties from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d187d-106">Методы</span><span class="sxs-lookup"><span data-stu-id="d187d-106">Methods</span></span>

| <span data-ttu-id="d187d-107">Метод</span><span class="sxs-lookup"><span data-stu-id="d187d-107">Method</span></span>                                                       | <span data-ttu-id="d187d-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d187d-108">Return Type</span></span>                                   | <span data-ttu-id="d187d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d187d-109">Description</span></span>                                                      |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="d187d-110">Получение Едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="d187d-110">Get educationalActivity</span></span>](../api/educationalactivity-get.md) | [<span data-ttu-id="d187d-111">едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="d187d-111">educationalActivity</span></span>](educationalactivity.md) | <span data-ttu-id="d187d-112">Чтение свойств и связей объекта Едукатионалактивити.</span><span class="sxs-lookup"><span data-stu-id="d187d-112">Read properties and relationships of educationalActivity object.</span></span> |
| [<span data-ttu-id="d187d-113">Update</span><span class="sxs-lookup"><span data-stu-id="d187d-113">Update</span></span>](../api/educationalactivity-update.md)               | [<span data-ttu-id="d187d-114">едукатионалактивити</span><span class="sxs-lookup"><span data-stu-id="d187d-114">educationalActivity</span></span>](educationalactivity.md) | <span data-ttu-id="d187d-115">Обновление объекта Едукатионалактивити.</span><span class="sxs-lookup"><span data-stu-id="d187d-115">Update educationalActivity object.</span></span>                               |
| [<span data-ttu-id="d187d-116">Delete</span><span class="sxs-lookup"><span data-stu-id="d187d-116">Delete</span></span>](../api/educationalactivity-delete.md)               | <span data-ttu-id="d187d-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="d187d-117">None</span></span>                                          | <span data-ttu-id="d187d-118">Удаление объекта Едукатионалактивити.</span><span class="sxs-lookup"><span data-stu-id="d187d-118">Delete educationalActivity object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="d187d-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="d187d-119">Properties</span></span>

| <span data-ttu-id="d187d-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="d187d-120">Property</span></span>           | <span data-ttu-id="d187d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="d187d-121">Type</span></span>                                                      | <span data-ttu-id="d187d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d187d-122">Description</span></span>                                                                |
|:-------------------|:----------------------------------------------------------|:---------------------------------------------------------------------------|
|<span data-ttu-id="d187d-123">комплетионмонсеар</span><span class="sxs-lookup"><span data-stu-id="d187d-123">completionMonthYear</span></span> |<span data-ttu-id="d187d-124">Дата</span><span class="sxs-lookup"><span data-stu-id="d187d-124">Date</span></span>                                                       |<span data-ttu-id="d187d-125">Месяц и год, когда пользователь выполнит или выполнил действие.</span><span class="sxs-lookup"><span data-stu-id="d187d-125">The month and year the user graduated or completed the activity.</span></span>            |
|<span data-ttu-id="d187d-126">ендмонсеар</span><span class="sxs-lookup"><span data-stu-id="d187d-126">endMonthYear</span></span>        |<span data-ttu-id="d187d-127">Дата</span><span class="sxs-lookup"><span data-stu-id="d187d-127">Date</span></span>                                                       |<span data-ttu-id="d187d-128">Месяц и год, когда пользователь завершил действие учебного заведения.</span><span class="sxs-lookup"><span data-stu-id="d187d-128">The month and year the user completed the educational activity referenced.</span></span>  |
|<span data-ttu-id="d187d-129">Организация</span><span class="sxs-lookup"><span data-stu-id="d187d-129">institution</span></span>         |[<span data-ttu-id="d187d-130">институтиондата</span><span class="sxs-lookup"><span data-stu-id="d187d-130">institutionData</span></span>](institutiondata.md)                      |<span data-ttu-id="d187d-131">Содержит подробные сведения о учебном заведения.</span><span class="sxs-lookup"><span data-stu-id="d187d-131">Contains details of the institution studied at.</span></span>                             |
|<span data-ttu-id="d187d-132">Программа</span><span class="sxs-lookup"><span data-stu-id="d187d-132">program</span></span>             |[<span data-ttu-id="d187d-133">едукатионалактивитидетаил</span><span class="sxs-lookup"><span data-stu-id="d187d-133">educationalActivityDetail</span></span>](educationalactivitydetail.md)  |<span data-ttu-id="d187d-134">Содержит расширенные сведения о программе или курсе.</span><span class="sxs-lookup"><span data-stu-id="d187d-134">Contains extended information about the program or course.</span></span>                  |
|<span data-ttu-id="d187d-135">стартмонсеар</span><span class="sxs-lookup"><span data-stu-id="d187d-135">startMonthYear</span></span>      |<span data-ttu-id="d187d-136">Дата</span><span class="sxs-lookup"><span data-stu-id="d187d-136">Date</span></span>                                                       |<span data-ttu-id="d187d-137">Месяц и год, когда пользователь присвоено указанному действию.</span><span class="sxs-lookup"><span data-stu-id="d187d-137">The month and year the user commenced the activity referenced.</span></span>              |

## <a name="relationships"></a><span data-ttu-id="d187d-138">Связи</span><span class="sxs-lookup"><span data-stu-id="d187d-138">Relationships</span></span>

<span data-ttu-id="d187d-139">Нет</span><span class="sxs-lookup"><span data-stu-id="d187d-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d187d-140">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d187d-140">JSON representation</span></span>

<span data-ttu-id="d187d-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d187d-141">The following is a JSON representation of the resource.</span></span>

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