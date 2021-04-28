---
title: тип ресурса qualityUpdateReference
description: Представляет Windows 10 обновления качества.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: ca416ba5031e4642a073f4796ee27996d22f0f5a
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068079"
---
# <a name="qualityupdatereference-resource-type"></a><span data-ttu-id="8d8a1-103">тип ресурса qualityUpdateReference</span><span class="sxs-lookup"><span data-stu-id="8d8a1-103">qualityUpdateReference resource type</span></span>

<span data-ttu-id="8d8a1-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="8d8a1-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8d8a1-105">Представляет Windows 10 обновления качества.</span><span class="sxs-lookup"><span data-stu-id="8d8a1-105">Represents Windows 10 quality update content.</span></span>

<span data-ttu-id="8d8a1-106">В развертывании такая же ссылка на обновление качества может привести к тому, что устройства получают различные изменения обновления, но контент считается контекстуальным эквивалентом для всех устройств в развертывании.</span><span class="sxs-lookup"><span data-stu-id="8d8a1-106">In a deployment, the same quality update reference could result in devices receiving different update revisions, but the content is considered contextually equivalent for all devices in the deployment.</span></span>

<span data-ttu-id="8d8a1-107">Наследует [от windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="8d8a1-107">Inherits from [windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md).</span></span> <span data-ttu-id="8d8a1-108">Базовый [тип ускоренногоQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="8d8a1-108">Base type of [expeditedQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md).</span></span>

## <a name="properties"></a><span data-ttu-id="8d8a1-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d8a1-109">Properties</span></span>
|<span data-ttu-id="8d8a1-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d8a1-110">Property</span></span>|<span data-ttu-id="8d8a1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8d8a1-111">Type</span></span>|<span data-ttu-id="8d8a1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8d8a1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d8a1-113">classification</span><span class="sxs-lookup"><span data-stu-id="8d8a1-113">classification</span></span>|<span data-ttu-id="8d8a1-114">microsoft.graph.windowsUpdates.qualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="8d8a1-114">microsoft.graph.windowsUpdates.qualityUpdateClassification</span></span>|<span data-ttu-id="8d8a1-115">Указывает классификацию указанного контента.</span><span class="sxs-lookup"><span data-stu-id="8d8a1-115">Specifies the classification of the referenced content.</span></span> <span data-ttu-id="8d8a1-116">Поддерживает подмножество значений **для qualityUpdateClassification.**</span><span class="sxs-lookup"><span data-stu-id="8d8a1-116">Supports a subset of the values for **qualityUpdateClassification**.</span></span> <span data-ttu-id="8d8a1-117">Возможные значения: `security` .</span><span class="sxs-lookup"><span data-stu-id="8d8a1-117">Possible values are: `security`.</span></span>|
|<span data-ttu-id="8d8a1-118">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="8d8a1-118">releaseDateTime</span></span>|<span data-ttu-id="8d8a1-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d8a1-119">DateTimeOffset</span></span>|<span data-ttu-id="8d8a1-120">Указывает обновление качества в указанной службеChannel с указанной классификацией по дате (например, последнее обновление, опубликованное в указанную дату).</span><span class="sxs-lookup"><span data-stu-id="8d8a1-120">Specifies a quality update in the given servicingChannel with the given classification by date (i.e. the last update published on the specified date).</span></span> <span data-ttu-id="8d8a1-121">Значение по умолчанию — безопасность.</span><span class="sxs-lookup"><span data-stu-id="8d8a1-121">Default value is security.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d8a1-122">Связи</span><span class="sxs-lookup"><span data-stu-id="8d8a1-122">Relationships</span></span>
<span data-ttu-id="8d8a1-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8d8a1-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d8a1-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="8d8a1-124">JSON representation</span></span>
<span data-ttu-id="8d8a1-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d8a1-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.qualityUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.qualityUpdateReference",
  "classification": "String",
  "releaseDateTime": "String (timestamp)"
}
```

