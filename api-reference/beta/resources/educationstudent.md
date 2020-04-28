---
title: Тип ресурса educationStudent
description: Добавляются дополнительные сведения в файл educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9b8f2de9f3b40a72aab7f9273b9b4fc30594059b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500767"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="fc9d1-103">Тип ресурса educationStudent</span><span class="sxs-lookup"><span data-stu-id="fc9d1-103">educationStudent resource type</span></span>

<span data-ttu-id="fc9d1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc9d1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc9d1-105">Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `student`.</span><span class="sxs-lookup"><span data-stu-id="fc9d1-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="fc9d1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc9d1-106">Properties</span></span>
| <span data-ttu-id="fc9d1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc9d1-107">Property</span></span>     | <span data-ttu-id="fc9d1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fc9d1-108">Type</span></span>   |<span data-ttu-id="fc9d1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fc9d1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc9d1-110">birthDate</span><span class="sxs-lookup"><span data-stu-id="fc9d1-110">birthDate</span></span>|<span data-ttu-id="fc9d1-111">Date</span><span class="sxs-lookup"><span data-stu-id="fc9d1-111">Date</span></span>| <span data-ttu-id="fc9d1-112">Дата рождения учащегося.</span><span class="sxs-lookup"><span data-stu-id="fc9d1-112">Birth date of the student.</span></span>|
|<span data-ttu-id="fc9d1-113">externalId</span><span class="sxs-lookup"><span data-stu-id="fc9d1-113">externalId</span></span>|<span data-ttu-id="fc9d1-114">String</span><span class="sxs-lookup"><span data-stu-id="fc9d1-114">String</span></span>| <span data-ttu-id="fc9d1-115">Идентификатор учащегося в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="fc9d1-115">ID of the student in the source system.</span></span>|
|<span data-ttu-id="fc9d1-116">gender</span><span class="sxs-lookup"><span data-stu-id="fc9d1-116">gender</span></span>|<span data-ttu-id="fc9d1-117">едукатионжендер</span><span class="sxs-lookup"><span data-stu-id="fc9d1-117">educationGender</span></span>| <span data-ttu-id="fc9d1-118">Возможные значения: `female`, `male`, `other`.</span><span class="sxs-lookup"><span data-stu-id="fc9d1-118">Possible values are: `female`, `male`, `other`.</span></span>|
|<span data-ttu-id="fc9d1-119">оценка</span><span class="sxs-lookup"><span data-stu-id="fc9d1-119">grade</span></span>|<span data-ttu-id="fc9d1-120">String</span><span class="sxs-lookup"><span data-stu-id="fc9d1-120">String</span></span>|<span data-ttu-id="fc9d1-121">Текущий уровень оценок учащегося.</span><span class="sxs-lookup"><span data-stu-id="fc9d1-121">Current grade level of the student.</span></span>|
|<span data-ttu-id="fc9d1-122">graduationYear</span><span class="sxs-lookup"><span data-stu-id="fc9d1-122">graduationYear</span></span>|<span data-ttu-id="fc9d1-123">String</span><span class="sxs-lookup"><span data-stu-id="fc9d1-123">String</span></span>| <span data-ttu-id="fc9d1-124">Год выпуска учащегося из школы.</span><span class="sxs-lookup"><span data-stu-id="fc9d1-124">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="fc9d1-125">studentNumber</span><span class="sxs-lookup"><span data-stu-id="fc9d1-125">studentNumber</span></span>|<span data-ttu-id="fc9d1-126">String</span><span class="sxs-lookup"><span data-stu-id="fc9d1-126">String</span></span>| <span data-ttu-id="fc9d1-127">Student Number.</span><span class="sxs-lookup"><span data-stu-id="fc9d1-127">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fc9d1-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc9d1-128">JSON representation</span></span>

<span data-ttu-id="fc9d1-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc9d1-129">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
