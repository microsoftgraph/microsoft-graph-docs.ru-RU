---
title: Тип ресурса educationStudent
description: Добавляются дополнительные сведения в файл educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b6f6cf8e8a79c427403c2f2157228c8ce130b313
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913312"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="36021-103">Тип ресурса educationStudent</span><span class="sxs-lookup"><span data-stu-id="36021-103">educationStudent resource type</span></span>

> <span data-ttu-id="36021-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="36021-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="36021-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36021-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="36021-106">Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `student`.</span><span class="sxs-lookup"><span data-stu-id="36021-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="36021-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="36021-107">Properties</span></span>
| <span data-ttu-id="36021-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="36021-108">Property</span></span>     | <span data-ttu-id="36021-109">Тип</span><span class="sxs-lookup"><span data-stu-id="36021-109">Type</span></span>   |<span data-ttu-id="36021-110">Описание</span><span class="sxs-lookup"><span data-stu-id="36021-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="36021-111">birthDate</span><span class="sxs-lookup"><span data-stu-id="36021-111">birthDate</span></span>|<span data-ttu-id="36021-112">Date</span><span class="sxs-lookup"><span data-stu-id="36021-112">Date</span></span>| <span data-ttu-id="36021-113">Дата рождения учащегося.</span><span class="sxs-lookup"><span data-stu-id="36021-113">Birth date of the student.</span></span>|
|<span data-ttu-id="36021-114">externalId</span><span class="sxs-lookup"><span data-stu-id="36021-114">externalId</span></span>|<span data-ttu-id="36021-115">String</span><span class="sxs-lookup"><span data-stu-id="36021-115">String</span></span>| <span data-ttu-id="36021-116">Идентификатор учащегося в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="36021-116">ID of the student in the source system.</span></span>|
|<span data-ttu-id="36021-117">gender</span><span class="sxs-lookup"><span data-stu-id="36021-117">gender</span></span>|`educationGender enumeration`| <span data-ttu-id="36021-118">Возможные значения: `female`, `male`, `other`, `unkownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="36021-118">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="36021-119">оценка</span><span class="sxs-lookup"><span data-stu-id="36021-119">grade</span></span>|<span data-ttu-id="36021-120">String</span><span class="sxs-lookup"><span data-stu-id="36021-120">String</span></span>|<span data-ttu-id="36021-121">Текущий уровень оценок учащегося.</span><span class="sxs-lookup"><span data-stu-id="36021-121">Current grade level of the student.</span></span>|
|<span data-ttu-id="36021-122">graduationYear</span><span class="sxs-lookup"><span data-stu-id="36021-122">graduationYear</span></span>|<span data-ttu-id="36021-123">String</span><span class="sxs-lookup"><span data-stu-id="36021-123">String</span></span>| <span data-ttu-id="36021-124">Год выпуска учащегося из школы.</span><span class="sxs-lookup"><span data-stu-id="36021-124">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="36021-125">studentNumber</span><span class="sxs-lookup"><span data-stu-id="36021-125">studentNumber</span></span>|<span data-ttu-id="36021-126">String</span><span class="sxs-lookup"><span data-stu-id="36021-126">String</span></span>| <span data-ttu-id="36021-127">Student Number.</span><span class="sxs-lookup"><span data-stu-id="36021-127">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="36021-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="36021-128">JSON representation</span></span>

<span data-ttu-id="36021-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="36021-129">The following is a JSON representation of the resource.</span></span>

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
