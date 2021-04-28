---
title: тип ресурса windowsUpdateReference
description: Представляет конкретные Windows 10 обновления.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: a75f1afe1c2689760848283bf078b957bb8739ba
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067480"
---
# <a name="windowsupdatereference-resource-type"></a><span data-ttu-id="fc62e-103">тип ресурса windowsUpdateReference</span><span class="sxs-lookup"><span data-stu-id="fc62e-103">windowsUpdateReference resource type</span></span>

<span data-ttu-id="fc62e-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="fc62e-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc62e-105">Представляет конкретные Windows 10 обновления.</span><span class="sxs-lookup"><span data-stu-id="fc62e-105">Represents specific Windows 10 update content.</span></span>

<span data-ttu-id="fc62e-106">В развертывании одно и то же Windows обновления может привести к тому, что устройства получают различные изменения, но содержимое считается контекстуальным эквивалентом для всех устройств в развертывании.</span><span class="sxs-lookup"><span data-stu-id="fc62e-106">In a deployment, the same Windows update reference could result in devices receiving different update revisions, but the content is considered contextually equivalent for all devices in the deployment.</span></span>

<span data-ttu-id="fc62e-107">Все Windows обновления существуют как один из следующих производных типов: [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md) и [speededQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="fc62e-107">All Windows update references exist as one of the following derived types: [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md) and [expeditedQualityUpdateReference](../resources/windowsupdates-expeditedqualityupdatereference.md).</span></span>

<span data-ttu-id="fc62e-108">Наследует от [softwareUpdateReference](../resources/windowsupdates-softwareupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="fc62e-108">Inherits from [softwareUpdateReference](../resources/windowsupdates-softwareupdatereference.md).</span></span> <span data-ttu-id="fc62e-109">Базовый тип [для featureUpdateReference](../resources/windowsupdates-featureupdatereference.md) и [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="fc62e-109">Base type for [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md) and [qualityUpdateReference](../resources/windowsupdates-qualityupdatereference.md).</span></span>

<span data-ttu-id="fc62e-110">Это абстрактный тип.</span><span class="sxs-lookup"><span data-stu-id="fc62e-110">This is an abstract type.</span></span>

## <a name="properties"></a><span data-ttu-id="fc62e-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc62e-111">Properties</span></span>
<span data-ttu-id="fc62e-112">Нет</span><span class="sxs-lookup"><span data-stu-id="fc62e-112">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="fc62e-113">Связи</span><span class="sxs-lookup"><span data-stu-id="fc62e-113">Relationships</span></span>
<span data-ttu-id="fc62e-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fc62e-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc62e-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fc62e-115">JSON representation</span></span>
<span data-ttu-id="fc62e-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc62e-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.windowsUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.windowsUpdateReference"
}
```

