---
title: тип ресурса accessReviewScheduleSettings
description: В функции обзоров доступа Azure AD представлены параметры, связанные `accessReviewScheduleSettings` с серией обзоров доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 77ea7d8601df36525aad7a3448aa3b6f031d98d3
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469327"
---
# <a name="accessreviewschedulesettings-resource-type"></a><span data-ttu-id="93c29-103">тип ресурса accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="93c29-103">accessReviewScheduleSettings resource type</span></span>

<span data-ttu-id="93c29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93c29-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="93c29-105">**AccessReviewScheduleSettings** определяет параметры [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="93c29-105">The **accessReviewScheduleSettings** defines the settings of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="93c29-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="93c29-106">Properties</span></span>
| <span data-ttu-id="93c29-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="93c29-107">Property</span></span>    | <span data-ttu-id="93c29-108">Тип</span><span class="sxs-lookup"><span data-stu-id="93c29-108">Type</span></span>   | <span data-ttu-id="93c29-109">Описание</span><span class="sxs-lookup"><span data-stu-id="93c29-109">Description</span></span> |
| :---------------| :---------- | :---------- |
| <span data-ttu-id="93c29-110">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="93c29-110">mailNotificationsEnabled</span></span>|<span data-ttu-id="93c29-111">Логический</span><span class="sxs-lookup"><span data-stu-id="93c29-111">Boolean</span></span> | <span data-ttu-id="93c29-112">Флаг, чтобы указать, включены ли или отключены сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="93c29-112">Flag to indicate whether emails are enabled/disabled.</span></span>                |
| <span data-ttu-id="93c29-113">reminderNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="93c29-113">reminderNotificationsEnabled</span></span>|<span data-ttu-id="93c29-114">Логический</span><span class="sxs-lookup"><span data-stu-id="93c29-114">Boolean</span></span>  | <span data-ttu-id="93c29-115">Флаг, чтобы указать, включены ли или отключены напоминания.</span><span class="sxs-lookup"><span data-stu-id="93c29-115">Flag to indicate whether reminders are enabled/disabled.</span></span>   |
| <span data-ttu-id="93c29-116">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="93c29-116">justificationRequiredOnApproval</span></span>|<span data-ttu-id="93c29-117">Логический</span><span class="sxs-lookup"><span data-stu-id="93c29-117">Boolean</span></span> | <span data-ttu-id="93c29-118">Флаг, чтобы указать, требуются ли рецензенты для обоснования своего решения.</span><span class="sxs-lookup"><span data-stu-id="93c29-118">Flag to indicate whether reviewers are required to provide justification with their decision.</span></span> |
| <span data-ttu-id="93c29-119">defaultDecisionEnabled</span><span class="sxs-lookup"><span data-stu-id="93c29-119">defaultDecisionEnabled</span></span>|<span data-ttu-id="93c29-120">Логический</span><span class="sxs-lookup"><span data-stu-id="93c29-120">Boolean</span></span> | <span data-ttu-id="93c29-121">Флаг, чтобы указать, включено или отключено решение по умолчанию, если рецензенты не отвечают.</span><span class="sxs-lookup"><span data-stu-id="93c29-121">Flag to indicate whether default decision is enabled/disabled when reviewers do not respond.</span></span> |
| <span data-ttu-id="93c29-122">defaultDecision</span><span class="sxs-lookup"><span data-stu-id="93c29-122">defaultDecision</span></span>|<span data-ttu-id="93c29-123">String</span><span class="sxs-lookup"><span data-stu-id="93c29-123">String</span></span> | <span data-ttu-id="93c29-124">Решение, `defaultDecisionEnabled` выбранное, если включено.</span><span class="sxs-lookup"><span data-stu-id="93c29-124">Decision chosen if `defaultDecisionEnabled` is enabled.</span></span> <span data-ttu-id="93c29-125">Может быть одним из "Утверждение", "Отказ" или "Рекомендация".</span><span class="sxs-lookup"><span data-stu-id="93c29-125">Can be one of "Approve", "Deny", or "Recommendation".</span></span> |
| <span data-ttu-id="93c29-126">instanceDurationInDays</span><span class="sxs-lookup"><span data-stu-id="93c29-126">instanceDurationInDays</span></span>|<span data-ttu-id="93c29-127">Int32</span><span class="sxs-lookup"><span data-stu-id="93c29-127">Int32</span></span> | <span data-ttu-id="93c29-128">Продолжительность каждого повторения обзора `accessReviewInstance` () в количестве дней.</span><span class="sxs-lookup"><span data-stu-id="93c29-128">Duration of each recurrence of review (`accessReviewInstance`) in number of days.</span></span> |
| <span data-ttu-id="93c29-129">recurrence</span><span class="sxs-lookup"><span data-stu-id="93c29-129">recurrence</span></span>|[<span data-ttu-id="93c29-130">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="93c29-130">patternedRecurrence</span></span>](../resources/patternedrecurrence.md) | <span data-ttu-id="93c29-131">Подробные параметры для повторения.</span><span class="sxs-lookup"><span data-stu-id="93c29-131">Detailed settings for recurrence.</span></span> <span data-ttu-id="93c29-132">Использование стандартного объекта повторения Outlook.</span><span class="sxs-lookup"><span data-stu-id="93c29-132">Using standard Outlook recurrence object.</span></span> <span data-ttu-id="93c29-133">Обратите внимание, что dayOfMonth не поддерживается — используйте свойство startDate на recurrenceRange, чтобы определить день начала проверки.</span><span class="sxs-lookup"><span data-stu-id="93c29-133">Note that dayOfMonth is not supported - use property startDate on recurrenceRange to determine the day the review will start on.</span></span> |
| <span data-ttu-id="93c29-134">autoApplyDecisionsEnabled</span><span class="sxs-lookup"><span data-stu-id="93c29-134">autoApplyDecisionsEnabled</span></span>|<span data-ttu-id="93c29-135">Логический</span><span class="sxs-lookup"><span data-stu-id="93c29-135">Boolean</span></span> | <span data-ttu-id="93c29-136">Флаг, чтобы указать, включена ли функция автоматического применения.</span><span class="sxs-lookup"><span data-stu-id="93c29-136">Flag to indicate whether auto-apply feature is enabled.</span></span> |
| <span data-ttu-id="93c29-137">applyActions</span><span class="sxs-lookup"><span data-stu-id="93c29-137">applyActions</span></span>|<span data-ttu-id="93c29-138">[accessReviewApplyAction collection](../resources/accessreviewapplyaction.md)</span><span class="sxs-lookup"><span data-stu-id="93c29-138">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) collection</span></span> | <span data-ttu-id="93c29-139">Необязательное поле.</span><span class="sxs-lookup"><span data-stu-id="93c29-139">Optional field.</span></span> <span data-ttu-id="93c29-140">Описывает действия, которые необходимо выполнить после завершения проверки.</span><span class="sxs-lookup"><span data-stu-id="93c29-140">Describes the  actions to take once a review is complete.</span></span> <span data-ttu-id="93c29-141">В настоящее время поддерживается два типа: `removeAccessApplyAction` (по умолчанию) и `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="93c29-141">There are two types that are currently supported: `removeAccessApplyAction` (default) and `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="93c29-142">Поле должно быть указано только в случае `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="93c29-142">Field only needs to be specified in the case of `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="93c29-143">См. [accessReviewApplyAction](accessreviewapplyaction.md).</span><span class="sxs-lookup"><span data-stu-id="93c29-143">See [accessReviewApplyAction](accessreviewapplyaction.md).</span></span> |
| <span data-ttu-id="93c29-144">recommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="93c29-144">recommendationsEnabled</span></span>|<span data-ttu-id="93c29-145">Логический</span><span class="sxs-lookup"><span data-stu-id="93c29-145">Boolean</span></span> | <span data-ttu-id="93c29-146">Флаг, чтобы указать, включены или отключены рекомендации по принятию решений.</span><span class="sxs-lookup"><span data-stu-id="93c29-146">Flag to indicate whether decision recommendations are enabled/disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="93c29-147">Связи</span><span class="sxs-lookup"><span data-stu-id="93c29-147">Relationships</span></span>
<span data-ttu-id="93c29-148">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="93c29-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="93c29-149">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="93c29-149">JSON representation</span></span>
<span data-ttu-id="93c29-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93c29-150">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScheduleSettings",
  "mailNotificationsEnabled": "Boolean",
  "reminderNotificationsEnabled": "Boolean",
  "justificationRequiredOnApproval": "Boolean",
  "defaultDecisionEnabled": "Boolean",
  "defaultDecision": "String",
  "instanceDurationInDays": "Integer",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "autoApplyDecisionsEnabled": "Boolean",
  "applyActions": [
    {
      "@odata.type": "microsoft.graph.removeAccessApplyAction"
    }
  ],
  "recommendationsEnabled": "Boolean"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScheduleSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
