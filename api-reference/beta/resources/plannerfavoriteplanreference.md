---
title: Тип ресурса Планнерфаворитепланреференце
description: 'Тип ресурса **планнерфаворитепланреференце** репесентс ссылку на plannerPlan, помеченную пользователем в качестве избранного. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 77a931a882cc4b01725bd8ceb0ae6bcc721a9013
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457104"
---
# <a name="plannerfavoriteplanreference-resource-type"></a><span data-ttu-id="277f0-103">Тип ресурса Планнерфаворитепланреференце</span><span class="sxs-lookup"><span data-stu-id="277f0-103">plannerFavoritePlanReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="277f0-104">Тип ресурса **планнерфаворитепланреференце** репесентс ссылку на [plannerPlan](plannerplan.md) , помеченную пользователем в качестве избранного.</span><span class="sxs-lookup"><span data-stu-id="277f0-104">The **plannerFavoritePlanReference** resource type repesents a reference to a [plannerPlan](plannerplan.md) that has been marked as a favorite by the user.</span></span> <span data-ttu-id="277f0-105">Клиенты должны отметить, что записи **планнерфаворитепланреференце** могут ссылаться на **планов** , которые были удалены, что пользователь больше не может получить доступ, или он был обновлен с другим названием.</span><span class="sxs-lookup"><span data-stu-id="277f0-105">Clients should note that **plannerFavoritePlanReference** entries can reference **plannerPlans** that are deleted, that the user can no longer access, or that have been updated with a different title.</span></span>

<span data-ttu-id="277f0-106">Мы рекомендуем клиентам уведомлять пользователей о наличии расхождений и постоянном обновлении записей.</span><span class="sxs-lookup"><span data-stu-id="277f0-106">We recommend that clients notify users when there are discrepancies and keep the entries up to date.</span></span>


## <a name="properties"></a><span data-ttu-id="277f0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="277f0-107">Properties</span></span>
| <span data-ttu-id="277f0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="277f0-108">Property</span></span>     | <span data-ttu-id="277f0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="277f0-109">Type</span></span>   |<span data-ttu-id="277f0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="277f0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="277f0-111">orderHint</span><span class="sxs-lookup"><span data-stu-id="277f0-111">orderHint</span></span>|<span data-ttu-id="277f0-112">String</span><span class="sxs-lookup"><span data-stu-id="277f0-112">String</span></span>|<span data-ttu-id="277f0-p102">Указание, используемое для упорядочивания элементов этого типа в списке. Формат определен в статье [Использование указаний order в Планировщике](planner-order-hint-format.md).</span><span class="sxs-lookup"><span data-stu-id="277f0-p102">Hint used to order items of this type in a list view. The format is defined in [Using order hints in Planner](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="277f0-115">Плантитле</span><span class="sxs-lookup"><span data-stu-id="277f0-115">planTitle</span></span>|<span data-ttu-id="277f0-116">Строка</span><span class="sxs-lookup"><span data-stu-id="277f0-116">String</span></span>|<span data-ttu-id="277f0-117">Название плана на тот момент, когда пользователь пометил его в качестве избранного.</span><span class="sxs-lookup"><span data-stu-id="277f0-117">Title of the plan at the time the user marked it as a favorite.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="277f0-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="277f0-118">JSON representation</span></span>

<span data-ttu-id="277f0-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="277f0-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerFavoritePlanReference"
}-->

```json
{
  "orderHint": "String",
  "planTitle": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerfavoriteplanreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
