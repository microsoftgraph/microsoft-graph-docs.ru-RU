---
title: Тип ресурса educationStudent
description: Добавляются дополнительные сведения в файл educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 355230339129a351f5a609292e7e7623a39a59b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049739"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="bcf4c-103">Тип ресурса educationStudent</span><span class="sxs-lookup"><span data-stu-id="bcf4c-103">educationStudent resource type</span></span>

<span data-ttu-id="bcf4c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bcf4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bcf4c-105">Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `student`.</span><span class="sxs-lookup"><span data-stu-id="bcf4c-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="bcf4c-106">При использовании делегированных областей разрешений Graph будет возвращать только `externalId` Свойства.</span><span class="sxs-lookup"><span data-stu-id="bcf4c-106">When using Delegated permission scopes, Graph will only return the `externalId` properties.</span></span> <span data-ttu-id="bcf4c-107">Для всех остальных свойств требуются области применения.</span><span class="sxs-lookup"><span data-stu-id="bcf4c-107">All other properties require Application scopes.</span></span>

## <a name="properties"></a><span data-ttu-id="bcf4c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bcf4c-108">Properties</span></span>

| <span data-ttu-id="bcf4c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bcf4c-109">Property</span></span>       | <span data-ttu-id="bcf4c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bcf4c-110">Type</span></span>            | <span data-ttu-id="bcf4c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bcf4c-111">Description</span></span>                                     |
| :------------- | :-------------- | :---------------------------------------------- |
| <span data-ttu-id="bcf4c-112">birthDate</span><span class="sxs-lookup"><span data-stu-id="bcf4c-112">birthDate</span></span>      | <span data-ttu-id="bcf4c-113">Date</span><span class="sxs-lookup"><span data-stu-id="bcf4c-113">Date</span></span>            | <span data-ttu-id="bcf4c-114">Дата рождения учащегося.</span><span class="sxs-lookup"><span data-stu-id="bcf4c-114">Birth date of the student.</span></span>                      |
| <span data-ttu-id="bcf4c-115">externalId</span><span class="sxs-lookup"><span data-stu-id="bcf4c-115">externalId</span></span>     | <span data-ttu-id="bcf4c-116">String</span><span class="sxs-lookup"><span data-stu-id="bcf4c-116">String</span></span>          | <span data-ttu-id="bcf4c-117">Идентификатор учащегося в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="bcf4c-117">ID of the student in the source system.</span></span>         |
| <span data-ttu-id="bcf4c-118">gender</span><span class="sxs-lookup"><span data-stu-id="bcf4c-118">gender</span></span>         | <span data-ttu-id="bcf4c-119">едукатионжендер</span><span class="sxs-lookup"><span data-stu-id="bcf4c-119">educationGender</span></span> | <span data-ttu-id="bcf4c-120">Возможные значения: `female`, `male`, `other`.</span><span class="sxs-lookup"><span data-stu-id="bcf4c-120">Possible values are: `female`, `male`, `other`.</span></span> |
| <span data-ttu-id="bcf4c-121">оценка</span><span class="sxs-lookup"><span data-stu-id="bcf4c-121">grade</span></span>          | <span data-ttu-id="bcf4c-122">String</span><span class="sxs-lookup"><span data-stu-id="bcf4c-122">String</span></span>          | <span data-ttu-id="bcf4c-123">Текущий уровень оценок учащегося.</span><span class="sxs-lookup"><span data-stu-id="bcf4c-123">Current grade level of the student.</span></span>             |
| <span data-ttu-id="bcf4c-124">graduationYear</span><span class="sxs-lookup"><span data-stu-id="bcf4c-124">graduationYear</span></span> | <span data-ttu-id="bcf4c-125">String</span><span class="sxs-lookup"><span data-stu-id="bcf4c-125">String</span></span>          | <span data-ttu-id="bcf4c-126">Год выпуска учащегося из школы.</span><span class="sxs-lookup"><span data-stu-id="bcf4c-126">Year the student is graduating from the school.</span></span> |
| <span data-ttu-id="bcf4c-127">studentNumber</span><span class="sxs-lookup"><span data-stu-id="bcf4c-127">studentNumber</span></span>  | <span data-ttu-id="bcf4c-128">String</span><span class="sxs-lookup"><span data-stu-id="bcf4c-128">String</span></span>          | <span data-ttu-id="bcf4c-129">Student Number.</span><span class="sxs-lookup"><span data-stu-id="bcf4c-129">Student Number.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="bcf4c-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bcf4c-130">JSON representation</span></span>

<span data-ttu-id="bcf4c-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bcf4c-131">The following is a JSON representation of the resource.</span></span>

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


