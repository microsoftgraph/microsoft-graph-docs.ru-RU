---
title: Тип ресурса educationStudent
description: Добавляются дополнительные сведения в файл educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 554763d41c4ce48a09334394330e05fcd6dd4152
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507137"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="db698-103">Тип ресурса educationStudent</span><span class="sxs-lookup"><span data-stu-id="db698-103">educationStudent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db698-104">Добавляются дополнительные сведения в файл [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `student`.</span><span class="sxs-lookup"><span data-stu-id="db698-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="db698-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="db698-105">Properties</span></span>
| <span data-ttu-id="db698-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="db698-106">Property</span></span>     | <span data-ttu-id="db698-107">Тип</span><span class="sxs-lookup"><span data-stu-id="db698-107">Type</span></span>   |<span data-ttu-id="db698-108">Описание</span><span class="sxs-lookup"><span data-stu-id="db698-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db698-109">birthDate</span><span class="sxs-lookup"><span data-stu-id="db698-109">birthDate</span></span>|<span data-ttu-id="db698-110">Date</span><span class="sxs-lookup"><span data-stu-id="db698-110">Date</span></span>| <span data-ttu-id="db698-111">Дата рождения учащегося.</span><span class="sxs-lookup"><span data-stu-id="db698-111">Birth date of the student.</span></span>|
|<span data-ttu-id="db698-112">externalId</span><span class="sxs-lookup"><span data-stu-id="db698-112">externalId</span></span>|<span data-ttu-id="db698-113">String</span><span class="sxs-lookup"><span data-stu-id="db698-113">String</span></span>| <span data-ttu-id="db698-114">Идентификатор учащегося в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="db698-114">ID of the student in the source system.</span></span>|
|<span data-ttu-id="db698-115">gender</span><span class="sxs-lookup"><span data-stu-id="db698-115">gender</span></span>|<span data-ttu-id="db698-116">Едукатионжендер</span><span class="sxs-lookup"><span data-stu-id="db698-116">educationGender</span></span>| <span data-ttu-id="db698-117">Возможные значения: `female`, `male`, `other`, `unkownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="db698-117">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="db698-118">оценка</span><span class="sxs-lookup"><span data-stu-id="db698-118">grade</span></span>|<span data-ttu-id="db698-119">String</span><span class="sxs-lookup"><span data-stu-id="db698-119">String</span></span>|<span data-ttu-id="db698-120">Текущий уровень оценок учащегося.</span><span class="sxs-lookup"><span data-stu-id="db698-120">Current grade level of the student.</span></span>|
|<span data-ttu-id="db698-121">graduationYear</span><span class="sxs-lookup"><span data-stu-id="db698-121">graduationYear</span></span>|<span data-ttu-id="db698-122">String</span><span class="sxs-lookup"><span data-stu-id="db698-122">String</span></span>| <span data-ttu-id="db698-123">Год выпуска учащегося из школы.</span><span class="sxs-lookup"><span data-stu-id="db698-123">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="db698-124">studentNumber</span><span class="sxs-lookup"><span data-stu-id="db698-124">studentNumber</span></span>|<span data-ttu-id="db698-125">String</span><span class="sxs-lookup"><span data-stu-id="db698-125">String</span></span>| <span data-ttu-id="db698-126">Student Number.</span><span class="sxs-lookup"><span data-stu-id="db698-126">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db698-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db698-127">JSON representation</span></span>

<span data-ttu-id="db698-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db698-128">The following is a JSON representation of the resource.</span></span>

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
