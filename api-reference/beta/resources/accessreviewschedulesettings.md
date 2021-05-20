---
title: тип ресурса accessReviewScheduleSettings
description: В функции обзоров доступа Azure AD представлены параметры, связанные `accessReviewScheduleSettings` с серией обзоров доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b354ebfc2b5e6c8093f65c8712516421f0b1d332
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579734"
---
# <a name="accessreviewschedulesettings-resource-type"></a><span data-ttu-id="0918e-103">тип ресурса accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="0918e-103">accessReviewScheduleSettings resource type</span></span>

<span data-ttu-id="0918e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0918e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="0918e-105">**AccessReviewScheduleSettings** определяет параметры [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0918e-105">The **accessReviewScheduleSettings** defines the settings of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="0918e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0918e-106">Properties</span></span>
| <span data-ttu-id="0918e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0918e-107">Property</span></span>    | <span data-ttu-id="0918e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0918e-108">Type</span></span>   | <span data-ttu-id="0918e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0918e-109">Description</span></span> |
| :---------------| :---------- | :---------- |
| <span data-ttu-id="0918e-110">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="0918e-110">mailNotificationsEnabled</span></span>|<span data-ttu-id="0918e-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="0918e-111">Boolean</span></span> | <span data-ttu-id="0918e-112">Указывает, включена ли электронная почта или отключена.</span><span class="sxs-lookup"><span data-stu-id="0918e-112">Indicates whether emails are enabled or disabled.</span></span> <span data-ttu-id="0918e-113">Значение по умолчанию — `false`.</span><span class="sxs-lookup"><span data-stu-id="0918e-113">Default value is `false`.</span></span>               |
| <span data-ttu-id="0918e-114">reminderNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="0918e-114">reminderNotificationsEnabled</span></span>|<span data-ttu-id="0918e-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="0918e-115">Boolean</span></span>  | <span data-ttu-id="0918e-116">Указывает, включены или отключены напоминания.</span><span class="sxs-lookup"><span data-stu-id="0918e-116">Indicates whether reminders are enabled or disabled.</span></span> <span data-ttu-id="0918e-117">Значение по умолчанию — `false`.</span><span class="sxs-lookup"><span data-stu-id="0918e-117">Default value is `false`.</span></span>  |
| <span data-ttu-id="0918e-118">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="0918e-118">justificationRequiredOnApproval</span></span>|<span data-ttu-id="0918e-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="0918e-119">Boolean</span></span> | <span data-ttu-id="0918e-120">Указывает, требуются ли рецензенты для обоснования своего решения.</span><span class="sxs-lookup"><span data-stu-id="0918e-120">Indicates whether reviewers are required to provide justification with their decision.</span></span> <span data-ttu-id="0918e-121">Значение по умолчанию — `false`.</span><span class="sxs-lookup"><span data-stu-id="0918e-121">Default value is `false`.</span></span> |
| <span data-ttu-id="0918e-122">defaultDecisionEnabled</span><span class="sxs-lookup"><span data-stu-id="0918e-122">defaultDecisionEnabled</span></span>|<span data-ttu-id="0918e-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="0918e-123">Boolean</span></span> | <span data-ttu-id="0918e-124">Указывает, включено или отключено решение по умолчанию, если рецензенты не отвечают.</span><span class="sxs-lookup"><span data-stu-id="0918e-124">Indicates whether the default decision is enabled or disabled when reviewers do not respond.</span></span> <span data-ttu-id="0918e-125">Значение по умолчанию — `false`.</span><span class="sxs-lookup"><span data-stu-id="0918e-125">Default value is `false`.</span></span> |
| <span data-ttu-id="0918e-126">defaultDecision</span><span class="sxs-lookup"><span data-stu-id="0918e-126">defaultDecision</span></span>|<span data-ttu-id="0918e-127">Строка</span><span class="sxs-lookup"><span data-stu-id="0918e-127">String</span></span> | <span data-ttu-id="0918e-128">Решение, `defaultDecisionEnabled` выбранное, если включено.</span><span class="sxs-lookup"><span data-stu-id="0918e-128">Decision chosen if `defaultDecisionEnabled` is enabled.</span></span> <span data-ttu-id="0918e-129">Может быть одним из `Approve` `Deny` , или `Recommendation` .</span><span class="sxs-lookup"><span data-stu-id="0918e-129">Can be one of `Approve`, `Deny`, or `Recommendation`.</span></span> |
| <span data-ttu-id="0918e-130">instanceDurationInDays</span><span class="sxs-lookup"><span data-stu-id="0918e-130">instanceDurationInDays</span></span>|<span data-ttu-id="0918e-131">Int32</span><span class="sxs-lookup"><span data-stu-id="0918e-131">Int32</span></span> | <span data-ttu-id="0918e-132">Продолжительность каждого повторения обзора `accessReviewInstance` () в количестве дней.</span><span class="sxs-lookup"><span data-stu-id="0918e-132">Duration of each recurrence of review (`accessReviewInstance`) in number of days.</span></span> |
| <span data-ttu-id="0918e-133">recurrence</span><span class="sxs-lookup"><span data-stu-id="0918e-133">recurrence</span></span>|[<span data-ttu-id="0918e-134">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="0918e-134">patternedRecurrence</span></span>](../resources/patternedrecurrence.md) | <span data-ttu-id="0918e-135">Подробные параметры для повторения с помощью стандартного объекта Outlook повторения.</span><span class="sxs-lookup"><span data-stu-id="0918e-135">Detailed settings for recurrence using the standard Outlook recurrence object.</span></span> <span data-ttu-id="0918e-136">Поддерживаются `weekly` `absoluteMonthly` только и при **повторном повтореPattern.**</span><span class="sxs-lookup"><span data-stu-id="0918e-136">Only `weekly` and `absoluteMonthly` on **recurrencePattern** are supported.</span></span> <span data-ttu-id="0918e-137">Используйте свойство **startDate на** **recurrenceRange,** чтобы определить день начала проверки.</span><span class="sxs-lookup"><span data-stu-id="0918e-137">Use the property **startDate** on **recurrenceRange** to determine the day the review starts.</span></span> |
| <span data-ttu-id="0918e-138">autoApplyDecisionsEnabled</span><span class="sxs-lookup"><span data-stu-id="0918e-138">autoApplyDecisionsEnabled</span></span>|<span data-ttu-id="0918e-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="0918e-139">Boolean</span></span> | <span data-ttu-id="0918e-140">Указывает, применяются ли решения автоматически.</span><span class="sxs-lookup"><span data-stu-id="0918e-140">Indicates whether decisions are automatically applied.</span></span> <span data-ttu-id="0918e-141">Если установлено, пользователь должен применять решения вручную, как только рецензент завершит `false` обзор доступа.</span><span class="sxs-lookup"><span data-stu-id="0918e-141">When set to `false`, a user must apply the decisions manually once the reviewer completes the access review.</span></span> <span data-ttu-id="0918e-142">При наборе решения применяются автоматически после окончания срока действия экземпляра проверки доступа независимо от того, откликнулись ли `true` рецензенты.</span><span class="sxs-lookup"><span data-stu-id="0918e-142">When set to `true`, decisions are applied automatically after the access review instance duration ends, whether or not the reviewers have responded.</span></span> <span data-ttu-id="0918e-143">Значение по умолчанию — `false`.</span><span class="sxs-lookup"><span data-stu-id="0918e-143">Default value is `false`.</span></span> |
| <span data-ttu-id="0918e-144">applyActions</span><span class="sxs-lookup"><span data-stu-id="0918e-144">applyActions</span></span>|<span data-ttu-id="0918e-145">[accessReviewApplyAction collection](../resources/accessreviewapplyaction.md)</span><span class="sxs-lookup"><span data-stu-id="0918e-145">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) collection</span></span> | <span data-ttu-id="0918e-146">Необязательное поле.</span><span class="sxs-lookup"><span data-stu-id="0918e-146">Optional field.</span></span> <span data-ttu-id="0918e-147">Описывает действия, которые необходимо выполнить после завершения проверки.</span><span class="sxs-lookup"><span data-stu-id="0918e-147">Describes the  actions to take once a review is complete.</span></span> <span data-ttu-id="0918e-148">В настоящее время поддерживается два типа: `removeAccessApplyAction` (по умолчанию) и `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="0918e-148">There are two types that are currently supported: `removeAccessApplyAction` (default) and `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="0918e-149">Поле должно быть указано только в случае `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="0918e-149">Field only needs to be specified in the case of `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="0918e-150">См. [accessReviewApplyAction](accessreviewapplyaction.md).</span><span class="sxs-lookup"><span data-stu-id="0918e-150">See [accessReviewApplyAction](accessreviewapplyaction.md).</span></span> |
| <span data-ttu-id="0918e-151">recommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="0918e-151">recommendationsEnabled</span></span>|<span data-ttu-id="0918e-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="0918e-152">Boolean</span></span> | <span data-ttu-id="0918e-153">Указывает, включены ли рекомендации по принятию решений или отключены.</span><span class="sxs-lookup"><span data-stu-id="0918e-153">Indicates whether decision recommendations are enabled/disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="0918e-154">Отношения</span><span class="sxs-lookup"><span data-stu-id="0918e-154">Relationships</span></span>
<span data-ttu-id="0918e-155">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0918e-155">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0918e-156">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0918e-156">JSON representation</span></span>
<span data-ttu-id="0918e-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0918e-157">The following is a JSON representation of the resource.</span></span>
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
