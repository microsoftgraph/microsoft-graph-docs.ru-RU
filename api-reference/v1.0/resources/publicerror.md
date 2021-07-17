---
title: тип ресурса publicError
description: Представляет общую ошибку и ее сведения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: AkJo
ms.openlocfilehash: e9f5decf8edc2ebf3e11d00eb89e68236a6a73d4
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467531"
---
# <a name="publicerror-resource-type"></a><span data-ttu-id="bb25e-103">тип ресурса publicError</span><span class="sxs-lookup"><span data-stu-id="bb25e-103">publicError resource type</span></span>

<span data-ttu-id="bb25e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb25e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bb25e-105">Представляет общую ошибку и ее сведения.</span><span class="sxs-lookup"><span data-stu-id="bb25e-105">Represents a generic error and its details.</span></span>

## <a name="properties"></a><span data-ttu-id="bb25e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb25e-106">Properties</span></span>
|<span data-ttu-id="bb25e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb25e-107">Property</span></span>|<span data-ttu-id="bb25e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="bb25e-108">Type</span></span>|<span data-ttu-id="bb25e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bb25e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb25e-110">code</span><span class="sxs-lookup"><span data-stu-id="bb25e-110">code</span></span>|<span data-ttu-id="bb25e-111">string</span><span class="sxs-lookup"><span data-stu-id="bb25e-111">string</span></span>| <span data-ttu-id="bb25e-112">Представляет код ошибки.</span><span class="sxs-lookup"><span data-stu-id="bb25e-112">Represents the error code.</span></span>
|<span data-ttu-id="bb25e-113">подробности</span><span class="sxs-lookup"><span data-stu-id="bb25e-113">details</span></span>|<span data-ttu-id="bb25e-114">[коллекция publicErrorDetail](publicerrordetail.md)</span><span class="sxs-lookup"><span data-stu-id="bb25e-114">[publicErrorDetail](publicerrordetail.md) collection</span></span>|<span data-ttu-id="bb25e-115">Сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="bb25e-115">Details of the error.</span></span>|
|<span data-ttu-id="bb25e-116">innerError</span><span class="sxs-lookup"><span data-stu-id="bb25e-116">innerError</span></span>|[<span data-ttu-id="bb25e-117">publicInnerError</span><span class="sxs-lookup"><span data-stu-id="bb25e-117">publicInnerError</span></span>](publicinnererror.md)|<span data-ttu-id="bb25e-118">Сведения о внутренней ошибке.</span><span class="sxs-lookup"><span data-stu-id="bb25e-118">Details of the inner error.</span></span>|
|<span data-ttu-id="bb25e-119">message</span><span class="sxs-lookup"><span data-stu-id="bb25e-119">message</span></span>|<span data-ttu-id="bb25e-120">string</span><span class="sxs-lookup"><span data-stu-id="bb25e-120">string</span></span>| <span data-ttu-id="bb25e-121">Не локализованное сообщение для разработчика.</span><span class="sxs-lookup"><span data-stu-id="bb25e-121">A non-localized message for the developer.</span></span>
|<span data-ttu-id="bb25e-122">target</span><span class="sxs-lookup"><span data-stu-id="bb25e-122">target</span></span>|<span data-ttu-id="bb25e-123">String</span><span class="sxs-lookup"><span data-stu-id="bb25e-123">String</span></span>|<span data-ttu-id="bb25e-124">Целевое значение ошибки.</span><span class="sxs-lookup"><span data-stu-id="bb25e-124">The target of the error.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb25e-125">Связи</span><span class="sxs-lookup"><span data-stu-id="bb25e-125">Relationships</span></span>
<span data-ttu-id="bb25e-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bb25e-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb25e-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bb25e-127">JSON representation</span></span>
<span data-ttu-id="bb25e-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb25e-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicError",
  "code": "String",
  "message": "String",
  "target": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.publicErrorDetail"
    }
  ],
  "innerError": {
    "@odata.type": "microsoft.graph.publicInnerError"
  }
}
```
