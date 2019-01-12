---
title: Тип ресурса alertTrigger
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 56034fb566f960ec858b86cdb4bcac86e5b9b47a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946429"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="247f5-104">Тип ресурса alertTrigger</span><span class="sxs-lookup"><span data-stu-id="247f5-104">alertTrigger resource type</span></span>

 > <span data-ttu-id="247f5-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="247f5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="247f5-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="247f5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="247f5-107">Содержит сведения о свойствах, которые запускаются обнаружения (свойства существуют оповещения сущности).</span><span class="sxs-lookup"><span data-stu-id="247f5-107">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="247f5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="247f5-108">Properties</span></span>

| <span data-ttu-id="247f5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="247f5-109">Property</span></span>   | <span data-ttu-id="247f5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="247f5-110">Type</span></span>|<span data-ttu-id="247f5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="247f5-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="247f5-112">name</span><span class="sxs-lookup"><span data-stu-id="247f5-112">name</span></span>|<span data-ttu-id="247f5-113">Строка</span><span class="sxs-lookup"><span data-stu-id="247f5-113">String</span></span>|<span data-ttu-id="247f5-114">Имя свойства, используемого в качестве триггера обнаружения.</span><span class="sxs-lookup"><span data-stu-id="247f5-114">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="247f5-115">type</span><span class="sxs-lookup"><span data-stu-id="247f5-115">type</span></span>|<span data-ttu-id="247f5-116">Строка</span><span class="sxs-lookup"><span data-stu-id="247f5-116">String</span></span>|<span data-ttu-id="247f5-117">Тип свойства в пары "ключ: значение" для интерпретации.</span><span class="sxs-lookup"><span data-stu-id="247f5-117">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="247f5-118">Например String, Boolean, и т.д.</span><span class="sxs-lookup"><span data-stu-id="247f5-118">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="247f5-119">value</span><span class="sxs-lookup"><span data-stu-id="247f5-119">value</span></span>|<span data-ttu-id="247f5-120">Строка</span><span class="sxs-lookup"><span data-stu-id="247f5-120">String</span></span>|<span data-ttu-id="247f5-121">Значение свойства, используемого в качестве триггера обнаружения.</span><span class="sxs-lookup"><span data-stu-id="247f5-121">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="247f5-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="247f5-122">JSON representation</span></span>

<span data-ttu-id="247f5-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="247f5-123">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="247f5-124">Пример</span><span class="sxs-lookup"><span data-stu-id="247f5-124">Example</span></span>

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
