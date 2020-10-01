---
title: Тип ресурса Акцессревиевсеттингс
description: Предоставляет дополнительные параметры при создании проверки доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d4de925ecb2fac65e3ab339ba8d4e602fcdc2af3
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330356"
---
# <a name="accessreviewsettings-resource-type"></a><span data-ttu-id="1275a-103">Тип ресурса Акцессревиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="1275a-103">accessReviewSettings resource type</span></span>

<span data-ttu-id="1275a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1275a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1275a-105">Предоставляет дополнительные параметры при создании проверки доступа, чтобы управлять поведением компонента при запуске проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="1275a-105">Provides additional settings when creating an access review, to control the feature behavior when starting an access review.</span></span>

## <a name="properties"></a><span data-ttu-id="1275a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="1275a-106">Properties</span></span>

| <span data-ttu-id="1275a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="1275a-107">Property</span></span> | <span data-ttu-id="1275a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="1275a-108">Type</span></span> | <span data-ttu-id="1275a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="1275a-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="1275a-110">маилнотификатионсенаблед</span><span class="sxs-lookup"><span data-stu-id="1275a-110">mailNotificationsEnabled</span></span> | <span data-ttu-id="1275a-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="1275a-111">Boolean</span></span> | <span data-ttu-id="1275a-112">Указывает, включена ли отправка почты рецензентам и создателю рецензирования.</span><span class="sxs-lookup"><span data-stu-id="1275a-112">Indicates whether sending mails to reviewers and the review creator is enabled.</span></span> |
| <span data-ttu-id="1275a-113">реминдерсенаблед</span><span class="sxs-lookup"><span data-stu-id="1275a-113">remindersEnabled</span></span> | <span data-ttu-id="1275a-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="1275a-114">Boolean</span></span> | <span data-ttu-id="1275a-115">Указывает, включено ли отправку сообщений напоминания рецензентам.</span><span class="sxs-lookup"><span data-stu-id="1275a-115">Indicates whether sending reminder emails to reviewers is enabled.</span></span> |
| <span data-ttu-id="1275a-116">жустификатионрекуиредонаппровал</span><span class="sxs-lookup"><span data-stu-id="1275a-116">justificationRequiredOnApproval</span></span> | <span data-ttu-id="1275a-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="1275a-117">Boolean</span></span> | <span data-ttu-id="1275a-118">Указывает, требуются ли проверяющие для предоставления обоснования при проверке доступа.</span><span class="sxs-lookup"><span data-stu-id="1275a-118">Indicates whether reviewers are required to provide a justification when reviewing access.</span></span> |
| <span data-ttu-id="1275a-119">активитидуратиониндайс</span><span class="sxs-lookup"><span data-stu-id="1275a-119">activityDurationInDays</span></span> | <span data-ttu-id="1275a-120">Int64</span><span class="sxs-lookup"><span data-stu-id="1275a-120">Int64</span></span> | <span data-ttu-id="1275a-121">Количество дней, в течение которых действия пользователей отображаются для рецензентов.</span><span class="sxs-lookup"><span data-stu-id="1275a-121">The number of days of user activities to show to reviewers.</span></span> |
| <span data-ttu-id="1275a-122">ауторевиевенаблед</span><span class="sxs-lookup"><span data-stu-id="1275a-122">autoReviewEnabled</span></span> | <span data-ttu-id="1275a-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="1275a-123">Boolean</span></span> | <span data-ttu-id="1275a-124">Указывает, следует ли задать решение, если проверяющий не предоставил его.</span><span class="sxs-lookup"><span data-stu-id="1275a-124">Indicates whether a decision should be set if the reviewer did not supply one.</span></span> <span data-ttu-id="1275a-125">Для использования при включенном автоматическом применении.</span><span class="sxs-lookup"><span data-stu-id="1275a-125">For use when auto-apply is enabled.</span></span> <span data-ttu-id="1275a-126">Если вы не хотите, чтобы решение для проверки было записано, пока проверяющий не выйдет явный выбор, задайте для него значение `false` .</span><span class="sxs-lookup"><span data-stu-id="1275a-126">If you don't want to have a review decision recorded unless the reviewer makes an explicit choice, set it to `false`.</span></span>|
| <span data-ttu-id="1275a-127">ауторевиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="1275a-127">autoReviewSettings</span></span> | [<span data-ttu-id="1275a-128">ауторевиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="1275a-128">autoReviewSettings</span></span>](autoreviewsettings.md) | <span data-ttu-id="1275a-129">Подробные параметры, определяющие, как компонент должен устанавливать решение по проверке.</span><span class="sxs-lookup"><span data-stu-id="1275a-129">Detailed settings for how the feature should set the review decision.</span></span> <span data-ttu-id="1275a-130">Для использования при включенном автоматическом применении.</span><span class="sxs-lookup"><span data-stu-id="1275a-130">For use when auto-apply is enabled.</span></span> |
| <span data-ttu-id="1275a-131">рекурренцесеттингс</span><span class="sxs-lookup"><span data-stu-id="1275a-131">recurrenceSettings</span></span> | [<span data-ttu-id="1275a-132">акцессревиеврекурренцесеттингс</span><span class="sxs-lookup"><span data-stu-id="1275a-132">accessReviewRecurrenceSettings</span></span>](accessreviewrecurrencesettings.md) | <span data-ttu-id="1275a-133">Подробные параметры для периодичности.</span><span class="sxs-lookup"><span data-stu-id="1275a-133">Detailed settings for recurrence.</span></span> |
| <span data-ttu-id="1275a-134">аутоапплиревиевресултсенаблед</span><span class="sxs-lookup"><span data-stu-id="1275a-134">autoApplyReviewResultsEnabled</span></span> | <span data-ttu-id="1275a-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="1275a-135">Boolean</span></span> | <span data-ttu-id="1275a-136">Указывает, включена ли функция автоматического применения, чтобы автоматически изменить целевой ресурс доступа к объектам.</span><span class="sxs-lookup"><span data-stu-id="1275a-136">Indicates whether the auto-apply capability, to automatically change the target object access resource, is enabled.</span></span>  <span data-ttu-id="1275a-137">Если этот параметр не включен, пользователь должен, после завершения проверки, применить проверку доступа.</span><span class="sxs-lookup"><span data-stu-id="1275a-137">If not enabled, a user must, after the review completes, apply the access review.</span></span> |
| <span data-ttu-id="1275a-138">акцессрекоммендатионсенаблед</span><span class="sxs-lookup"><span data-stu-id="1275a-138">accessRecommendationsEnabled</span></span> | <span data-ttu-id="1275a-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="1275a-139">Boolean</span></span> | <span data-ttu-id="1275a-140">Указывает, включены ли рекомендации для рецензентов.</span><span class="sxs-lookup"><span data-stu-id="1275a-140">Indicates whether showing recommendations to reviewers is enabled.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1275a-141">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1275a-141">JSON representation</span></span>
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