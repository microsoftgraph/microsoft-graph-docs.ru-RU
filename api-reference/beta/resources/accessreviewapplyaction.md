---
title: тип ресурса accessReviewApplyAction
description: Представляет действия, которые необходимо принять для рассмотренных пользователей после завершения экземпляра проверки доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c7f1425bb7155762f973f65fd766db8da55b8d77
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579643"
---
# <a name="accessreviewapplyaction-resource-type"></a><span data-ttu-id="e2882-103">тип ресурса accessReviewApplyAction</span><span class="sxs-lookup"><span data-stu-id="e2882-103">accessReviewApplyAction resource type</span></span>

<span data-ttu-id="e2882-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2882-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="e2882-105">Представляет базовый класс для применения действий в [accessReviewScheduleSettings](accessreviewschedulesettings.md) [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e2882-105">Represents a base class for apply actions in the [accessReviewScheduleSettings](accessreviewschedulesettings.md) of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="e2882-106">Поддерживаемые производные типы:</span><span class="sxs-lookup"><span data-stu-id="e2882-106">Supported derived types:</span></span>

- <span data-ttu-id="e2882-107">[removeAccessApplyAction](removeaccessapplyaction.md) — это производный тип accessReviewApplyAction, который указывает на удаление доступа к объекту, проверяемого по завершении проверки.</span><span class="sxs-lookup"><span data-stu-id="e2882-107">[removeAccessApplyAction](removeaccessapplyaction.md) is a derived type of accessReviewApplyAction that indicates removing access of an entity being reviewed upon completion of the review.</span></span> <span data-ttu-id="e2882-108">Это тип по умолчанию для свойства applyActions в accessReviewScheduleSettings и не требует указаний.</span><span class="sxs-lookup"><span data-stu-id="e2882-108">This is the default type for the applyActions property in accessReviewScheduleSettings and does not need to be specified.</span></span>

- <span data-ttu-id="e2882-109">[disableAndDeleteUserApplyAction](disableanddeleteuserapplyaction.md) — это производный тип accessReviewApplyAction, который указывает на отключение и удаление пользователя, проверяемого по завершении проверки.</span><span class="sxs-lookup"><span data-stu-id="e2882-109">[disableAndDeleteUserApplyAction](disableanddeleteuserapplyaction.md) is a derived type of accessReviewApplyAction that indicates disabling and deleting the user being reviewed upon completion of the review.</span></span> <span data-ttu-id="e2882-110">Это тип по умолчанию, который должен быть указан в accessReviewScheduleSettings.</span><span class="sxs-lookup"><span data-stu-id="e2882-110">This is the non-default type and needs to specified in accessReviewScheduleSettings.</span></span>

## <a name="properties"></a><span data-ttu-id="e2882-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2882-111">Properties</span></span>
<span data-ttu-id="e2882-112">Нет</span><span class="sxs-lookup"><span data-stu-id="e2882-112">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="e2882-113">Связи</span><span class="sxs-lookup"><span data-stu-id="e2882-113">Relationships</span></span>
<span data-ttu-id="e2882-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e2882-114">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e2882-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e2882-115">JSON representation</span></span>
<span data-ttu-id="e2882-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e2882-116">The following is a JSON representation of the resource.</span></span>
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
