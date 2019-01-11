---
title: Тип ресурса alertTrigger
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
ms.openlocfilehash: e375538806f09f85539f7a03e31c8a1ae041afdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866649"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="90ed4-104">Тип ресурса alertTrigger</span><span class="sxs-lookup"><span data-stu-id="90ed4-104">alertTrigger resource type</span></span>

 > <span data-ttu-id="90ed4-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="90ed4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90ed4-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90ed4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="90ed4-107">Содержит сведения о свойствах, которые запускаются обнаружения (свойства существуют оповещения сущности).</span><span class="sxs-lookup"><span data-stu-id="90ed4-107">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="90ed4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="90ed4-108">Properties</span></span>

| <span data-ttu-id="90ed4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="90ed4-109">Property</span></span>   | <span data-ttu-id="90ed4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="90ed4-110">Type</span></span>|<span data-ttu-id="90ed4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="90ed4-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90ed4-112">name</span><span class="sxs-lookup"><span data-stu-id="90ed4-112">name</span></span>|<span data-ttu-id="90ed4-113">Строка</span><span class="sxs-lookup"><span data-stu-id="90ed4-113">String</span></span>|<span data-ttu-id="90ed4-114">Имя свойства, используемого в качестве триггера обнаружения.</span><span class="sxs-lookup"><span data-stu-id="90ed4-114">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="90ed4-115">type</span><span class="sxs-lookup"><span data-stu-id="90ed4-115">type</span></span>|<span data-ttu-id="90ed4-116">Строка</span><span class="sxs-lookup"><span data-stu-id="90ed4-116">String</span></span>|<span data-ttu-id="90ed4-117">Тип свойства в пары "ключ: значение" для интерпретации.</span><span class="sxs-lookup"><span data-stu-id="90ed4-117">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="90ed4-118">Например String, Boolean, и т.д.</span><span class="sxs-lookup"><span data-stu-id="90ed4-118">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="90ed4-119">value</span><span class="sxs-lookup"><span data-stu-id="90ed4-119">value</span></span>|<span data-ttu-id="90ed4-120">Строка</span><span class="sxs-lookup"><span data-stu-id="90ed4-120">String</span></span>|<span data-ttu-id="90ed4-121">Значение свойства, используемого в качестве триггера обнаружения.</span><span class="sxs-lookup"><span data-stu-id="90ed4-121">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="90ed4-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="90ed4-122">JSON representation</span></span>

<span data-ttu-id="90ed4-123">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90ed4-123">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="90ed4-124">Пример</span><span class="sxs-lookup"><span data-stu-id="90ed4-124">Example</span></span>

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
