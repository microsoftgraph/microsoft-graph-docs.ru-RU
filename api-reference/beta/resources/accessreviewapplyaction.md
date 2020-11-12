---
title: Тип ресурса Акцессревиеваппляктион
description: Представляет действие, которое необходимо выполнить для проверенных пользователей после завершения экземпляра проверки доступа.
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 33aa0f7a9d7fbfeab9b957f4c94b87d6f6e50d44
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/12/2020
ms.locfileid: "49001046"
---
# <a name="accessreviewapplyaction-resource-type"></a><span data-ttu-id="0111c-103">Тип ресурса Акцессревиеваппляктион</span><span class="sxs-lookup"><span data-stu-id="0111c-103">accessReviewApplyAction resource type</span></span>

<span data-ttu-id="0111c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0111c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0111c-105">Представляет базовый класс для применения действий в [акцессревиевсчедулесеттингс](accessreviewschedulesettings.md) объекта [акцессревиевсчедуледефинитион](accessreviewscheduledefinition.md).</span><span class="sxs-lookup"><span data-stu-id="0111c-105">Represents a base class for apply actions in the [accessReviewScheduleSettings](accessreviewschedulesettings.md) of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="0111c-106">Поддерживаемые производные типы:</span><span class="sxs-lookup"><span data-stu-id="0111c-106">Supported derived types:</span></span>

- <span data-ttu-id="0111c-107">**ремовеакцессаппляктион** — это производный тип акцессревиеваппляктион, указывающий на удаление доступа сущности, которая просматривается после выполнения проверки.</span><span class="sxs-lookup"><span data-stu-id="0111c-107">**removeAccessApplyAction** is a derived type of accessReviewApplyAction that indicates removing access of an entity being reviewed upon completion of the review.</span></span> <span data-ttu-id="0111c-108">Это тип по умолчанию для свойства Аппляктионс в Акцессревиевсчедулесеттингс, и его не требуется указывать.</span><span class="sxs-lookup"><span data-stu-id="0111c-108">This is the default type for the applyActions property in accessReviewScheduleSettings and does not need to be specified.</span></span>

- <span data-ttu-id="0111c-109">**дисаблеандделетеусераппляктион** — это производный тип акцессревиеваппляктион, который указывает на отключение и удаление пользователя, который просматривается после выполнения проверки.</span><span class="sxs-lookup"><span data-stu-id="0111c-109">**disableAndDeleteUserApplyAction** is a derived type of accessReviewApplyAction that indicates disabling and deleting the user being reviewed upon completion of the review.</span></span> <span data-ttu-id="0111c-110">Это не тип по умолчанию, и его необходимо указать в Акцессревиевсчедулесеттингс.</span><span class="sxs-lookup"><span data-stu-id="0111c-110">This is the non-default type and needs to specified in accessReviewScheduleSettings.</span></span>

## <a name="properties"></a><span data-ttu-id="0111c-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="0111c-111">Properties</span></span>
<span data-ttu-id="0111c-112">Нет</span><span class="sxs-lookup"><span data-stu-id="0111c-112">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="0111c-113">Связи</span><span class="sxs-lookup"><span data-stu-id="0111c-113">Relationships</span></span>
<span data-ttu-id="0111c-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0111c-114">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="0111c-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0111c-115">JSON representation</span></span>
<span data-ttu-id="0111c-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0111c-116">The following is a JSON representation of the resource.</span></span>
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
