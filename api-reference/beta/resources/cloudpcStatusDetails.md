---
title: Тип ресурса Клаудпкстатусдетаилс
description: Сведения о состоянии облачного компьютера.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 61260bc7f3437fe1f10575afc616462eec2e47dc
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563863"
---
# <a name="cloudpcstatusdetails-resource-type"></a><span data-ttu-id="eb365-103">Тип ресурса Клаудпкстатусдетаилс</span><span class="sxs-lookup"><span data-stu-id="eb365-103">cloudPcStatusDetails resource type</span></span>

<span data-ttu-id="eb365-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb365-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb365-105">Сведения о состоянии облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="eb365-105">The details of the cloud PC status.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="eb365-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="eb365-106">Properties</span></span>

|<span data-ttu-id="eb365-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="eb365-107">Property</span></span>|<span data-ttu-id="eb365-108">Тип</span><span class="sxs-lookup"><span data-stu-id="eb365-108">Type</span></span>|<span data-ttu-id="eb365-109">Описание</span><span class="sxs-lookup"><span data-stu-id="eb365-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb365-110">code</span><span class="sxs-lookup"><span data-stu-id="eb365-110">code</span></span>|<span data-ttu-id="eb365-111">String</span><span class="sxs-lookup"><span data-stu-id="eb365-111">String</span></span>|<span data-ttu-id="eb365-112">Код, связанный с состоянием Cloud PC.</span><span class="sxs-lookup"><span data-stu-id="eb365-112">The code associated with the cloud PC status.</span></span>|
|<span data-ttu-id="eb365-113">message</span><span class="sxs-lookup"><span data-stu-id="eb365-113">message</span></span>|<span data-ttu-id="eb365-114">String</span><span class="sxs-lookup"><span data-stu-id="eb365-114">String</span></span>|<span data-ttu-id="eb365-115">Сообщение о состоянии.</span><span class="sxs-lookup"><span data-stu-id="eb365-115">The status message.</span></span>|
|<span data-ttu-id="eb365-116">аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="eb365-116">additionalInformation</span></span>|<span data-ttu-id="eb365-117">Коллекция [KeyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="eb365-117">[KeyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="eb365-118">Любые дополнительные сведения о состоянии Cloud PC.</span><span class="sxs-lookup"><span data-stu-id="eb365-118">Any additional information about the cloud PC status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb365-119">Связи</span><span class="sxs-lookup"><span data-stu-id="eb365-119">Relationships</span></span>

<span data-ttu-id="eb365-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="eb365-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb365-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="eb365-121">JSON representation</span></span>

<span data-ttu-id="eb365-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eb365-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcStatusDetails",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcStatusDetails",
  "code": "String",
  "message": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```
