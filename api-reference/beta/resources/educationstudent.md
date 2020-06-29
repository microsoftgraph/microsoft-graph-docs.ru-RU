---
title: Тип ресурса educationStudent
description: Добавляются дополнительные сведения в файл educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e64899cf56140246373c36428518ebd28bb136c7
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909725"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="9fdd4-103">Тип ресурса educationStudent</span><span class="sxs-lookup"><span data-stu-id="9fdd4-103">educationStudent resource type</span></span>

<span data-ttu-id="9fdd4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fdd4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fdd4-105">Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `student`.</span><span class="sxs-lookup"><span data-stu-id="9fdd4-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="9fdd4-106">При использовании делегированных областей разрешений Graph будет возвращать только `externalId` Свойства.</span><span class="sxs-lookup"><span data-stu-id="9fdd4-106">When using Delegated permission scopes, Graph will only return the `externalId` properties.</span></span> <span data-ttu-id="9fdd4-107">Для всех остальных свойств требуются области применения.</span><span class="sxs-lookup"><span data-stu-id="9fdd4-107">All other properties require Application scopes.</span></span>

## <a name="properties"></a><span data-ttu-id="9fdd4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9fdd4-108">Properties</span></span>

| <span data-ttu-id="9fdd4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9fdd4-109">Property</span></span>       | <span data-ttu-id="9fdd4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9fdd4-110">Type</span></span>            | <span data-ttu-id="9fdd4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9fdd4-111">Description</span></span>                                     |
| :------------- | :-------------- | :---------------------------------------------- |
| <span data-ttu-id="9fdd4-112">birthDate</span><span class="sxs-lookup"><span data-stu-id="9fdd4-112">birthDate</span></span>      | <span data-ttu-id="9fdd4-113">Date</span><span class="sxs-lookup"><span data-stu-id="9fdd4-113">Date</span></span>            | <span data-ttu-id="9fdd4-114">Дата рождения учащегося.</span><span class="sxs-lookup"><span data-stu-id="9fdd4-114">Birth date of the student.</span></span>                      |
| <span data-ttu-id="9fdd4-115">externalId</span><span class="sxs-lookup"><span data-stu-id="9fdd4-115">externalId</span></span>     | <span data-ttu-id="9fdd4-116">String</span><span class="sxs-lookup"><span data-stu-id="9fdd4-116">String</span></span>          | <span data-ttu-id="9fdd4-117">Идентификатор учащегося в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="9fdd4-117">ID of the student in the source system.</span></span>         |
| <span data-ttu-id="9fdd4-118">gender</span><span class="sxs-lookup"><span data-stu-id="9fdd4-118">gender</span></span>         | <span data-ttu-id="9fdd4-119">едукатионжендер</span><span class="sxs-lookup"><span data-stu-id="9fdd4-119">educationGender</span></span> | <span data-ttu-id="9fdd4-120">Возможные значения: `female`, `male`, `other`.</span><span class="sxs-lookup"><span data-stu-id="9fdd4-120">Possible values are: `female`, `male`, `other`.</span></span> |
| <span data-ttu-id="9fdd4-121">оценка</span><span class="sxs-lookup"><span data-stu-id="9fdd4-121">grade</span></span>          | <span data-ttu-id="9fdd4-122">String</span><span class="sxs-lookup"><span data-stu-id="9fdd4-122">String</span></span>          | <span data-ttu-id="9fdd4-123">Текущий уровень оценок учащегося.</span><span class="sxs-lookup"><span data-stu-id="9fdd4-123">Current grade level of the student.</span></span>             |
| <span data-ttu-id="9fdd4-124">graduationYear</span><span class="sxs-lookup"><span data-stu-id="9fdd4-124">graduationYear</span></span> | <span data-ttu-id="9fdd4-125">String</span><span class="sxs-lookup"><span data-stu-id="9fdd4-125">String</span></span>          | <span data-ttu-id="9fdd4-126">Год выпуска учащегося из школы.</span><span class="sxs-lookup"><span data-stu-id="9fdd4-126">Year the student is graduating from the school.</span></span> |
| <span data-ttu-id="9fdd4-127">studentNumber</span><span class="sxs-lookup"><span data-stu-id="9fdd4-127">studentNumber</span></span>  | <span data-ttu-id="9fdd4-128">String</span><span class="sxs-lookup"><span data-stu-id="9fdd4-128">String</span></span>          | <span data-ttu-id="9fdd4-129">Student Number.</span><span class="sxs-lookup"><span data-stu-id="9fdd4-129">Student Number.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="9fdd4-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9fdd4-130">JSON representation</span></span>

<span data-ttu-id="9fdd4-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9fdd4-131">The following is a JSON representation of the resource.</span></span>

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
