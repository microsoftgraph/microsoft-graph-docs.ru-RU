---
title: Тип ресурса autoReviewSettings
description: Указывает поведение, которое будет происходить после завершения проверки доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f46ef4b57a921cc08fbb8f3768597eef12c1ce4f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136936"
---
# <a name="autoreviewsettings-resource-type"></a><span data-ttu-id="75188-103">Тип ресурса autoReviewSettings</span><span class="sxs-lookup"><span data-stu-id="75188-103">autoReviewSettings resource type</span></span>

<span data-ttu-id="75188-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75188-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="75188-105">Тип **ресурса autoReviewSettings** используется в ресурсе [accessReviewSettings](accessreviewsettings.md) и определяет поведение после завершения проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="75188-105">The **autoReviewSettings** resource type is used in the [accessReviewSettings](accessreviewsettings.md) resource and specifies the behavior for when an access review completes.</span></span>    

## <a name="properties"></a><span data-ttu-id="75188-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="75188-106">Properties</span></span>

| <span data-ttu-id="75188-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="75188-107">Property</span></span> | <span data-ttu-id="75188-108">Тип</span><span class="sxs-lookup"><span data-stu-id="75188-108">Type</span></span> | <span data-ttu-id="75188-109">Описание</span><span class="sxs-lookup"><span data-stu-id="75188-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="75188-110">notReviewedResult</span><span class="sxs-lookup"><span data-stu-id="75188-110">notReviewedResult</span></span> | <span data-ttu-id="75188-111">Строка</span><span class="sxs-lookup"><span data-stu-id="75188-111">String</span></span> | <span data-ttu-id="75188-112">Возможные значения: `Approve` , `Deny` , или `Recommendation` .</span><span class="sxs-lookup"><span data-stu-id="75188-112">Possible values: `Approve`, `Deny`, or `Recommendation`.</span></span>  <span data-ttu-id="75188-113">Если `Recommendation` , **то accessRecommendationsEnabled** в **ресурсе accessReviewSettings** также должен быть установлен в `true` .</span><span class="sxs-lookup"><span data-stu-id="75188-113">If `Recommendation`, then **accessRecommendationsEnabled** in the **accessReviewSettings** resource should also be set to `true`.</span></span> <span data-ttu-id="75188-114">Если вы хотите, чтобы система предоставила решение, даже если проверяющий не делает выбор, установите свойство **autoReviewEnabled** в **ресурсе accessReviewSettings** и включите объект `true` **autoReviewSettings** со свойством **notReviewedResult.**</span><span class="sxs-lookup"><span data-stu-id="75188-114">If you want to have the system provide a decision even if the reviewer does not make a choice, set the **autoReviewEnabled** property in the **accessReviewSettings** resource to `true` and include an **autoReviewSettings** object with the **notReviewedResult** property.</span></span> <span data-ttu-id="75188-115">Затем, когда проверка завершается на основе свойства **notReviewedResult,** решение регистрируются как либо `Approve` либо `Deny` .</span><span class="sxs-lookup"><span data-stu-id="75188-115">Then, when a review completes, based on the **notReviewedResult** property, the decision is recorded as either `Approve` or `Deny`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75188-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="75188-116">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.autoReviewSettings"
}-->
```json
{
  "notReviewedResult": "string"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "autoReviewSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
