---
title: тип ресурса accessReviewApplyAction
description: Представляет действия, которые необходимо принять для рассмотренных пользователей после завершения экземпляра проверки доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 4a96ed1009a8af4404c50041258e784d8bd04030
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031229"
---
# <a name="accessreviewapplyaction-resource-type"></a><span data-ttu-id="63128-103">тип ресурса accessReviewApplyAction</span><span class="sxs-lookup"><span data-stu-id="63128-103">accessReviewApplyAction resource type</span></span>

<span data-ttu-id="63128-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63128-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="63128-105">Представляет базовый класс для применения действий в [accessReviewScheduleSettings](accessreviewschedulesettings.md) [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="63128-105">Represents a base class for apply actions in the [accessReviewScheduleSettings](accessreviewschedulesettings.md) of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="63128-106">Поддерживаемые производные типы:</span><span class="sxs-lookup"><span data-stu-id="63128-106">Supported derived types:</span></span>

- <span data-ttu-id="63128-107">[removeAccessApplyAction](removeaccessapplyaction.md) — это производный тип accessReviewApplyAction, который указывает на удаление доступа к объекту, проверяемого по завершении проверки.</span><span class="sxs-lookup"><span data-stu-id="63128-107">[removeAccessApplyAction](removeaccessapplyaction.md) is a derived type of accessReviewApplyAction that indicates removing access of an entity being reviewed upon completion of the review.</span></span> <span data-ttu-id="63128-108">Это тип по умолчанию для свойства applyActions в accessReviewScheduleSettings и не требует указаний.</span><span class="sxs-lookup"><span data-stu-id="63128-108">This is the default type for the applyActions property in accessReviewScheduleSettings and does not need to be specified.</span></span>

- <span data-ttu-id="63128-109">[disableAndDeleteUserApplyAction](disableanddeleteuserapplyaction.md) — это производный тип accessReviewApplyAction, который указывает на отключение и удаление пользователя, проверяемого по завершении проверки.</span><span class="sxs-lookup"><span data-stu-id="63128-109">[disableAndDeleteUserApplyAction](disableanddeleteuserapplyaction.md) is a derived type of accessReviewApplyAction that indicates disabling and deleting the user being reviewed upon completion of the review.</span></span> <span data-ttu-id="63128-110">Это тип по умолчанию, который должен быть указан в accessReviewScheduleSettings.</span><span class="sxs-lookup"><span data-stu-id="63128-110">This is the non-default type and needs to specified in accessReviewScheduleSettings.</span></span>

## <a name="properties"></a><span data-ttu-id="63128-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="63128-111">Properties</span></span>
<span data-ttu-id="63128-112">Нет</span><span class="sxs-lookup"><span data-stu-id="63128-112">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="63128-113">Связи</span><span class="sxs-lookup"><span data-stu-id="63128-113">Relationships</span></span>
<span data-ttu-id="63128-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="63128-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="63128-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="63128-115">JSON representation</span></span>
<span data-ttu-id="63128-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="63128-116">The following is a JSON representation of the resource.</span></span>
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

