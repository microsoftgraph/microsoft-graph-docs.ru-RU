---
title: Тип ресурса publicInnerError
description: Представляет внутренние сведения об ошибке.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e8380e8836076687a2d6ab3e8a0a4a53b8bd6964
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658352"
---
# <a name="publicinnererror-resource-type"></a><span data-ttu-id="31661-103">Тип ресурса publicInnerError</span><span class="sxs-lookup"><span data-stu-id="31661-103">publicInnerError resource type</span></span>

<span data-ttu-id="31661-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31661-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="31661-105">Представляет внутренние сведения [publicError.](../resources/publicerrordetail.md)</span><span class="sxs-lookup"><span data-stu-id="31661-105">Represents the inner details of a [publicError](../resources/publicerrordetail.md).</span></span> 
## <a name="properties"></a><span data-ttu-id="31661-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="31661-106">Properties</span></span>
|<span data-ttu-id="31661-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="31661-107">Property</span></span>|<span data-ttu-id="31661-108">Тип</span><span class="sxs-lookup"><span data-stu-id="31661-108">Type</span></span>|<span data-ttu-id="31661-109">Описание</span><span class="sxs-lookup"><span data-stu-id="31661-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31661-110">code</span><span class="sxs-lookup"><span data-stu-id="31661-110">code</span></span>|<span data-ttu-id="31661-111">String</span><span class="sxs-lookup"><span data-stu-id="31661-111">String</span></span>|<span data-ttu-id="31661-112">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="31661-112">The error code.</span></span>|
|<span data-ttu-id="31661-113">details</span><span class="sxs-lookup"><span data-stu-id="31661-113">details</span></span>|<span data-ttu-id="31661-114">[Коллекция publicErrorDetail](../resources/publicerrordetail.md)</span><span class="sxs-lookup"><span data-stu-id="31661-114">[publicErrorDetail](../resources/publicerrordetail.md) collection</span></span>|<span data-ttu-id="31661-115">Коллекция сведений об ошибках.</span><span class="sxs-lookup"><span data-stu-id="31661-115">A collection of error details.</span></span>|
|<span data-ttu-id="31661-116">message</span><span class="sxs-lookup"><span data-stu-id="31661-116">message</span></span>|<span data-ttu-id="31661-117">String</span><span class="sxs-lookup"><span data-stu-id="31661-117">String</span></span>|<span data-ttu-id="31661-118">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="31661-118">The error message.</span></span>|
|<span data-ttu-id="31661-119">target</span><span class="sxs-lookup"><span data-stu-id="31661-119">target</span></span>|<span data-ttu-id="31661-120">String</span><span class="sxs-lookup"><span data-stu-id="31661-120">String</span></span>|<span data-ttu-id="31661-121">Целевое значение ошибки.</span><span class="sxs-lookup"><span data-stu-id="31661-121">The target of the error.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31661-122">Связи</span><span class="sxs-lookup"><span data-stu-id="31661-122">Relationships</span></span>
<span data-ttu-id="31661-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="31661-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="31661-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="31661-124">JSON representation</span></span>
<span data-ttu-id="31661-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31661-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicInnerError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicInnerError",
  "code": "String",
  "message": "String",
  "target": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.publicErrorDetail"
    }
  ]
}
```

