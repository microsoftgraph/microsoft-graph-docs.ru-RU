---
title: Тип ресурса accessReviewScheduleSettings
description: В функции проверки доступа Azure AD параметры, связанные с ряду отзывов `accessReviewScheduleSettings` о доступе.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3a58ba9a682e443efbc159befaea61b15e3fdc81
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133450"
---
# <a name="accessreviewschedulesettings-resource-type"></a><span data-ttu-id="d61a3-103">Тип ресурса accessReviewScheduleSettings</span><span class="sxs-lookup"><span data-stu-id="d61a3-103">accessReviewScheduleSettings resource type</span></span>

<span data-ttu-id="d61a3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d61a3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d61a3-105">**AccessReviewScheduleSettings** определяет параметры [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="d61a3-105">The **accessReviewScheduleSettings** defines the settings of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="d61a3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d61a3-106">Properties</span></span>
| <span data-ttu-id="d61a3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d61a3-107">Property</span></span>    | <span data-ttu-id="d61a3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d61a3-108">Type</span></span>   | <span data-ttu-id="d61a3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d61a3-109">Description</span></span> |
| :---------------| :---------- | :---------- |
| <span data-ttu-id="d61a3-110">mailNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="d61a3-110">mailNotificationsEnabled</span></span>|<span data-ttu-id="d61a3-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="d61a3-111">Boolean</span></span> | <span data-ttu-id="d61a3-112">Флаг, который указывает, включены ли или отключены сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d61a3-112">Flag to indicate whether emails are enabled/disabled.</span></span>                |
| <span data-ttu-id="d61a3-113">reminderNotificationsEnabled</span><span class="sxs-lookup"><span data-stu-id="d61a3-113">reminderNotificationsEnabled</span></span>|<span data-ttu-id="d61a3-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="d61a3-114">Boolean</span></span>  | <span data-ttu-id="d61a3-115">Флаг, который указывает, включены или отключены напоминания.</span><span class="sxs-lookup"><span data-stu-id="d61a3-115">Flag to indicate whether reminders are enabled/disabled.</span></span>   |
| <span data-ttu-id="d61a3-116">justificationRequiredOnApproval</span><span class="sxs-lookup"><span data-stu-id="d61a3-116">justificationRequiredOnApproval</span></span>|<span data-ttu-id="d61a3-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="d61a3-117">Boolean</span></span> | <span data-ttu-id="d61a3-118">Флаг, который указывает, требуются ли проверяющих для обоснования своего решения.</span><span class="sxs-lookup"><span data-stu-id="d61a3-118">Flag to indicate whether reviewers are required to provide justification with their decision.</span></span> |
| <span data-ttu-id="d61a3-119">defaultDecisionEnabled</span><span class="sxs-lookup"><span data-stu-id="d61a3-119">defaultDecisionEnabled</span></span>|<span data-ttu-id="d61a3-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="d61a3-120">Boolean</span></span> | <span data-ttu-id="d61a3-121">Флаг, который указывает, включено ли решение по умолчанию, если рецензенты не отвечают.</span><span class="sxs-lookup"><span data-stu-id="d61a3-121">Flag to indicate whether default decision is enabled/disabled when reviewers do not respond.</span></span> |
| <span data-ttu-id="d61a3-122">defaultDecision</span><span class="sxs-lookup"><span data-stu-id="d61a3-122">defaultDecision</span></span>|<span data-ttu-id="d61a3-123">Строка</span><span class="sxs-lookup"><span data-stu-id="d61a3-123">String</span></span> | <span data-ttu-id="d61a3-124">Решение, выбранное, `defaultDecisionEnabled` если включено.</span><span class="sxs-lookup"><span data-stu-id="d61a3-124">Decision chosen if `defaultDecisionEnabled` is enabled.</span></span> <span data-ttu-id="d61a3-125">Может иметь одно из двух ок: "Утвердить", "Запретить" или "Рекомендация".</span><span class="sxs-lookup"><span data-stu-id="d61a3-125">Can be one of "Approve", "Deny", or "Recommendation".</span></span> |
| <span data-ttu-id="d61a3-126">instanceDurationInDays</span><span class="sxs-lookup"><span data-stu-id="d61a3-126">instanceDurationInDays</span></span>|<span data-ttu-id="d61a3-127">Int32</span><span class="sxs-lookup"><span data-stu-id="d61a3-127">Int32</span></span> | <span data-ttu-id="d61a3-128">Длительность каждого повторения проверки `accessReviewInstance` () в днях.</span><span class="sxs-lookup"><span data-stu-id="d61a3-128">Duration of each recurrence of review (`accessReviewInstance`) in number of days.</span></span> |
| <span data-ttu-id="d61a3-129">recurrence</span><span class="sxs-lookup"><span data-stu-id="d61a3-129">recurrence</span></span>|[<span data-ttu-id="d61a3-130">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="d61a3-130">patternedRecurrence</span></span>](../resources/patternedrecurrence.md) | <span data-ttu-id="d61a3-131">Подробные параметры повторения.</span><span class="sxs-lookup"><span data-stu-id="d61a3-131">Detailed settings for recurrence.</span></span> <span data-ttu-id="d61a3-132">Использование стандартного объекта повторения Outlook.</span><span class="sxs-lookup"><span data-stu-id="d61a3-132">Using standard Outlook recurrence object.</span></span>  |
| <span data-ttu-id="d61a3-133">autoApplyDecisionsEnabled</span><span class="sxs-lookup"><span data-stu-id="d61a3-133">autoApplyDecisionsEnabled</span></span>|<span data-ttu-id="d61a3-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="d61a3-134">Boolean</span></span> | <span data-ttu-id="d61a3-135">Флаг, который указывает, включена ли функция автоматического применения.</span><span class="sxs-lookup"><span data-stu-id="d61a3-135">Flag to indicate whether auto-apply feature is enabled.</span></span> |
| <span data-ttu-id="d61a3-136">applyActions</span><span class="sxs-lookup"><span data-stu-id="d61a3-136">applyActions</span></span>|<span data-ttu-id="d61a3-137">[Коллекция accessReviewApplyAction](../resources/accessreviewapplyaction.md)</span><span class="sxs-lookup"><span data-stu-id="d61a3-137">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) collection</span></span> | <span data-ttu-id="d61a3-138">Необязательное поле.</span><span class="sxs-lookup"><span data-stu-id="d61a3-138">Optional field.</span></span> <span data-ttu-id="d61a3-139">Описывает действия, которые необходимо выполнить после проверки.</span><span class="sxs-lookup"><span data-stu-id="d61a3-139">Describes the  actions to take once a review is complete.</span></span> <span data-ttu-id="d61a3-140">В настоящее время поддерживаются два типа: `removeAccessApplyAction` (по умолчанию) и `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="d61a3-140">There are two types that are currently supported: `removeAccessApplyAction` (default) and `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="d61a3-141">Поле должно быть указано только в случае с `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="d61a3-141">Field only needs to be specified in the case of `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="d61a3-142">См. [accessReviewApplyAction.](accessreviewapplyaction.md)</span><span class="sxs-lookup"><span data-stu-id="d61a3-142">See [accessReviewApplyAction](accessreviewapplyaction.md).</span></span> |
| <span data-ttu-id="d61a3-143">recommendationsEnabled</span><span class="sxs-lookup"><span data-stu-id="d61a3-143">recommendationsEnabled</span></span>|<span data-ttu-id="d61a3-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="d61a3-144">Boolean</span></span> | <span data-ttu-id="d61a3-145">Флаг, который указывает, включены ли рекомендации по принятию решений.</span><span class="sxs-lookup"><span data-stu-id="d61a3-145">Flag to indicate whether decision recommendations are enabled/disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d61a3-146">Связи</span><span class="sxs-lookup"><span data-stu-id="d61a3-146">Relationships</span></span>
<span data-ttu-id="d61a3-147">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d61a3-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d61a3-148">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d61a3-148">JSON representation</span></span>
<span data-ttu-id="d61a3-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d61a3-149">The following is a JSON representation of the resource.</span></span>
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
