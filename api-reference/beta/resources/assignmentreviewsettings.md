---
title: Тип ресурса assignmentReviewSettings
description: Тип assignmentReviewSettings, используемый для свойства accessReviewSettings политики назначения пакета доступа, предоставляет дополнительные параметры, чтобы выбрать, кто должен просмотреть назначения пакетов доступа из этой политики и как часто их необходимо просмотреть.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: bde8c6d330eda7e100071edbf2190e170ca913ea
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131343"
---
# <a name="assignmentreviewsettings-resource-type"></a><span data-ttu-id="dbd75-103">Тип ресурса assignmentReviewSettings</span><span class="sxs-lookup"><span data-stu-id="dbd75-103">assignmentReviewSettings resource type</span></span>

<span data-ttu-id="dbd75-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbd75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbd75-105">Используется для свойства **accessReviewSettings** политики [назначения пакета доступа.](accesspackageassignmentpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="dbd75-105">Used for the **accessReviewSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="dbd75-106">Предоставляет дополнительные параметры, чтобы выбрать, кто должен просмотреть назначения пакетов доступа из этой политики и как часто их необходимо просмотреть.</span><span class="sxs-lookup"><span data-stu-id="dbd75-106">Provides additional settings to select who must review access package assignments from this policy, and how often they must be reviewed.</span></span>  

## <a name="properties"></a><span data-ttu-id="dbd75-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="dbd75-107">Properties</span></span>

<span data-ttu-id="dbd75-108">Этот тип имеет следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="dbd75-108">This type has the following properties:</span></span>

| <span data-ttu-id="dbd75-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="dbd75-109">Property</span></span>                     | <span data-ttu-id="dbd75-110">Тип</span><span class="sxs-lookup"><span data-stu-id="dbd75-110">Type</span></span>                      | <span data-ttu-id="dbd75-111">Описание</span><span class="sxs-lookup"><span data-stu-id="dbd75-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="dbd75-112">isEnabled</span><span class="sxs-lookup"><span data-stu-id="dbd75-112">isEnabled</span></span>| <span data-ttu-id="dbd75-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="dbd75-113">Boolean</span></span> | <span data-ttu-id="dbd75-114">Если имеется true, для назначений из этой политики требуются проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="dbd75-114">If true, access reviews are required for assignments from this policy.</span></span> |
| <span data-ttu-id="dbd75-115">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="dbd75-115">recurrenceType</span></span> | <span data-ttu-id="dbd75-116">Строка</span><span class="sxs-lookup"><span data-stu-id="dbd75-116">String</span></span> | <span data-ttu-id="dbd75-117">Интервал повторения, например `monthly` или `quarterly` .</span><span class="sxs-lookup"><span data-stu-id="dbd75-117">The interval for recurrence, such as `monthly` or `quarterly`.</span></span> |
| <span data-ttu-id="dbd75-118">reviewerType</span><span class="sxs-lookup"><span data-stu-id="dbd75-118">reviewerType</span></span> | <span data-ttu-id="dbd75-119">Строка</span><span class="sxs-lookup"><span data-stu-id="dbd75-119">String</span></span> | <span data-ttu-id="dbd75-120">Кто должен быть предложено сделать отзыв, либо `Self` `Reviewers` .</span><span class="sxs-lookup"><span data-stu-id="dbd75-120">Who should be asked to do the review, either `Self` or `Reviewers`.</span></span> |
| <span data-ttu-id="dbd75-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="dbd75-121">startDateTime</span></span> | <span data-ttu-id="dbd75-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbd75-122">DateTimeOffset</span></span> | <span data-ttu-id="dbd75-123">Когда должен начаться первый обзор.</span><span class="sxs-lookup"><span data-stu-id="dbd75-123">When the first review should start.</span></span> |
| <span data-ttu-id="dbd75-124">durationInDays</span><span class="sxs-lookup"><span data-stu-id="dbd75-124">durationInDays</span></span> | <span data-ttu-id="dbd75-125">Int32</span><span class="sxs-lookup"><span data-stu-id="dbd75-125">Int32</span></span> | <span data-ttu-id="dbd75-126">Количество дней, в течение которые можно разрешить ввод данных от проверяющих.</span><span class="sxs-lookup"><span data-stu-id="dbd75-126">The number of days to allow input from reviewers.</span></span>|
| <span data-ttu-id="dbd75-127">рецензенты</span><span class="sxs-lookup"><span data-stu-id="dbd75-127">reviewers</span></span> | <span data-ttu-id="dbd75-128">[Коллекция userSet](userset.md)</span><span class="sxs-lookup"><span data-stu-id="dbd75-128">[userSet](userset.md) collection</span></span> | <span data-ttu-id="dbd75-129">Если это reviewerType, эта коллекция указывает пользователей, которые будут рецензентами по ИД или в качестве членов группы, используя коллекцию `Reviewers` [singleUser](singleuser.md) и [groupMembers.](groupmembers.md)</span><span class="sxs-lookup"><span data-stu-id="dbd75-129">If the reviewerType is `Reviewers`, this collection specifies the users who will be reviewers, either by ID or as members of a group, using a collection of [singleUser](singleuser.md) and [groupMembers](groupmembers.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dbd75-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="dbd75-130">JSON representation</span></span>


<span data-ttu-id="dbd75-131">Ниже приводится представление свойства параметров проверки доступа политики в JSON.</span><span class="sxs-lookup"><span data-stu-id="dbd75-131">The following is a JSON representation of the access review settings property of a policy.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignmentReviewSettings"
}-->

```json
{
  "isEnabled": true,
  "recurrenceType": "quarterly",
  "reviewerType": "Self",
  "startDateTime": "2020-01-23T07:59:59.998Z",
  "durationInDays": 25,
  "reviewers": []
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "assignmentReviewSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


