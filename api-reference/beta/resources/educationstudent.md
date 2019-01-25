---
title: Тип ресурса educationStudent
description: Добавляются дополнительные сведения в файл `student`, который присутствует, когда значение параметра primaryRole для пользователя — .
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 554763d41c4ce48a09334394330e05fcd6dd4152
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522037"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="40fdf-103">Тип ресурса educationStudent</span><span class="sxs-lookup"><span data-stu-id="40fdf-103">educationStudent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40fdf-104">Добавляются дополнительные сведения в файл [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `student`.</span><span class="sxs-lookup"><span data-stu-id="40fdf-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="40fdf-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="40fdf-105">Properties</span></span>
| <span data-ttu-id="40fdf-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="40fdf-106">Property</span></span>     | <span data-ttu-id="40fdf-107">Тип</span><span class="sxs-lookup"><span data-stu-id="40fdf-107">Type</span></span>   |<span data-ttu-id="40fdf-108">Описание</span><span class="sxs-lookup"><span data-stu-id="40fdf-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="40fdf-109">birthDate</span><span class="sxs-lookup"><span data-stu-id="40fdf-109">birthDate</span></span>|<span data-ttu-id="40fdf-110">Date</span><span class="sxs-lookup"><span data-stu-id="40fdf-110">Date</span></span>| <span data-ttu-id="40fdf-111">Дата рождения учащегося.</span><span class="sxs-lookup"><span data-stu-id="40fdf-111">Birth date of the student.</span></span>|
|<span data-ttu-id="40fdf-112">externalId</span><span class="sxs-lookup"><span data-stu-id="40fdf-112">externalId</span></span>|<span data-ttu-id="40fdf-113">String</span><span class="sxs-lookup"><span data-stu-id="40fdf-113">String</span></span>| <span data-ttu-id="40fdf-114">Идентификатор учащегося в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="40fdf-114">ID of the student in the source system.</span></span>|
|<span data-ttu-id="40fdf-115">gender</span><span class="sxs-lookup"><span data-stu-id="40fdf-115">gender</span></span>|<span data-ttu-id="40fdf-116">educationGender</span><span class="sxs-lookup"><span data-stu-id="40fdf-116">educationGender</span></span>| <span data-ttu-id="40fdf-117">Возможные значения: `female`, `male`, `other`, `unkownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="40fdf-117">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="40fdf-118">оценка</span><span class="sxs-lookup"><span data-stu-id="40fdf-118">grade</span></span>|<span data-ttu-id="40fdf-119">String</span><span class="sxs-lookup"><span data-stu-id="40fdf-119">String</span></span>|<span data-ttu-id="40fdf-120">Текущий уровень оценок учащегося.</span><span class="sxs-lookup"><span data-stu-id="40fdf-120">Current grade level of the student.</span></span>|
|<span data-ttu-id="40fdf-121">graduationYear</span><span class="sxs-lookup"><span data-stu-id="40fdf-121">graduationYear</span></span>|<span data-ttu-id="40fdf-122">String</span><span class="sxs-lookup"><span data-stu-id="40fdf-122">String</span></span>| <span data-ttu-id="40fdf-123">Год выпуска учащегося из школы.</span><span class="sxs-lookup"><span data-stu-id="40fdf-123">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="40fdf-124">studentNumber</span><span class="sxs-lookup"><span data-stu-id="40fdf-124">studentNumber</span></span>|<span data-ttu-id="40fdf-125">String</span><span class="sxs-lookup"><span data-stu-id="40fdf-125">String</span></span>| <span data-ttu-id="40fdf-126">Student Number.</span><span class="sxs-lookup"><span data-stu-id="40fdf-126">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="40fdf-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40fdf-127">JSON representation</span></span>

<span data-ttu-id="40fdf-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40fdf-128">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationstudent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
