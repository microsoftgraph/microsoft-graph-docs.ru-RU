---
title: Тип ресурса educationStudent
description: Добавляются дополнительные сведения в файл educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `student`.
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: f87bbe9b15f89660a166c0ca1d9a1aaa4bbd9eff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878122"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="41125-103">Тип ресурса educationStudent</span><span class="sxs-lookup"><span data-stu-id="41125-103">educationStudent resource type</span></span>

> <span data-ttu-id="41125-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="41125-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41125-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41125-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="41125-106">Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `student`.</span><span class="sxs-lookup"><span data-stu-id="41125-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="41125-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="41125-107">Properties</span></span>
| <span data-ttu-id="41125-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="41125-108">Property</span></span>     | <span data-ttu-id="41125-109">Тип</span><span class="sxs-lookup"><span data-stu-id="41125-109">Type</span></span>   |<span data-ttu-id="41125-110">Описание</span><span class="sxs-lookup"><span data-stu-id="41125-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41125-111">birthDate</span><span class="sxs-lookup"><span data-stu-id="41125-111">birthDate</span></span>|<span data-ttu-id="41125-112">Date</span><span class="sxs-lookup"><span data-stu-id="41125-112">Date</span></span>| <span data-ttu-id="41125-113">Дата рождения учащегося.</span><span class="sxs-lookup"><span data-stu-id="41125-113">Birth date of the student.</span></span>|
|<span data-ttu-id="41125-114">externalId</span><span class="sxs-lookup"><span data-stu-id="41125-114">externalId</span></span>|<span data-ttu-id="41125-115">String</span><span class="sxs-lookup"><span data-stu-id="41125-115">String</span></span>| <span data-ttu-id="41125-116">Идентификатор учащегося в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="41125-116">ID of the student in the source system.</span></span>|
|<span data-ttu-id="41125-117">gender</span><span class="sxs-lookup"><span data-stu-id="41125-117">gender</span></span>|`educationGender enumeration`| <span data-ttu-id="41125-118">Возможные значения: `female`, `male`, `other`, `unkownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="41125-118">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="41125-119">оценка</span><span class="sxs-lookup"><span data-stu-id="41125-119">grade</span></span>|<span data-ttu-id="41125-120">String</span><span class="sxs-lookup"><span data-stu-id="41125-120">String</span></span>|<span data-ttu-id="41125-121">Текущий уровень оценок учащегося.</span><span class="sxs-lookup"><span data-stu-id="41125-121">Current grade level of the student.</span></span>|
|<span data-ttu-id="41125-122">graduationYear</span><span class="sxs-lookup"><span data-stu-id="41125-122">graduationYear</span></span>|<span data-ttu-id="41125-123">String</span><span class="sxs-lookup"><span data-stu-id="41125-123">String</span></span>| <span data-ttu-id="41125-124">Год выпуска учащегося из школы.</span><span class="sxs-lookup"><span data-stu-id="41125-124">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="41125-125">studentNumber</span><span class="sxs-lookup"><span data-stu-id="41125-125">studentNumber</span></span>|<span data-ttu-id="41125-126">String</span><span class="sxs-lookup"><span data-stu-id="41125-126">String</span></span>| <span data-ttu-id="41125-127">Student Number.</span><span class="sxs-lookup"><span data-stu-id="41125-127">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="41125-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="41125-128">JSON representation</span></span>

<span data-ttu-id="41125-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41125-129">The following is a JSON representation of the resource.</span></span>

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
