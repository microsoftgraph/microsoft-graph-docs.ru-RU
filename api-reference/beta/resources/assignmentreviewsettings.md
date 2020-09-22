---
title: Тип ресурса Ассигнментревиевсеттингс
description: Тип Ассигнментревиевсеттингс, используемый для свойства Акцессревиевсеттингс политики назначения пакетов Access, предоставляет дополнительные параметры для выбора пользователей, которые должны проверить назначения пакетов доступа из этой политики и как часто они должны быть проверены.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 4a6e92f2c31a5972528fefdea68a4fa8a61677da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040184"
---
# <a name="assignmentreviewsettings-resource-type"></a><span data-ttu-id="50bf2-103">Тип ресурса Ассигнментревиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="50bf2-103">assignmentReviewSettings resource type</span></span>

<span data-ttu-id="50bf2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50bf2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50bf2-105">Используется для свойства **акцессревиевсеттингс** [политики назначения пакетов Access](accesspackageassignmentpolicy.md).</span><span class="sxs-lookup"><span data-stu-id="50bf2-105">Used for the **accessReviewSettings** property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="50bf2-106">Предоставляет дополнительные параметры для выбора пользователей, которые должны просматривать назначения пакетов доступа из этой политики и как часто они должны проверяться.</span><span class="sxs-lookup"><span data-stu-id="50bf2-106">Provides additional settings to select who must review access package assignments from this policy, and how often they must be reviewed.</span></span>  

## <a name="properties"></a><span data-ttu-id="50bf2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="50bf2-107">Properties</span></span>

<span data-ttu-id="50bf2-108">Этот тип имеет следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="50bf2-108">This type has the following properties:</span></span>

| <span data-ttu-id="50bf2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="50bf2-109">Property</span></span>                     | <span data-ttu-id="50bf2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="50bf2-110">Type</span></span>                      | <span data-ttu-id="50bf2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="50bf2-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="50bf2-112">isEnabled</span><span class="sxs-lookup"><span data-stu-id="50bf2-112">isEnabled</span></span>| <span data-ttu-id="50bf2-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="50bf2-113">Boolean</span></span> | <span data-ttu-id="50bf2-114">Если этот параметр имеет значение true, для назначений из этой политики требуются обзоры доступа.</span><span class="sxs-lookup"><span data-stu-id="50bf2-114">If true, access reviews are required for assignments from this policy.</span></span> |
| <span data-ttu-id="50bf2-115">recurrenceType</span><span class="sxs-lookup"><span data-stu-id="50bf2-115">recurrenceType</span></span> | <span data-ttu-id="50bf2-116">String</span><span class="sxs-lookup"><span data-stu-id="50bf2-116">String</span></span> | <span data-ttu-id="50bf2-117">Интервал повторения, например `monthly` или `quarterly` .</span><span class="sxs-lookup"><span data-stu-id="50bf2-117">The interval for recurrence, such as `monthly` or `quarterly`.</span></span> |
| <span data-ttu-id="50bf2-118">ревиевертипе</span><span class="sxs-lookup"><span data-stu-id="50bf2-118">reviewerType</span></span> | <span data-ttu-id="50bf2-119">String</span><span class="sxs-lookup"><span data-stu-id="50bf2-119">String</span></span> | <span data-ttu-id="50bf2-120">Кто должен иметь запрос на выполнение проверки, либо `Self` `Reviewers` .</span><span class="sxs-lookup"><span data-stu-id="50bf2-120">Who should be asked to do the review, either `Self` or `Reviewers`.</span></span> |
| <span data-ttu-id="50bf2-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="50bf2-121">startDateTime</span></span> | <span data-ttu-id="50bf2-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50bf2-122">DateTimeOffset</span></span> | <span data-ttu-id="50bf2-123">Когда должна начаться Первая проверка.</span><span class="sxs-lookup"><span data-stu-id="50bf2-123">When the first review should start.</span></span> |
| <span data-ttu-id="50bf2-124">дуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="50bf2-124">durationInDays</span></span> | <span data-ttu-id="50bf2-125">Int32</span><span class="sxs-lookup"><span data-stu-id="50bf2-125">Int32</span></span> | <span data-ttu-id="50bf2-126">Количество дней, в течение которого допускается ввод данных от рецензентов.</span><span class="sxs-lookup"><span data-stu-id="50bf2-126">The number of days to allow input from reviewers.</span></span>|
| <span data-ttu-id="50bf2-127">обсужден</span><span class="sxs-lookup"><span data-stu-id="50bf2-127">reviewers</span></span> | <span data-ttu-id="50bf2-128">Коллекция [User](userset.md) Collection</span><span class="sxs-lookup"><span data-stu-id="50bf2-128">[userSet](userset.md) collection</span></span> | <span data-ttu-id="50bf2-129">Если задано значение Ревиевертипе `Reviewers` , эта коллекция указывает пользователей, которые будут рецензентами, по идентификатору или членам группы, используя коллекцию [SingleUser.](singleuser.md) и [граупмемберс](groupmembers.md).</span><span class="sxs-lookup"><span data-stu-id="50bf2-129">If the reviewerType is `Reviewers`, this collection specifies the users who will be reviewers, either by ID or as members of a group, using a collection of [singleUser](singleuser.md) and [groupMembers](groupmembers.md).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="50bf2-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="50bf2-130">JSON representation</span></span>


<span data-ttu-id="50bf2-131">Ниже представлено описание свойства "Просмотр параметров проверки доступа" для политики в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="50bf2-131">The following is a JSON representation of the access review settings property of a policy.</span></span>

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


