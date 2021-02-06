---
title: Тип ресурса accessReviewApplyAction
description: Представляет действие, необходимое для проверяемой пользователей после завершения экземпляра проверки доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7360c2a3a058eb4f884cb786c05a83efe09a6193
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133541"
---
# <a name="accessreviewapplyaction-resource-type"></a><span data-ttu-id="7a55a-103">Тип ресурса accessReviewApplyAction</span><span class="sxs-lookup"><span data-stu-id="7a55a-103">accessReviewApplyAction resource type</span></span>

<span data-ttu-id="7a55a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a55a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a55a-105">Представляет базовый класс для применения действий [в accessReviewScheduleSettings](accessreviewschedulesettings.md) [accessReviewScheduleDefinition.](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="7a55a-105">Represents a base class for apply actions in the [accessReviewScheduleSettings](accessreviewschedulesettings.md) of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="7a55a-106">Поддерживаемые производные типы:</span><span class="sxs-lookup"><span data-stu-id="7a55a-106">Supported derived types:</span></span>

- <span data-ttu-id="7a55a-107">**removeAccessApplyAction** — это производный тип accessReviewApplyAction, который указывает на удаление доступа к объекту, проверяемого по завершении проверки.</span><span class="sxs-lookup"><span data-stu-id="7a55a-107">**removeAccessApplyAction** is a derived type of accessReviewApplyAction that indicates removing access of an entity being reviewed upon completion of the review.</span></span> <span data-ttu-id="7a55a-108">Это тип по умолчанию для свойства applyActions в accessReviewScheduleSettings, который не требуется задан.</span><span class="sxs-lookup"><span data-stu-id="7a55a-108">This is the default type for the applyActions property in accessReviewScheduleSettings and does not need to be specified.</span></span>

- <span data-ttu-id="7a55a-109">**disableAndDeleteUserApplyAction** — это производный тип accessReviewApplyAction, который указывает на отключение и удаление пользователя, проверяемого по завершении проверки.</span><span class="sxs-lookup"><span data-stu-id="7a55a-109">**disableAndDeleteUserApplyAction** is a derived type of accessReviewApplyAction that indicates disabling and deleting the user being reviewed upon completion of the review.</span></span> <span data-ttu-id="7a55a-110">Этот тип не является типом по умолчанию и должен быть указан в accessReviewScheduleSettings.</span><span class="sxs-lookup"><span data-stu-id="7a55a-110">This is the non-default type and needs to specified in accessReviewScheduleSettings.</span></span>

## <a name="properties"></a><span data-ttu-id="7a55a-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a55a-111">Properties</span></span>
<span data-ttu-id="7a55a-112">Нет</span><span class="sxs-lookup"><span data-stu-id="7a55a-112">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="7a55a-113">Связи</span><span class="sxs-lookup"><span data-stu-id="7a55a-113">Relationships</span></span>
<span data-ttu-id="7a55a-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7a55a-114">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="7a55a-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7a55a-115">JSON representation</span></span>
<span data-ttu-id="7a55a-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7a55a-116">The following is a JSON representation of the resource.</span></span>
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
