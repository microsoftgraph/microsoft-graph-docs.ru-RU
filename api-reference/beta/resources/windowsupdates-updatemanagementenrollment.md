---
title: тип ресурса updateManagementEnrollment
description: Представляет регистрацию в управлении службой определенной категории обновлений.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 1d00bc152d5fc3b7b4be267cd3ea56fab52b8b38
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067492"
---
# <a name="updatemanagementenrollment-resource-type"></a><span data-ttu-id="3c464-103">тип ресурса updateManagementEnrollment</span><span class="sxs-lookup"><span data-stu-id="3c464-103">updateManagementEnrollment resource type</span></span>

<span data-ttu-id="3c464-104">Пространство имен: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="3c464-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c464-105">Представляет регистрацию в управлении службой определенной категории обновлений.</span><span class="sxs-lookup"><span data-stu-id="3c464-105">Represents enrollment into management by the service of a certain update category.</span></span>

<span data-ttu-id="3c464-106">Наследует [от updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md).</span><span class="sxs-lookup"><span data-stu-id="3c464-106">Inherits from [updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3c464-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c464-107">Properties</span></span>
|<span data-ttu-id="3c464-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c464-108">Property</span></span>|<span data-ttu-id="3c464-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3c464-109">Type</span></span>|<span data-ttu-id="3c464-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3c464-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c464-111">updateCategory</span><span class="sxs-lookup"><span data-stu-id="3c464-111">updateCategory</span></span>|<span data-ttu-id="3c464-112">microsoft.graph.windowsUpdates.updateCategory</span><span class="sxs-lookup"><span data-stu-id="3c464-112">microsoft.graph.windowsUpdates.updateCategory</span></span>|<span data-ttu-id="3c464-113">Категория обновлений, управляемых службой.</span><span class="sxs-lookup"><span data-stu-id="3c464-113">The category of updates that the service manages.</span></span> <span data-ttu-id="3c464-114">Поддерживает подмножество значений **для updateCategory.**</span><span class="sxs-lookup"><span data-stu-id="3c464-114">Supports a subset of the values for **updateCategory**.</span></span> <span data-ttu-id="3c464-115">Возможные значения: `feature` .</span><span class="sxs-lookup"><span data-stu-id="3c464-115">Possible values are: `feature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c464-116">Связи</span><span class="sxs-lookup"><span data-stu-id="3c464-116">Relationships</span></span>
<span data-ttu-id="3c464-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3c464-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c464-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3c464-118">JSON representation</span></span>
<span data-ttu-id="3c464-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c464-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updateManagementEnrollment",
  "updateCategory": "String"
}
```

