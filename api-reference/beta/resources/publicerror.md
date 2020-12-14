---
title: Тип ресурса publicError
description: Представляет общую ошибку и ее сведения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: AkJo
ms.openlocfilehash: 65a75b6eb2756b92f9da6386390fae3b254f818b
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49660088"
---
# <a name="publicerror-resource-type"></a><span data-ttu-id="b6db7-103">Тип ресурса publicError</span><span class="sxs-lookup"><span data-stu-id="b6db7-103">publicError resource type</span></span>

<span data-ttu-id="b6db7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6db7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b6db7-105">Представляет общую ошибку и ее сведения.</span><span class="sxs-lookup"><span data-stu-id="b6db7-105">Represents a generic error and its details.</span></span>

## <a name="properties"></a><span data-ttu-id="b6db7-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b6db7-106">Properties</span></span>
|<span data-ttu-id="b6db7-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b6db7-107">Property</span></span>|<span data-ttu-id="b6db7-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b6db7-108">Type</span></span>|<span data-ttu-id="b6db7-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b6db7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6db7-110">code</span><span class="sxs-lookup"><span data-stu-id="b6db7-110">code</span></span>|<span data-ttu-id="b6db7-111">string</span><span class="sxs-lookup"><span data-stu-id="b6db7-111">string</span></span>| <span data-ttu-id="b6db7-112">Представляет код ошибки.</span><span class="sxs-lookup"><span data-stu-id="b6db7-112">Represents the error code.</span></span>
|<span data-ttu-id="b6db7-113">details</span><span class="sxs-lookup"><span data-stu-id="b6db7-113">details</span></span>|<span data-ttu-id="b6db7-114">[Коллекция publicErrorDetail](publicerrordetail.md)</span><span class="sxs-lookup"><span data-stu-id="b6db7-114">[publicErrorDetail](publicerrordetail.md) collection</span></span>|<span data-ttu-id="b6db7-115">Сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="b6db7-115">Details of the error.</span></span>|
|<span data-ttu-id="b6db7-116">innerError</span><span class="sxs-lookup"><span data-stu-id="b6db7-116">innerError</span></span>|[<span data-ttu-id="b6db7-117">publicInnerError</span><span class="sxs-lookup"><span data-stu-id="b6db7-117">publicInnerError</span></span>](publicinnererror.md)|<span data-ttu-id="b6db7-118">Сведения о внутренней ошибке.</span><span class="sxs-lookup"><span data-stu-id="b6db7-118">Details of the inner error.</span></span>|
|<span data-ttu-id="b6db7-119">message</span><span class="sxs-lookup"><span data-stu-id="b6db7-119">message</span></span>|<span data-ttu-id="b6db7-120">string</span><span class="sxs-lookup"><span data-stu-id="b6db7-120">string</span></span>| <span data-ttu-id="b6db7-121">Не локализованное сообщение для разработчика.</span><span class="sxs-lookup"><span data-stu-id="b6db7-121">A non-localized message for the developer.</span></span>
|<span data-ttu-id="b6db7-122">target</span><span class="sxs-lookup"><span data-stu-id="b6db7-122">target</span></span>|<span data-ttu-id="b6db7-123">String</span><span class="sxs-lookup"><span data-stu-id="b6db7-123">String</span></span>|<span data-ttu-id="b6db7-124">Целевое значение ошибки.</span><span class="sxs-lookup"><span data-stu-id="b6db7-124">The target of the error.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6db7-125">Связи</span><span class="sxs-lookup"><span data-stu-id="b6db7-125">Relationships</span></span>
<span data-ttu-id="b6db7-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b6db7-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6db7-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="b6db7-127">JSON representation</span></span>
<span data-ttu-id="b6db7-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b6db7-128">The following is a JSON representation of the resource.</span></span>
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

