---
title: тип ресурса softwareUpdateReference
description: Представляет определенный контент обновления.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 66f7f895bd3d7556ad5e3d35066236663b474f41
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068203"
---
# <a name="softwareupdatereference-resource-type"></a><span data-ttu-id="67a3d-103">тип ресурса softwareUpdateReference</span><span class="sxs-lookup"><span data-stu-id="67a3d-103">softwareUpdateReference resource type</span></span>

<span data-ttu-id="67a3d-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="67a3d-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67a3d-105">Представляет определенный контент обновления.</span><span class="sxs-lookup"><span data-stu-id="67a3d-105">Represents specific update content.</span></span>

<span data-ttu-id="67a3d-106">В развертывании одно и то же **программное обеспечениеUpdateReference** может привести к тому, что устройства получают различные изменения обновления, но контент считается контекстуальным эквивалентом для всех устройств в развертывании.</span><span class="sxs-lookup"><span data-stu-id="67a3d-106">In a deployment, the same **softwareUpdateReference** could result in devices receiving different update revisions, but the content is considered contextually equivalent for all devices in the deployment.</span></span>

<span data-ttu-id="67a3d-107">Все ссылки на обновление программного обеспечения существуют как один из следующих производных типов: [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="67a3d-107">All software update references exist as one of the following derived types: [featureUpdateReference](../resources/windowsupdates-featureupdatereference.md).</span></span>

<span data-ttu-id="67a3d-108">Наследуется [от deployableContent](../resources/windowsupdates-deployablecontent.md).</span><span class="sxs-lookup"><span data-stu-id="67a3d-108">Inherits from [deployableContent](../resources/windowsupdates-deployablecontent.md).</span></span> <span data-ttu-id="67a3d-109">Базовый тип [для windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md).</span><span class="sxs-lookup"><span data-stu-id="67a3d-109">Base type for [windowsUpdateReference](../resources/windowsupdates-windowsupdatereference.md).</span></span>

<span data-ttu-id="67a3d-110">Это абстрактный тип.</span><span class="sxs-lookup"><span data-stu-id="67a3d-110">This is an abstract type.</span></span>

## <a name="properties"></a><span data-ttu-id="67a3d-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="67a3d-111">Properties</span></span>
<span data-ttu-id="67a3d-112">Нет</span><span class="sxs-lookup"><span data-stu-id="67a3d-112">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="67a3d-113">Связи</span><span class="sxs-lookup"><span data-stu-id="67a3d-113">Relationships</span></span>
<span data-ttu-id="67a3d-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="67a3d-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="67a3d-115">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="67a3d-115">JSON representation</span></span>
<span data-ttu-id="67a3d-116">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="67a3d-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.softwareUpdateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.softwareUpdateReference"
}
```

