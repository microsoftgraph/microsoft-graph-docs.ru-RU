---
title: тип ресурса publicInnerError
description: Представляет внутренние сведения об ошибке.
author: AkJo
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f089c120ac4ba1307f0b0ffa2f08f8578613eaa1
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467522"
---
# <a name="publicinnererror-resource-type"></a><span data-ttu-id="7278a-103">тип ресурса publicInnerError</span><span class="sxs-lookup"><span data-stu-id="7278a-103">publicInnerError resource type</span></span>

<span data-ttu-id="7278a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7278a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7278a-105">Представляет внутренние сведения [publicError](../resources/publicerrordetail.md).</span><span class="sxs-lookup"><span data-stu-id="7278a-105">Represents the inner details of a [publicError](../resources/publicerrordetail.md).</span></span> 
## <a name="properties"></a><span data-ttu-id="7278a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="7278a-106">Properties</span></span>
|<span data-ttu-id="7278a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="7278a-107">Property</span></span>|<span data-ttu-id="7278a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="7278a-108">Type</span></span>|<span data-ttu-id="7278a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7278a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7278a-110">code</span><span class="sxs-lookup"><span data-stu-id="7278a-110">code</span></span>|<span data-ttu-id="7278a-111">String</span><span class="sxs-lookup"><span data-stu-id="7278a-111">String</span></span>|<span data-ttu-id="7278a-112">Код ошибки.</span><span class="sxs-lookup"><span data-stu-id="7278a-112">The error code.</span></span>|
|<span data-ttu-id="7278a-113">подробности</span><span class="sxs-lookup"><span data-stu-id="7278a-113">details</span></span>|<span data-ttu-id="7278a-114">[коллекция publicErrorDetail](../resources/publicerrordetail.md)</span><span class="sxs-lookup"><span data-stu-id="7278a-114">[publicErrorDetail](../resources/publicerrordetail.md) collection</span></span>|<span data-ttu-id="7278a-115">Коллекция сведений об ошибках.</span><span class="sxs-lookup"><span data-stu-id="7278a-115">A collection of error details.</span></span>|
|<span data-ttu-id="7278a-116">message</span><span class="sxs-lookup"><span data-stu-id="7278a-116">message</span></span>|<span data-ttu-id="7278a-117">String</span><span class="sxs-lookup"><span data-stu-id="7278a-117">String</span></span>|<span data-ttu-id="7278a-118">Сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="7278a-118">The error message.</span></span>|
|<span data-ttu-id="7278a-119">target</span><span class="sxs-lookup"><span data-stu-id="7278a-119">target</span></span>|<span data-ttu-id="7278a-120">String</span><span class="sxs-lookup"><span data-stu-id="7278a-120">String</span></span>|<span data-ttu-id="7278a-121">Целевое значение ошибки.</span><span class="sxs-lookup"><span data-stu-id="7278a-121">The target of the error.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7278a-122">Связи</span><span class="sxs-lookup"><span data-stu-id="7278a-122">Relationships</span></span>
<span data-ttu-id="7278a-123">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7278a-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7278a-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7278a-124">JSON representation</span></span>
<span data-ttu-id="7278a-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7278a-125">The following is a JSON representation of the resource.</span></span>
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
