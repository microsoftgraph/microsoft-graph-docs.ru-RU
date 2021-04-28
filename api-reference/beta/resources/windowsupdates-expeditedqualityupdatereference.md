---
title: ускоренный тип ресурсаQualityUpdateReference
description: Представляет Windows 10 обновления качества для ускорения.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 685f65d8c5661cd4c8308ed712ab3fddedbae51d
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068176"
---
# <a name="expeditedqualityupdatereference-resource-type"></a><span data-ttu-id="e044c-103">ускоренный тип ресурсаQualityUpdateReference</span><span class="sxs-lookup"><span data-stu-id="e044c-103">expeditedQualityUpdateReference resource type</span></span>

<span data-ttu-id="e044c-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="e044c-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e044c-105">Представляет Windows 10 обновления качества для ускорения.</span><span class="sxs-lookup"><span data-stu-id="e044c-105">Represents Windows 10 quality update content to expedite.</span></span>

<span data-ttu-id="e044c-106">В развертывании такая же ссылка на ускоренное обновление качества может привести к тому, что устройства получают различные изменения, но контент считается контекстуальным эквивалентом для всех устройств в развертывании.</span><span class="sxs-lookup"><span data-stu-id="e044c-106">In a deployment, the same expedited quality update reference could result in devices receiving different update revisions, but the content is considered contextually equivalent for all devices in the deployment.</span></span>

<span data-ttu-id="e044c-107">Наследует [от qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="e044c-107">Inherits from [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e044c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e044c-108">Properties</span></span>
|<span data-ttu-id="e044c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e044c-109">Property</span></span>|<span data-ttu-id="e044c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e044c-110">Type</span></span>|<span data-ttu-id="e044c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e044c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e044c-112">classification</span><span class="sxs-lookup"><span data-stu-id="e044c-112">classification</span></span>|<span data-ttu-id="e044c-113">microsoft.graph.windowsUpdates.qualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="e044c-113">microsoft.graph.windowsUpdates.qualityUpdateClassification</span></span>|<span data-ttu-id="e044c-114">Указывает классификацию указанного контента.</span><span class="sxs-lookup"><span data-stu-id="e044c-114">Specifies the classification of the referenced content.</span></span> <span data-ttu-id="e044c-115">Поддерживает подмножество значений **для qualityUpdateClassification.**</span><span class="sxs-lookup"><span data-stu-id="e044c-115">Supports a subset of the values for **qualityUpdateClassification**.</span></span> <span data-ttu-id="e044c-116">Значение по умолчанию — `security`.</span><span class="sxs-lookup"><span data-stu-id="e044c-116">Default value is `security`.</span></span> <span data-ttu-id="e044c-117">Возможные значения: `security` .</span><span class="sxs-lookup"><span data-stu-id="e044c-117">Possible values are: `security`.</span></span> <span data-ttu-id="e044c-118">Наследуется [от qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="e044c-118">Inherited from [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span></span>|
|<span data-ttu-id="e044c-119">equivalentContent</span><span class="sxs-lookup"><span data-stu-id="e044c-119">equivalentContent</span></span>|<span data-ttu-id="e044c-120">microsoft.graph.windowsUpdates.equivalentContentOption</span><span class="sxs-lookup"><span data-stu-id="e044c-120">microsoft.graph.windowsUpdates.equivalentContentOption</span></span>|<span data-ttu-id="e044c-121">Указывает другое содержимое, которое следует считать эквивалентным.</span><span class="sxs-lookup"><span data-stu-id="e044c-121">Specifies other content to consider as equivalent.</span></span> <span data-ttu-id="e044c-122">Поддерживает подмножество значений **для equivalentContentOption**.</span><span class="sxs-lookup"><span data-stu-id="e044c-122">Supports a subset of the values for **equivalentContentOption**.</span></span> <span data-ttu-id="e044c-123">Значение по умолчанию — `latestSecurity`.</span><span class="sxs-lookup"><span data-stu-id="e044c-123">Default value is `latestSecurity`.</span></span> <span data-ttu-id="e044c-124">Возможные значения: `latestSecurity` .</span><span class="sxs-lookup"><span data-stu-id="e044c-124">Possible values are: `latestSecurity`.</span></span>|
|<span data-ttu-id="e044c-125">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="e044c-125">releaseDateTime</span></span>|<span data-ttu-id="e044c-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e044c-126">DateTimeOffset</span></span>|<span data-ttu-id="e044c-127">Указывает обновление качества с указанной классификацией **на** дату публикации (то есть последнее обновление, опубликованное в указанную дату).</span><span class="sxs-lookup"><span data-stu-id="e044c-127">Specifies a quality update with the given **classification** by its publish date (i.e. the last update published on the specified date).</span></span> <span data-ttu-id="e044c-128">Все устройства с обновлением, которое было опубликовано до **выпускаDateTime,** получат ускоренное обновление качества.</span><span class="sxs-lookup"><span data-stu-id="e044c-128">Any devices with an update that was published prior to the **releaseDateTime** will receive an expedited quality update.</span></span> <span data-ttu-id="e044c-129">Наследуется [от qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="e044c-129">Inherited from [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="e044c-130">Связи</span><span class="sxs-lookup"><span data-stu-id="e044c-130">Relationships</span></span>
<span data-ttu-id="e044c-131">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e044c-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e044c-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e044c-132">JSON representation</span></span>
<span data-ttu-id="e044c-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e044c-133">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.expeditedQualityUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.expeditedQualityUpdateReference",
  "classification": "String",
  "releaseDateTime": "String (timestamp)",
  "equivalentContent": "String"
}
```

