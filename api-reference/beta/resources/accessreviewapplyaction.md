---
title: тип ресурса accessReviewApplyAction
description: Представляет действия, которые необходимо принять для рассмотренных пользователей после завершения экземпляра проверки доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 09e23095f62c2e09b623e1e0634987f712e56730
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/18/2021
ms.locfileid: "51469404"
---
# <a name="accessreviewapplyaction-resource-type"></a><span data-ttu-id="0b012-103">тип ресурса accessReviewApplyAction</span><span class="sxs-lookup"><span data-stu-id="0b012-103">accessReviewApplyAction resource type</span></span>

<span data-ttu-id="0b012-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b012-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="0b012-105">Представляет базовый класс для применения действий в [accessReviewScheduleSettings](accessreviewschedulesettings.md) [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0b012-105">Represents a base class for apply actions in the [accessReviewScheduleSettings](accessreviewschedulesettings.md) of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="0b012-106">Поддерживаемые производные типы:</span><span class="sxs-lookup"><span data-stu-id="0b012-106">Supported derived types:</span></span>

- <span data-ttu-id="0b012-107">**removeAccessApplyAction** — это производный тип accessReviewApplyAction, который указывает на удаление доступа к объекту, проверяемого по завершении проверки.</span><span class="sxs-lookup"><span data-stu-id="0b012-107">**removeAccessApplyAction** is a derived type of accessReviewApplyAction that indicates removing access of an entity being reviewed upon completion of the review.</span></span> <span data-ttu-id="0b012-108">Это тип по умолчанию для свойства applyActions в accessReviewScheduleSettings и не требует указаний.</span><span class="sxs-lookup"><span data-stu-id="0b012-108">This is the default type for the applyActions property in accessReviewScheduleSettings and does not need to be specified.</span></span>

- <span data-ttu-id="0b012-109">**disableAndDeleteUserApplyAction** — это производный тип accessReviewApplyAction, который указывает на отключение и удаление пользователя, проверяемого по завершении проверки.</span><span class="sxs-lookup"><span data-stu-id="0b012-109">**disableAndDeleteUserApplyAction** is a derived type of accessReviewApplyAction that indicates disabling and deleting the user being reviewed upon completion of the review.</span></span> <span data-ttu-id="0b012-110">Это тип по умолчанию, который должен быть указан в accessReviewScheduleSettings.</span><span class="sxs-lookup"><span data-stu-id="0b012-110">This is the non-default type and needs to specified in accessReviewScheduleSettings.</span></span>

## <a name="properties"></a><span data-ttu-id="0b012-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="0b012-111">Properties</span></span>
<span data-ttu-id="0b012-112">Нет</span><span class="sxs-lookup"><span data-stu-id="0b012-112">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="0b012-113">Связи</span><span class="sxs-lookup"><span data-stu-id="0b012-113">Relationships</span></span>
<span data-ttu-id="0b012-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0b012-114">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0b012-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0b012-115">JSON representation</span></span>
<span data-ttu-id="0b012-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0b012-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewApplyAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewApplyAction"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewApplyAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
