---
title: Тип ресурса Ассигнментревиевсеттингс
description: Тип Ассигнментревиевсеттингс, используемый для свойства Акцессревиевсеттингс политики назначения пакетов Access, предоставляет дополнительные параметры для выбора пользователей, которые должны проверить назначения пакетов доступа из этой политики и как часто они должны быть проверены.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c673d96ab5bb6dbb6f217d5b36f41520b421f5bf
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331425"
---
# <a name="assignmentreviewsettings-resource-type"></a><span data-ttu-id="d55bd-103">Тип ресурса Ассигнментревиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="d55bd-103">assignmentReviewSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d55bd-104">Используется для свойства **акцессревиевсеттингс** [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="d55bd-104">Used for the **accessReviewSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="d55bd-105">Предоставляет дополнительные параметры для выбора пользователей, которые должны просматривать назначения пакетов доступа из этой политики и как часто они должны проверяться.</span><span class="sxs-lookup"><span data-stu-id="d55bd-105">Provides additional settings to select who must review access package assignments from this policy, and how often they must be reviewed.</span></span>  

## <a name="properties"></a><span data-ttu-id="d55bd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d55bd-106">Properties</span></span>

<span data-ttu-id="d55bd-107">Этот тип имеет следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="d55bd-107">This type has the following properties:</span></span>

| <span data-ttu-id="d55bd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d55bd-108">Property</span></span>                     | <span data-ttu-id="d55bd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d55bd-109">Type</span></span>                      | <span data-ttu-id="d55bd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d55bd-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="d55bd-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="d55bd-111">isEnabled</span></span>| <span data-ttu-id="d55bd-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="d55bd-112">Boolean</span></span> | <span data-ttu-id="d55bd-113">Если этот параметр имеет значение true, для назначений из этой политики требуются обзоры доступа.</span><span class="sxs-lookup"><span data-stu-id="d55bd-113">If true, access reviews are required for assignments from this policy.</span></span> |
| <span data-ttu-id="d55bd-114">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="d55bd-114">recurrenceType</span></span> | <span data-ttu-id="d55bd-115">String</span><span class="sxs-lookup"><span data-stu-id="d55bd-115">String</span></span> | <span data-ttu-id="d55bd-116">Интервал повторения, например `monthly` или. `quarterly`</span><span class="sxs-lookup"><span data-stu-id="d55bd-116">The interval for recurrence, such as `monthly` or `quarterly`.</span></span> |
| <span data-ttu-id="d55bd-117">ревиевертипе</span><span class="sxs-lookup"><span data-stu-id="d55bd-117">reviewerType</span></span> | <span data-ttu-id="d55bd-118">String</span><span class="sxs-lookup"><span data-stu-id="d55bd-118">String</span></span> | <span data-ttu-id="d55bd-119">Кто должен иметь запрос на выполнение проверки, либо `Self` `Reviewers`.</span><span class="sxs-lookup"><span data-stu-id="d55bd-119">Who should be asked to do the review, either `Self` or `Reviewers`.</span></span> |
| <span data-ttu-id="d55bd-120">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d55bd-120">startDateTime</span></span> | <span data-ttu-id="d55bd-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d55bd-121">DateTimeOffset</span></span> | <span data-ttu-id="d55bd-122">Когда должна начаться Первая проверка.</span><span class="sxs-lookup"><span data-stu-id="d55bd-122">When the first review should start.</span></span> |
| <span data-ttu-id="d55bd-123">дуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="d55bd-123">durationInDays</span></span> | <span data-ttu-id="d55bd-124">Int32</span><span class="sxs-lookup"><span data-stu-id="d55bd-124">Int32</span></span> | <span data-ttu-id="d55bd-125">Количество дней, в течение которого допускается ввод данных от рецензентов.</span><span class="sxs-lookup"><span data-stu-id="d55bd-125">The number of days to allow input from reviewers.</span></span>|
| <span data-ttu-id="d55bd-126">обсужден</span><span class="sxs-lookup"><span data-stu-id="d55bd-126">reviewers</span></span> | <span data-ttu-id="d55bd-127">Коллекция [User](userset.md) Collection</span><span class="sxs-lookup"><span data-stu-id="d55bd-127">[userSet](userset.md) collection</span></span> | <span data-ttu-id="d55bd-128">Если задано `Reviewers`значение ревиевертипе, эта коллекция указывает пользователей, которые будут рецензентами, по идентификатору или членам группы, используя коллекцию [SingleUser.](singleuser.md) и [граупмемберс](groupmembers.md).</span><span class="sxs-lookup"><span data-stu-id="d55bd-128">If the reviewerType is `Reviewers`, this collection specifies the users who will be reviewers, either by ID or as members of a group, using a collection of [singleUser](singleuser.md) and [groupMembers](groupmembers.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d55bd-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d55bd-129">JSON representation</span></span>


<span data-ttu-id="d55bd-130">Ниже представлено описание свойства "Просмотр параметров проверки доступа" для политики в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d55bd-130">The following is a JSON representation of the access review settings property of a policy.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignmentReviewSettings",
  "baseType": ""
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
