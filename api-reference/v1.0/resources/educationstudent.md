---
title: Тип ресурса educationStudent
description: Добавляются дополнительные сведения в файл educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 2b8574d790094468d4a74ab5796c18e26b696540
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030494"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="29f1f-103">Тип ресурса educationStudent</span><span class="sxs-lookup"><span data-stu-id="29f1f-103">educationStudent resource type</span></span>

<span data-ttu-id="29f1f-104">Добавляются дополнительные сведения в файл [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `student`.</span><span class="sxs-lookup"><span data-stu-id="29f1f-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="29f1f-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="29f1f-105">Properties</span></span>
| <span data-ttu-id="29f1f-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="29f1f-106">Property</span></span>     | <span data-ttu-id="29f1f-107">Тип</span><span class="sxs-lookup"><span data-stu-id="29f1f-107">Type</span></span>   |<span data-ttu-id="29f1f-108">Описание</span><span class="sxs-lookup"><span data-stu-id="29f1f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29f1f-109">birthDate</span><span class="sxs-lookup"><span data-stu-id="29f1f-109">birthDate</span></span>|<span data-ttu-id="29f1f-110">Date</span><span class="sxs-lookup"><span data-stu-id="29f1f-110">Date</span></span>| <span data-ttu-id="29f1f-111">Дата рождения учащегося.</span><span class="sxs-lookup"><span data-stu-id="29f1f-111">Birth date of the student.</span></span>|
|<span data-ttu-id="29f1f-112">externalId</span><span class="sxs-lookup"><span data-stu-id="29f1f-112">externalId</span></span>|<span data-ttu-id="29f1f-113">String</span><span class="sxs-lookup"><span data-stu-id="29f1f-113">String</span></span>| <span data-ttu-id="29f1f-114">Идентификатор учащегося в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="29f1f-114">ID of the student in the source system.</span></span>|
|<span data-ttu-id="29f1f-115">gender</span><span class="sxs-lookup"><span data-stu-id="29f1f-115">gender</span></span>|<span data-ttu-id="29f1f-116">Едукатионжендер</span><span class="sxs-lookup"><span data-stu-id="29f1f-116">educationGender</span></span>| <span data-ttu-id="29f1f-117">Допустимые значения: `female`, `male`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="29f1f-117">The possible values are: `female`, `male`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="29f1f-118">оценка</span><span class="sxs-lookup"><span data-stu-id="29f1f-118">grade</span></span>|<span data-ttu-id="29f1f-119">String</span><span class="sxs-lookup"><span data-stu-id="29f1f-119">String</span></span>|<span data-ttu-id="29f1f-120">Текущий уровень оценок учащегося.</span><span class="sxs-lookup"><span data-stu-id="29f1f-120">Current grade level of the student.</span></span>|
|<span data-ttu-id="29f1f-121">graduationYear</span><span class="sxs-lookup"><span data-stu-id="29f1f-121">graduationYear</span></span>|<span data-ttu-id="29f1f-122">String</span><span class="sxs-lookup"><span data-stu-id="29f1f-122">String</span></span>| <span data-ttu-id="29f1f-123">Год выпуска учащегося из школы.</span><span class="sxs-lookup"><span data-stu-id="29f1f-123">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="29f1f-124">studentNumber</span><span class="sxs-lookup"><span data-stu-id="29f1f-124">studentNumber</span></span>|<span data-ttu-id="29f1f-125">String</span><span class="sxs-lookup"><span data-stu-id="29f1f-125">String</span></span>| <span data-ttu-id="29f1f-126">Student Number.</span><span class="sxs-lookup"><span data-stu-id="29f1f-126">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29f1f-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="29f1f-127">JSON representation</span></span>

<span data-ttu-id="29f1f-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29f1f-128">The following is a JSON representation of the resource.</span></span>

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
