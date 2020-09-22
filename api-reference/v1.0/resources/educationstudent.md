---
title: Тип ресурса educationStudent
description: Добавляются дополнительные сведения в файл educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c8cc053900a774f6a79bcabb5350a840959aeeb1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032622"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="69923-103">Тип ресурса educationStudent</span><span class="sxs-lookup"><span data-stu-id="69923-103">educationStudent resource type</span></span>

<span data-ttu-id="69923-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69923-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="69923-105">Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `student`.</span><span class="sxs-lookup"><span data-stu-id="69923-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="69923-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="69923-106">Properties</span></span>
| <span data-ttu-id="69923-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="69923-107">Property</span></span>     | <span data-ttu-id="69923-108">Тип</span><span class="sxs-lookup"><span data-stu-id="69923-108">Type</span></span>   |<span data-ttu-id="69923-109">Описание</span><span class="sxs-lookup"><span data-stu-id="69923-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69923-110">birthDate</span><span class="sxs-lookup"><span data-stu-id="69923-110">birthDate</span></span>|<span data-ttu-id="69923-111">Date</span><span class="sxs-lookup"><span data-stu-id="69923-111">Date</span></span>| <span data-ttu-id="69923-112">Дата рождения учащегося.</span><span class="sxs-lookup"><span data-stu-id="69923-112">Birth date of the student.</span></span>|
|<span data-ttu-id="69923-113">externalId</span><span class="sxs-lookup"><span data-stu-id="69923-113">externalId</span></span>|<span data-ttu-id="69923-114">String</span><span class="sxs-lookup"><span data-stu-id="69923-114">String</span></span>| <span data-ttu-id="69923-115">Идентификатор учащегося в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="69923-115">ID of the student in the source system.</span></span>|
|<span data-ttu-id="69923-116">gender</span><span class="sxs-lookup"><span data-stu-id="69923-116">gender</span></span>|<span data-ttu-id="69923-117">едукатионжендер</span><span class="sxs-lookup"><span data-stu-id="69923-117">educationGender</span></span>| <span data-ttu-id="69923-118">Допустимые значения: `female`, `male`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="69923-118">The possible values are: `female`, `male`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="69923-119">оценка</span><span class="sxs-lookup"><span data-stu-id="69923-119">grade</span></span>|<span data-ttu-id="69923-120">String</span><span class="sxs-lookup"><span data-stu-id="69923-120">String</span></span>|<span data-ttu-id="69923-121">Текущий уровень оценок учащегося.</span><span class="sxs-lookup"><span data-stu-id="69923-121">Current grade level of the student.</span></span>|
|<span data-ttu-id="69923-122">graduationYear</span><span class="sxs-lookup"><span data-stu-id="69923-122">graduationYear</span></span>|<span data-ttu-id="69923-123">String</span><span class="sxs-lookup"><span data-stu-id="69923-123">String</span></span>| <span data-ttu-id="69923-124">Год выпуска учащегося из школы.</span><span class="sxs-lookup"><span data-stu-id="69923-124">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="69923-125">studentNumber</span><span class="sxs-lookup"><span data-stu-id="69923-125">studentNumber</span></span>|<span data-ttu-id="69923-126">String</span><span class="sxs-lookup"><span data-stu-id="69923-126">String</span></span>| <span data-ttu-id="69923-127">Student Number.</span><span class="sxs-lookup"><span data-stu-id="69923-127">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="69923-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="69923-128">JSON representation</span></span>

<span data-ttu-id="69923-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="69923-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationStudent"
}-->

```json
{
  "birthDate": "String (timestamp)",
  "externalId": "String",
  "gender": "educationGender",
  "grade": "String",
  "graduationYear": "String",
  "studentNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

