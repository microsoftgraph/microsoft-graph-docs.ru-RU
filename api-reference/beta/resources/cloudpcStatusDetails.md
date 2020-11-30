---
title: Тип ресурса Клаудпкстатусдетаилс
description: Сведения о состоянии облачного компьютера.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 647c13878e054fbac6c1f43f565bd2788d19a9de
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378642"
---
# <a name="cloudpcstatusdetails-resource-type"></a><span data-ttu-id="a4e1b-103">Тип ресурса Клаудпкстатусдетаилс</span><span class="sxs-lookup"><span data-stu-id="a4e1b-103">cloudPcStatusDetails resource type</span></span>

<span data-ttu-id="a4e1b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4e1b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a4e1b-105">Сведения о состоянии облачного компьютера.</span><span class="sxs-lookup"><span data-stu-id="a4e1b-105">The details of the cloud PC status.</span></span>

## <a name="properties"></a><span data-ttu-id="a4e1b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a4e1b-106">Properties</span></span>

|<span data-ttu-id="a4e1b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a4e1b-107">Property</span></span>|<span data-ttu-id="a4e1b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a4e1b-108">Type</span></span>|<span data-ttu-id="a4e1b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a4e1b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a4e1b-110">code</span><span class="sxs-lookup"><span data-stu-id="a4e1b-110">code</span></span>|<span data-ttu-id="a4e1b-111">Строка</span><span class="sxs-lookup"><span data-stu-id="a4e1b-111">String</span></span>|<span data-ttu-id="a4e1b-112">Код, связанный с состоянием Cloud PC.</span><span class="sxs-lookup"><span data-stu-id="a4e1b-112">The code associated with the cloud PC status.</span></span>|
|<span data-ttu-id="a4e1b-113">message</span><span class="sxs-lookup"><span data-stu-id="a4e1b-113">message</span></span>|<span data-ttu-id="a4e1b-114">String</span><span class="sxs-lookup"><span data-stu-id="a4e1b-114">String</span></span>|<span data-ttu-id="a4e1b-115">Сообщение о состоянии.</span><span class="sxs-lookup"><span data-stu-id="a4e1b-115">The status message.</span></span>|
|<span data-ttu-id="a4e1b-116">аддитионалинформатион</span><span class="sxs-lookup"><span data-stu-id="a4e1b-116">additionalInformation</span></span>|<span data-ttu-id="a4e1b-117">Коллекция [KeyValuePair](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="a4e1b-117">[KeyValuePair](../resources/keyvaluepair.md) collection</span></span>|<span data-ttu-id="a4e1b-118">Любые дополнительные сведения о состоянии Cloud PC.</span><span class="sxs-lookup"><span data-stu-id="a4e1b-118">Any additional information about the cloud PC status.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4e1b-119">Связи</span><span class="sxs-lookup"><span data-stu-id="a4e1b-119">Relationships</span></span>

<span data-ttu-id="a4e1b-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a4e1b-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a4e1b-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="a4e1b-121">JSON representation</span></span>

<span data-ttu-id="a4e1b-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a4e1b-122">The following is a JSON representation of the resource.</span></span>
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
