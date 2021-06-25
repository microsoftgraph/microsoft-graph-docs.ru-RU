---
title: тип ресурса alertTrigger
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 1cda08c26b5d28de4c2b57c2bb5b34f79a84bcd8
ms.sourcegitcommit: 8a9be6f65f62f29973508d82e0348d4142c18f23
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2021
ms.locfileid: "53129472"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="6e445-104">тип ресурса alertTrigger</span><span class="sxs-lookup"><span data-stu-id="6e445-104">alertTrigger resource type</span></span>

<span data-ttu-id="6e445-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e445-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e445-106">Содержит сведения о свойствах, которые вызвали обнаружение (свойства существуют в объекте оповещений).</span><span class="sxs-lookup"><span data-stu-id="6e445-106">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="6e445-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e445-107">Properties</span></span>

| <span data-ttu-id="6e445-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e445-108">Property</span></span>   | <span data-ttu-id="6e445-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6e445-109">Type</span></span>|<span data-ttu-id="6e445-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6e445-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e445-111">name</span><span class="sxs-lookup"><span data-stu-id="6e445-111">name</span></span>|<span data-ttu-id="6e445-112">String</span><span class="sxs-lookup"><span data-stu-id="6e445-112">String</span></span>|<span data-ttu-id="6e445-113">Имя свойства, которое служит спусковым крючком обнаружения.</span><span class="sxs-lookup"><span data-stu-id="6e445-113">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="6e445-114">type</span><span class="sxs-lookup"><span data-stu-id="6e445-114">type</span></span>|<span data-ttu-id="6e445-115">String</span><span class="sxs-lookup"><span data-stu-id="6e445-115">String</span></span>|<span data-ttu-id="6e445-116">Тип свойства в паре key:value для интерпретации.</span><span class="sxs-lookup"><span data-stu-id="6e445-116">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="6e445-117">Например, String, Boolean и т.д.</span><span class="sxs-lookup"><span data-stu-id="6e445-117">For example, String, Boolean etc.</span></span>|
|<span data-ttu-id="6e445-118">value</span><span class="sxs-lookup"><span data-stu-id="6e445-118">value</span></span>|<span data-ttu-id="6e445-119">String</span><span class="sxs-lookup"><span data-stu-id="6e445-119">String</span></span>|<span data-ttu-id="6e445-120">Значение свойства, служащая в качестве триггера обнаружения.</span><span class="sxs-lookup"><span data-stu-id="6e445-120">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6e445-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e445-121">JSON representation</span></span>

<span data-ttu-id="6e445-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e445-122">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="6e445-123">Пример</span><span class="sxs-lookup"><span data-stu-id="6e445-123">Example</span></span>

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


