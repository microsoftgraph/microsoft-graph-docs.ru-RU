---
title: Тип ресурса alertTrigger
description: Содержит сведения о свойствах, которые запускаются обнаружения (свойства существуют оповещения сущности).
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 3a2f6818bad0c5600e4b2a2a2682707643d1900c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991260"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="5b517-103">Тип ресурса alertTrigger</span><span class="sxs-lookup"><span data-stu-id="5b517-103">alertTrigger resource type</span></span>

<span data-ttu-id="5b517-104">Содержит сведения о свойствах, которые запускаются обнаружения (свойства существуют оповещения сущности).</span><span class="sxs-lookup"><span data-stu-id="5b517-104">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="5b517-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b517-105">Properties</span></span>

| <span data-ttu-id="5b517-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b517-106">Property</span></span>   | <span data-ttu-id="5b517-107">Тип</span><span class="sxs-lookup"><span data-stu-id="5b517-107">Type</span></span>|<span data-ttu-id="5b517-108">Описание</span><span class="sxs-lookup"><span data-stu-id="5b517-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b517-109">name</span><span class="sxs-lookup"><span data-stu-id="5b517-109">name</span></span>|<span data-ttu-id="5b517-110">String</span><span class="sxs-lookup"><span data-stu-id="5b517-110">String</span></span>|<span data-ttu-id="5b517-111">Имя свойства, используемого в качестве триггера обнаружения.</span><span class="sxs-lookup"><span data-stu-id="5b517-111">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="5b517-112">type</span><span class="sxs-lookup"><span data-stu-id="5b517-112">type</span></span>|<span data-ttu-id="5b517-113">String</span><span class="sxs-lookup"><span data-stu-id="5b517-113">String</span></span>|<span data-ttu-id="5b517-114">Тип свойства в пары "ключ: значение" для интерпретации.</span><span class="sxs-lookup"><span data-stu-id="5b517-114">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="5b517-115">Например String, Boolean, и т.д.</span><span class="sxs-lookup"><span data-stu-id="5b517-115">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="5b517-116">value</span><span class="sxs-lookup"><span data-stu-id="5b517-116">value</span></span>|<span data-ttu-id="5b517-117">String</span><span class="sxs-lookup"><span data-stu-id="5b517-117">String</span></span>|<span data-ttu-id="5b517-118">Значение свойства, используемого в качестве триггера обнаружения.</span><span class="sxs-lookup"><span data-stu-id="5b517-118">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b517-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b517-119">JSON representation</span></span>

<span data-ttu-id="5b517-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b517-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a><span data-ttu-id="5b517-121">Пример</span><span class="sxs-lookup"><span data-stu-id="5b517-121">Example</span></span>

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
