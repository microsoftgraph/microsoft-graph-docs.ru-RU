---
title: Тип ресурса Ауторевиевсеттингс
description: Указывает поведение при завершении проверки доступа.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2b9d0a621c4229476e0b3bcdadb869e44422e931
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330333"
---
# <a name="autoreviewsettings-resource-type"></a><span data-ttu-id="4512a-103">Тип ресурса Ауторевиевсеттингс</span><span class="sxs-lookup"><span data-stu-id="4512a-103">autoReviewSettings resource type</span></span>

<span data-ttu-id="4512a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4512a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4512a-105">Тип ресурса **ауторевиевсеттингс** используется в ресурсе [акцессревиевсеттингс](accessreviewsettings.md) и определяет поведение при завершении проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="4512a-105">The **autoReviewSettings** resource type is used in the [accessReviewSettings](accessreviewsettings.md) resource and specifies the behavior for when an access review completes.</span></span>    

## <a name="properties"></a><span data-ttu-id="4512a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4512a-106">Properties</span></span>

| <span data-ttu-id="4512a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4512a-107">Property</span></span> | <span data-ttu-id="4512a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4512a-108">Type</span></span> | <span data-ttu-id="4512a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4512a-109">Description</span></span> |
| :------- | :--- | :---------- |
| <span data-ttu-id="4512a-110">нотревиеведресулт</span><span class="sxs-lookup"><span data-stu-id="4512a-110">notReviewedResult</span></span> | <span data-ttu-id="4512a-111">Строка</span><span class="sxs-lookup"><span data-stu-id="4512a-111">String</span></span> | <span data-ttu-id="4512a-112">Возможные значения: `Approve` , `Deny` , или `Recommendation` .</span><span class="sxs-lookup"><span data-stu-id="4512a-112">Possible values: `Approve`, `Deny`, or `Recommendation`.</span></span>  <span data-ttu-id="4512a-113">В `Recommendation` этом случае для **акцессрекоммендатионсенаблед** в ресурсе **акцессревиевсеттингс** также должно быть задано значение `true` .</span><span class="sxs-lookup"><span data-stu-id="4512a-113">If `Recommendation`, then **accessRecommendationsEnabled** in the **accessReviewSettings** resource should also be set to `true`.</span></span> <span data-ttu-id="4512a-114">Если вы хотите, чтобы система предоставляла решение, даже если проверяющий не сделает выбор, установите свойство **ауторевиевенаблед** в ресурсе **акцессревиевсеттингс** в `true` и включите объект **ауторевиевсеттингс** со свойством **нотревиеведресулт** .</span><span class="sxs-lookup"><span data-stu-id="4512a-114">If you want to have the system provide a decision even if the reviewer does not make a choice, set the **autoReviewEnabled** property in the **accessReviewSettings** resource to `true` and include an **autoReviewSettings** object with the **notReviewedResult** property.</span></span> <span data-ttu-id="4512a-115">После завершения анализа на основе свойства **нотревиеведресулт** решение записывается как `Approve` или `Deny` .</span><span class="sxs-lookup"><span data-stu-id="4512a-115">Then, when a review completes, based on the **notReviewedResult** property, the decision is recorded as either `Approve` or `Deny`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4512a-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4512a-116">JSON representation</span></span>

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