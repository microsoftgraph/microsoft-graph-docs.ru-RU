---
title: Тип ресурса accessReviewSettings
description: Предоставляет дополнительные параметры при создании проверки доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 18af2ef86c33650129934f43d2212222e98448fd
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133429"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="955dd-103">Тип ресурса accessReviewSettings</span><span class="sxs-lookup"><span data-stu-id="955dd-103">accessReviewSettings resource type</span></span>

<span data-ttu-id="955dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="955dd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="955dd-105">Предоставляет дополнительные параметры при создании проверки доступа для управления поведением функций при запуске проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="955dd-105">Provides additional settings when creating an access review, to control the feature behavior when starting an access review.</span></span>

## <a name="properties"></a><span data-ttu-id="955dd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="955dd-106">Properties</span></span>

| <span data-ttu-id="955dd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="955dd-107">Property</span></span> | <span data-ttu-id="955dd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="955dd-108">Type</span></span> | <span data-ttu-id="955dd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="955dd-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="955dd-110">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="955dd-110">mailNotificationsEnabled</span></span> | <span data-ttu-id="955dd-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="955dd-111">Boolean</span></span> | <span data-ttu-id="955dd-112">Указывает, включена ли отправка сообщений рецензентам и создателю отзывов.</span><span class="sxs-lookup"><span data-stu-id="955dd-112">Indicates whether sending mails to reviewers and the review creator is enabled.</span></span> |
| <span data-ttu-id="955dd-113">remindersEnabled</span><span class="sxs-lookup"><span data-stu-id="955dd-113">remindersEnabled</span></span> | <span data-ttu-id="955dd-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="955dd-114">Boolean</span></span> | <span data-ttu-id="955dd-115">Указывает, включена ли отправка напоминаний рецензентам.</span><span class="sxs-lookup"><span data-stu-id="955dd-115">Indicates whether sending reminder emails to reviewers is enabled.</span></span> |
| <span data-ttu-id="955dd-116">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="955dd-116">justificationRequiredOnApproval</span></span> | <span data-ttu-id="955dd-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="955dd-117">Boolean</span></span> | <span data-ttu-id="955dd-118">Указывает, должны ли проверяющие предоставлять обоснование при проверке доступа.</span><span class="sxs-lookup"><span data-stu-id="955dd-118">Indicates whether reviewers are required to provide a justification when reviewing access.</span></span> |
| <span data-ttu-id="955dd-119">activityDurationInDays</span><span class="sxs-lookup"><span data-stu-id="955dd-119">activityDurationInDays</span></span> | <span data-ttu-id="955dd-120">Int64</span><span class="sxs-lookup"><span data-stu-id="955dd-120">Int64</span></span> | <span data-ttu-id="955dd-121">Количество дней действий пользователей, которые будут показываться рецензентам.</span><span class="sxs-lookup"><span data-stu-id="955dd-121">The number of days of user activities to show to reviewers.</span></span> |
| <span data-ttu-id="955dd-122">autoReviewEnabled</span><span class="sxs-lookup"><span data-stu-id="955dd-122">autoReviewEnabled</span></span> | <span data-ttu-id="955dd-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="955dd-123">Boolean</span></span> | <span data-ttu-id="955dd-124">Указывает, следует ли принимать решение, если рецензент не указал его.</span><span class="sxs-lookup"><span data-stu-id="955dd-124">Indicates whether a decision should be set if the reviewer did not supply one.</span></span> <span data-ttu-id="955dd-125">Используется, если включено автоматическое применение.</span><span class="sxs-lookup"><span data-stu-id="955dd-125">For use when auto-apply is enabled.</span></span> <span data-ttu-id="955dd-126">Если вы не хотите, чтобы решение о проверке было записано, если рецензент не сделал явного выбора, установите для него такое же. `false`</span><span class="sxs-lookup"><span data-stu-id="955dd-126">If you don't want to have a review decision recorded unless the reviewer makes an explicit choice, set it to `false`.</span></span>|
| <span data-ttu-id="955dd-127">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="955dd-127">autoReviewSettings</span></span> | [<span data-ttu-id="955dd-128">autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="955dd-128">autoReviewSettings</span></span>](autoreviewsettings.md) | <span data-ttu-id="955dd-129">Подробные параметры настройки функции для принятия решения об отзыве.</span><span class="sxs-lookup"><span data-stu-id="955dd-129">Detailed settings for how the feature should set the review decision.</span></span> <span data-ttu-id="955dd-130">Используется, если включено автоматическое применение.</span><span class="sxs-lookup"><span data-stu-id="955dd-130">For use when auto-apply is enabled.</span></span> |
| <span data-ttu-id="955dd-131">recurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="955dd-131">recurrenceSettings</span></span> | [<span data-ttu-id="955dd-132">accessReviewRecurrenceSettings</span><span class="sxs-lookup"><span data-stu-id="955dd-132">accessReviewRecurrenceSettings</span></span>](accessreviewrecurrencesettings.md) | <span data-ttu-id="955dd-133">Подробные параметры повторения.</span><span class="sxs-lookup"><span data-stu-id="955dd-133">Detailed settings for recurrence.</span></span> |
| <span data-ttu-id="955dd-134">autoApplyReviewResultsEnabled</span><span class="sxs-lookup"><span data-stu-id="955dd-134">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="955dd-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="955dd-135">Boolean</span></span> | <span data-ttu-id="955dd-136">Указывает, включена ли возможность автоматического применения для автоматического изменения ресурса доступа к целевому объекту.</span><span class="sxs-lookup"><span data-stu-id="955dd-136">Indicates whether the auto-apply capability, to automatically change the target object access resource, is enabled.</span></span>  <span data-ttu-id="955dd-137">Если этот запрет не включен, пользователь должен после завершения проверки доступа применить проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="955dd-137">If not enabled, a user must, after the review completes, apply the access review.</span></span> |
| <span data-ttu-id="955dd-138">accessRecommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="955dd-138">accessRecommendationsEnabled</span></span> | <span data-ttu-id="955dd-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="955dd-139">Boolean</span></span> | <span data-ttu-id="955dd-140">Указывает, включены ли рекомендации для проверяющих.</span><span class="sxs-lookup"><span data-stu-id="955dd-140">Indicates whether showing recommendations to reviewers is enabled.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="955dd-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="955dd-141">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewSettings"
}-->
```json
{
  "mailNotificationsEnabled": true,
  "remindersEnabled": true,  
  "justificationRequiredOnApproval": true,
  "activityDurationInDays": 1024,
  "autoReviewEnabled": false,
  "autoReviewSettings": {"@odata.type": "microsoft.graph.autoReviewSettings"},
  "recurrenceSettings": {"@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"},
  "autoApplyReviewResultsEnabled": false,
  "accessRecommendationsEnabled": false
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "accessReviewSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
