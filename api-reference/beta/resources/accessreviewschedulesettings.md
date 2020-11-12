---
title: Тип ресурса Акцессревиевсчедулесеттингс
description: В функции рецензирования Access в Azure AD `accessReviewScheduleSettings` — представляет параметры, связанные с серией проверки доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 7cca1fa7fd0da05719c22728dd472087d9737d4e
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001047"
---
# <a name="accessreviewschedulesettings-resource-type"></a><span data-ttu-id="ac297-103">Тип ресурса Акцессревиевсчедулесеттингс</span><span class="sxs-lookup"><span data-stu-id="ac297-103">accessReviewScheduleSettings resource type</span></span>

<span data-ttu-id="ac297-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac297-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac297-105">**Акцессревиевсчедулесеттингс** определяет параметры объекта [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="ac297-105">The **accessReviewScheduleSettings** defines the settings of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> 

## <a name="properties"></a><span data-ttu-id="ac297-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ac297-106">Properties</span></span>
| <span data-ttu-id="ac297-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ac297-107">Property</span></span>    | <span data-ttu-id="ac297-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ac297-108">Type</span></span>   | <span data-ttu-id="ac297-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ac297-109">Description</span></span> |
| :---------------| :---------- | :---------- |
| <span data-ttu-id="ac297-110">маилнотификатионсенаблед</span><span class="sxs-lookup"><span data-stu-id="ac297-110">mailNotificationsEnabled</span></span>|<span data-ttu-id="ac297-111">Логический</span><span class="sxs-lookup"><span data-stu-id="ac297-111">Boolean</span></span> | <span data-ttu-id="ac297-112">Флаг, указывающий, включены ли сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ac297-112">Flag to indicate whether emails are enabled/disabled.</span></span>                |
| <span data-ttu-id="ac297-113">реминдернотификатионсенаблед</span><span class="sxs-lookup"><span data-stu-id="ac297-113">reminderNotificationsEnabled</span></span>|<span data-ttu-id="ac297-114">Логический</span><span class="sxs-lookup"><span data-stu-id="ac297-114">Boolean</span></span>  | <span data-ttu-id="ac297-115">Флаг, указывающий, включены ли напоминания.</span><span class="sxs-lookup"><span data-stu-id="ac297-115">Flag to indicate whether reminders are enabled/disabled.</span></span>   |
| <span data-ttu-id="ac297-116">жустификатионрекуиредонаппровал</span><span class="sxs-lookup"><span data-stu-id="ac297-116">justificationRequiredOnApproval</span></span>|<span data-ttu-id="ac297-117">Логический</span><span class="sxs-lookup"><span data-stu-id="ac297-117">Boolean</span></span> | <span data-ttu-id="ac297-118">Флаг, указывающий, требуются ли проверяющие для предоставления обоснования для решения.</span><span class="sxs-lookup"><span data-stu-id="ac297-118">Flag to indicate whether reviewers are required to provide justification with their decision.</span></span> |
| <span data-ttu-id="ac297-119">дефаултдеЦисионенаблед</span><span class="sxs-lookup"><span data-stu-id="ac297-119">defaultDecisionEnabled</span></span>|<span data-ttu-id="ac297-120">Логический</span><span class="sxs-lookup"><span data-stu-id="ac297-120">Boolean</span></span> | <span data-ttu-id="ac297-121">Флаг, указывающий, включено ли решение по умолчанию или отключено, когда проверяющие не отвечают.</span><span class="sxs-lookup"><span data-stu-id="ac297-121">Flag to indicate whether default decision is enabled/disabled when reviewers do not respond.</span></span> |
| <span data-ttu-id="ac297-122">дефаултдеЦисион</span><span class="sxs-lookup"><span data-stu-id="ac297-122">defaultDecision</span></span>|<span data-ttu-id="ac297-123">Строка</span><span class="sxs-lookup"><span data-stu-id="ac297-123">String</span></span> | <span data-ttu-id="ac297-124">Решение выбрано, если `defaultDecisionEnabled` включено.</span><span class="sxs-lookup"><span data-stu-id="ac297-124">Decision chosen if `defaultDecisionEnabled` is enabled.</span></span> <span data-ttu-id="ac297-125">Может иметь одно из "утверждений", "deny" или "рекомендация".</span><span class="sxs-lookup"><span data-stu-id="ac297-125">Can be one of "Approve", "Deny", or "Recommendation".</span></span> |
| <span data-ttu-id="ac297-126">инстанцедуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="ac297-126">instanceDurationInDays</span></span>|<span data-ttu-id="ac297-127">Int32</span><span class="sxs-lookup"><span data-stu-id="ac297-127">Int32</span></span> | <span data-ttu-id="ac297-128">Продолжительность каждого повторения проверки ( `accessReviewInstance` ) в днях.</span><span class="sxs-lookup"><span data-stu-id="ac297-128">Duration of each recurrence of review (`accessReviewInstance`) in number of days.</span></span> |
| <span data-ttu-id="ac297-129">recurrence</span><span class="sxs-lookup"><span data-stu-id="ac297-129">recurrence</span></span>|[<span data-ttu-id="ac297-130">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="ac297-130">patternedRecurrence</span></span>](../resources/patternedrecurrence.md) | <span data-ttu-id="ac297-131">Подробные параметры для периодичности.</span><span class="sxs-lookup"><span data-stu-id="ac297-131">Detailed settings for recurrence.</span></span> <span data-ttu-id="ac297-132">Использование стандартного объекта повторения Outlook.</span><span class="sxs-lookup"><span data-stu-id="ac297-132">Using standard Outlook recurrence object.</span></span>  |
| <span data-ttu-id="ac297-133">аутоапплидеЦисионсенаблед</span><span class="sxs-lookup"><span data-stu-id="ac297-133">autoApplyDecisionsEnabled</span></span>|<span data-ttu-id="ac297-134">Логический</span><span class="sxs-lookup"><span data-stu-id="ac297-134">Boolean</span></span> | <span data-ttu-id="ac297-135">Флаг, указывающий, включена ли функция автоматического применения.</span><span class="sxs-lookup"><span data-stu-id="ac297-135">Flag to indicate whether auto-apply feature is enabled.</span></span> |
| <span data-ttu-id="ac297-136">аппляктионс</span><span class="sxs-lookup"><span data-stu-id="ac297-136">applyActions</span></span>|<span data-ttu-id="ac297-137">Коллекция [акцессревиеваппляктион](../resources/accessreviewapplyaction.md)</span><span class="sxs-lookup"><span data-stu-id="ac297-137">[accessReviewApplyAction](../resources/accessreviewapplyaction.md) collection</span></span> | <span data-ttu-id="ac297-138">Необязательное поле.</span><span class="sxs-lookup"><span data-stu-id="ac297-138">Optional field.</span></span> <span data-ttu-id="ac297-139">Описывает действия, которые необходимо выполнить после завершения проверки.</span><span class="sxs-lookup"><span data-stu-id="ac297-139">Describes the  actions to take once a review is complete.</span></span> <span data-ttu-id="ac297-140">В настоящее время поддерживаются два типа: `removeAccessApplyAction` (по умолчанию) и `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="ac297-140">There are two types that are currently supported: `removeAccessApplyAction` (default) and `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="ac297-141">Поле необходимо указать только в случае `disableAndDeleteUserApplyAction` .</span><span class="sxs-lookup"><span data-stu-id="ac297-141">Field only needs to be specified in the case of `disableAndDeleteUserApplyAction`.</span></span> <span data-ttu-id="ac297-142">Обратитесь к разделу [акцессревиеваппляктион](accessreviewapplyaction.md).</span><span class="sxs-lookup"><span data-stu-id="ac297-142">See [accessReviewApplyAction](accessreviewapplyaction.md).</span></span> |
| <span data-ttu-id="ac297-143">рекоммендатионсенаблед</span><span class="sxs-lookup"><span data-stu-id="ac297-143">recommendationsEnabled</span></span>|<span data-ttu-id="ac297-144">Логический</span><span class="sxs-lookup"><span data-stu-id="ac297-144">Boolean</span></span> | <span data-ttu-id="ac297-145">Флаг, указывающий, включены ли рекомендации по принятию или отключены.</span><span class="sxs-lookup"><span data-stu-id="ac297-145">Flag to indicate whether decision recommendations are enabled/disabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ac297-146">Связи</span><span class="sxs-lookup"><span data-stu-id="ac297-146">Relationships</span></span>
<span data-ttu-id="ac297-147">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ac297-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac297-148">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ac297-148">JSON representation</span></span>
<span data-ttu-id="ac297-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ac297-149">The following is a JSON representation of the resource.</span></span>
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
