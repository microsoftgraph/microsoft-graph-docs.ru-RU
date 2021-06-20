---
title: тип ресурса accessReviewScheduleSettings
description: Представляет параметры, связанные с серией обзоров доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8120d5b9b40f5e2ad744b65dcf927516e1d868b8
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031237"
---
# <a name="accessreviewschedulesettings-resource-type"></a><span data-ttu-id="fd1cb-103">тип ресурса accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="fd1cb-103">accessReviewScheduleSettings resource type</span></span>

<span data-ttu-id="fd1cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd1cb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fd1cb-105">**AccessReviewScheduleSettings** определяет параметры [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="fd1cb-105">The **accessReviewScheduleSettings** defines the settings of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="fd1cb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd1cb-106">Properties</span></span>
|<span data-ttu-id="fd1cb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd1cb-107">Property</span></span>|<span data-ttu-id="fd1cb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="fd1cb-108">Type</span></span>|<span data-ttu-id="fd1cb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="fd1cb-109">Description</span></span>|
|:---|:---|:---|
| <span data-ttu-id="fd1cb-110">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="fd1cb-110">mailNotificationsEnabled</span></span>|<span data-ttu-id="fd1cb-111">Логический</span><span class="sxs-lookup"><span data-stu-id="fd1cb-111">Boolean</span></span> | <span data-ttu-id="fd1cb-112">Указывает, включена ли электронная почта или отключена.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-112">Indicates whether emails are enabled or disabled.</span></span> <span data-ttu-id="fd1cb-113">Значение по умолчанию — `false`.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-113">Default value is `false`.</span></span>               |
| <span data-ttu-id="fd1cb-114">reminderNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="fd1cb-114">reminderNotificationsEnabled</span></span>|<span data-ttu-id="fd1cb-115">Логический</span><span class="sxs-lookup"><span data-stu-id="fd1cb-115">Boolean</span></span>  | <span data-ttu-id="fd1cb-116">Указывает, включены или отключены напоминания.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-116">Indicates whether reminders are enabled or disabled.</span></span> <span data-ttu-id="fd1cb-117">Значение по умолчанию — `false`.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-117">Default value is `false`.</span></span>  |
| <span data-ttu-id="fd1cb-118">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="fd1cb-118">justificationRequiredOnApproval</span></span>|<span data-ttu-id="fd1cb-119">Логический</span><span class="sxs-lookup"><span data-stu-id="fd1cb-119">Boolean</span></span> | <span data-ttu-id="fd1cb-120">Указывает, требуются ли рецензенты для обоснования своего решения.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-120">Indicates whether reviewers are required to provide justification with their decision.</span></span> <span data-ttu-id="fd1cb-121">Значение по умолчанию — `false`.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-121">Default value is `false`.</span></span> |
| <span data-ttu-id="fd1cb-122">defaultDecisionEnabled</span><span class="sxs-lookup"><span data-stu-id="fd1cb-122">defaultDecisionEnabled</span></span>|<span data-ttu-id="fd1cb-123">Логический</span><span class="sxs-lookup"><span data-stu-id="fd1cb-123">Boolean</span></span> | <span data-ttu-id="fd1cb-124">Указывает, включено или отключено решение по умолчанию, если рецензенты не отвечают.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-124">Indicates whether the default decision is enabled or disabled when reviewers do not respond.</span></span> <span data-ttu-id="fd1cb-125">Значение по умолчанию — `false`.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-125">Default value is `false`.</span></span> |
| <span data-ttu-id="fd1cb-126">defaultDecision</span><span class="sxs-lookup"><span data-stu-id="fd1cb-126">defaultDecision</span></span>|<span data-ttu-id="fd1cb-127">String</span><span class="sxs-lookup"><span data-stu-id="fd1cb-127">String</span></span> | <span data-ttu-id="fd1cb-128">Решение, **выбранное, если значение defaultDecisionEnabled** `true` является .</span><span class="sxs-lookup"><span data-stu-id="fd1cb-128">Decision chosen if **defaultDecisionEnabled** is `true`.</span></span> <span data-ttu-id="fd1cb-129">Может быть одним из `Approve` `Deny` , или `Recommendation` .</span><span class="sxs-lookup"><span data-stu-id="fd1cb-129">Can be one of `Approve`, `Deny`, or `Recommendation`.</span></span> |
| <span data-ttu-id="fd1cb-130">instanceDurationInDays</span><span class="sxs-lookup"><span data-stu-id="fd1cb-130">instanceDurationInDays</span></span>|<span data-ttu-id="fd1cb-131">Int32</span><span class="sxs-lookup"><span data-stu-id="fd1cb-131">Int32</span></span> | <span data-ttu-id="fd1cb-132">Продолжительность каждого повторения обзора **(accessReviewInstance)** в количестве дней.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-132">Duration of each recurrence of review (**accessReviewInstance**) in number of days.</span></span> |
| <span data-ttu-id="fd1cb-133">recurrence</span><span class="sxs-lookup"><span data-stu-id="fd1cb-133">recurrence</span></span>|[<span data-ttu-id="fd1cb-134">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="fd1cb-134">patternedRecurrence</span></span>](../resources/patternedrecurrence.md) | <span data-ttu-id="fd1cb-135">Подробные параметры для повторения с помощью стандартного объекта Outlook повторения.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-135">Detailed settings for recurrence using the standard Outlook recurrence object.</span></span> <span data-ttu-id="fd1cb-136">Поддерживаются `weekly` `absoluteMonthly` только и при **повторном повтореPattern.**</span><span class="sxs-lookup"><span data-stu-id="fd1cb-136">Only `weekly` and `absoluteMonthly` on **recurrencePattern** are supported.</span></span> <span data-ttu-id="fd1cb-137">Используйте свойство **startDate на** **recurrenceRange,** чтобы определить день начала проверки.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-137">Use the property **startDate** on **recurrenceRange** to determine the day the review starts.</span></span> |
| <span data-ttu-id="fd1cb-138">autoApplyDecisionsEnabled</span><span class="sxs-lookup"><span data-stu-id="fd1cb-138">autoApplyDecisionsEnabled</span></span>|<span data-ttu-id="fd1cb-139">Логический</span><span class="sxs-lookup"><span data-stu-id="fd1cb-139">Boolean</span></span> | <span data-ttu-id="fd1cb-140">Указывает, применяются ли решения автоматически.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-140">Indicates whether decisions are automatically applied.</span></span> <span data-ttu-id="fd1cb-141">Если установлено, пользователь должен применять решения вручную, как только рецензент завершит `false` обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-141">When set to `false`, a user must apply the decisions manually once the reviewer completes the access review.</span></span> <span data-ttu-id="fd1cb-142">При наборе решения применяются автоматически после окончания срока действия экземпляра проверки доступа независимо от того, откликнулись ли `true` рецензенты.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-142">When set to `true`, decisions are applied automatically after the access review instance duration ends, whether or not the reviewers have responded.</span></span> <span data-ttu-id="fd1cb-143">Значение по умолчанию — `false`.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-143">Default value is `false`.</span></span> |
| <span data-ttu-id="fd1cb-144">applyActions</span><span class="sxs-lookup"><span data-stu-id="fd1cb-144">applyActions</span></span>|<span data-ttu-id="fd1cb-145">[accessReviewApplyAction collection](../resources/accessreviewapplyaction.md)</span><span class="sxs-lookup"><span data-stu-id="fd1cb-145">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) collection</span></span> | <span data-ttu-id="fd1cb-146">Необязательное поле.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-146">Optional field.</span></span> <span data-ttu-id="fd1cb-147">Описывает действия, которые необходимо выполнить после завершения проверки.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-147">Describes the  actions to take once a review is complete.</span></span> <span data-ttu-id="fd1cb-148">В настоящее время поддерживается два типа: `removeAccessApplyAction` (по умолчанию) и `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="fd1cb-148">There are two types that are currently supported: `removeAccessApplyAction` (default) and `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="fd1cb-149">Поле должно быть указано только в случае `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="fd1cb-149">Field only needs to be specified in the case of `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="fd1cb-150">См. [accessReviewApplyAction](accessreviewapplyaction.md).</span><span class="sxs-lookup"><span data-stu-id="fd1cb-150">See [accessReviewApplyAction](accessreviewapplyaction.md).</span></span> |
| <span data-ttu-id="fd1cb-151">recommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="fd1cb-151">recommendationsEnabled</span></span>|<span data-ttu-id="fd1cb-152">Логический</span><span class="sxs-lookup"><span data-stu-id="fd1cb-152">Boolean</span></span> | <span data-ttu-id="fd1cb-153">Указывает, включены или отключены рекомендации по принятию решений.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-153">Indicates whether decision recommendations are enabled or disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fd1cb-154">Связи</span><span class="sxs-lookup"><span data-stu-id="fd1cb-154">Relationships</span></span>
<span data-ttu-id="fd1cb-155">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-155">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd1cb-156">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fd1cb-156">JSON representation</span></span>
<span data-ttu-id="fd1cb-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd1cb-157">The following is a JSON representation of the resource.</span></span>
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
