---
title: Тип ресурса educationStudent
description: Добавляются дополнительные сведения в файл educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `student`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5b0e154beb5b8133c69392af8fa9611263c68945
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231852"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="b93e4-103">Тип ресурса educationStudent</span><span class="sxs-lookup"><span data-stu-id="b93e4-103">educationStudent resource type</span></span>

<span data-ttu-id="b93e4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b93e4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b93e4-105">Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `student`.</span><span class="sxs-lookup"><span data-stu-id="b93e4-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="b93e4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b93e4-106">Properties</span></span>

| <span data-ttu-id="b93e4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b93e4-107">Property</span></span>       | <span data-ttu-id="b93e4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b93e4-108">Type</span></span>            | <span data-ttu-id="b93e4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b93e4-109">Description</span></span>                                                               |
| :------------- | :-------------- | :------------------------------------------------------------------------ |
| <span data-ttu-id="b93e4-110">birthDate</span><span class="sxs-lookup"><span data-stu-id="b93e4-110">birthDate</span></span>      | <span data-ttu-id="b93e4-111">Date</span><span class="sxs-lookup"><span data-stu-id="b93e4-111">Date</span></span>            | <span data-ttu-id="b93e4-112">Дата рождения учащегося.</span><span class="sxs-lookup"><span data-stu-id="b93e4-112">Birth date of the student.</span></span>                                                |
| <span data-ttu-id="b93e4-113">externalId</span><span class="sxs-lookup"><span data-stu-id="b93e4-113">externalId</span></span>     | <span data-ttu-id="b93e4-114">String</span><span class="sxs-lookup"><span data-stu-id="b93e4-114">String</span></span>          | <span data-ttu-id="b93e4-115">Идентификатор учащегося в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="b93e4-115">ID of the student in the source system.</span></span>                                   |
| <span data-ttu-id="b93e4-116">gender</span><span class="sxs-lookup"><span data-stu-id="b93e4-116">gender</span></span>         | <span data-ttu-id="b93e4-117">educationGender</span><span class="sxs-lookup"><span data-stu-id="b93e4-117">educationGender</span></span> | <span data-ttu-id="b93e4-118">Допустимые значения: `female`, `male`, `other`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="b93e4-118">The possible values are: `female`, `male`, `other`, `unknownFutureValue`.</span></span> |
| <span data-ttu-id="b93e4-119">оценка</span><span class="sxs-lookup"><span data-stu-id="b93e4-119">grade</span></span>          | <span data-ttu-id="b93e4-120">String</span><span class="sxs-lookup"><span data-stu-id="b93e4-120">String</span></span>          | <span data-ttu-id="b93e4-121">Текущий уровень оценок учащегося.</span><span class="sxs-lookup"><span data-stu-id="b93e4-121">Current grade level of the student.</span></span>                                       |
| <span data-ttu-id="b93e4-122">graduationYear</span><span class="sxs-lookup"><span data-stu-id="b93e4-122">graduationYear</span></span> | <span data-ttu-id="b93e4-123">String</span><span class="sxs-lookup"><span data-stu-id="b93e4-123">String</span></span>          | <span data-ttu-id="b93e4-124">Год выпуска учащегося из школы.</span><span class="sxs-lookup"><span data-stu-id="b93e4-124">Year the student is graduating from the school.</span></span>                           |
| <span data-ttu-id="b93e4-125">studentNumber</span><span class="sxs-lookup"><span data-stu-id="b93e4-125">studentNumber</span></span>  | <span data-ttu-id="b93e4-126">String</span><span class="sxs-lookup"><span data-stu-id="b93e4-126">String</span></span>          | <span data-ttu-id="b93e4-127">Student Number.</span><span class="sxs-lookup"><span data-stu-id="b93e4-127">Student Number.</span></span>                                                           |

## <a name="relationships"></a><span data-ttu-id="b93e4-128">Связи</span><span class="sxs-lookup"><span data-stu-id="b93e4-128">Relationships</span></span>

<span data-ttu-id="b93e4-129">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b93e4-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b93e4-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b93e4-130">JSON representation</span></span>

<span data-ttu-id="b93e4-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b93e4-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationStudent"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationStudent",
  "graduationYear": "String",
  "grade": "String",
  "birthDate": "DateTimeOffset",
  "gender": "String",
  "studentNumber": "String",
  "externalId": "String"
}
```
