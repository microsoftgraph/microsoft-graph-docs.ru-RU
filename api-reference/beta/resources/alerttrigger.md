---
title: Тип ресурса Алерттригжер
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 594061ff17f80bb1ab462647562947b16965d9dc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48067397"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="abfea-104">Тип ресурса Алерттригжер</span><span class="sxs-lookup"><span data-stu-id="abfea-104">alertTrigger resource type</span></span>

<span data-ttu-id="abfea-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abfea-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abfea-106">Содержит сведения о свойствах, которые активируют обнаружение (свойства, существующие в объекте Alert).</span><span class="sxs-lookup"><span data-stu-id="abfea-106">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="abfea-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="abfea-107">Properties</span></span>

| <span data-ttu-id="abfea-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="abfea-108">Property</span></span>   | <span data-ttu-id="abfea-109">Тип</span><span class="sxs-lookup"><span data-stu-id="abfea-109">Type</span></span>|<span data-ttu-id="abfea-110">Описание</span><span class="sxs-lookup"><span data-stu-id="abfea-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abfea-111">name</span><span class="sxs-lookup"><span data-stu-id="abfea-111">name</span></span>|<span data-ttu-id="abfea-112">String</span><span class="sxs-lookup"><span data-stu-id="abfea-112">String</span></span>|<span data-ttu-id="abfea-113">Имя свойства, служащего триггером обнаружения.</span><span class="sxs-lookup"><span data-stu-id="abfea-113">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="abfea-114">type</span><span class="sxs-lookup"><span data-stu-id="abfea-114">type</span></span>|<span data-ttu-id="abfea-115">String</span><span class="sxs-lookup"><span data-stu-id="abfea-115">String</span></span>|<span data-ttu-id="abfea-116">Тип свойства в соотношении "ключ: значение" для интерпретации.</span><span class="sxs-lookup"><span data-stu-id="abfea-116">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="abfea-117">Например, String, Boolean и т. д.</span><span class="sxs-lookup"><span data-stu-id="abfea-117">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="abfea-118">value</span><span class="sxs-lookup"><span data-stu-id="abfea-118">value</span></span>|<span data-ttu-id="abfea-119">String</span><span class="sxs-lookup"><span data-stu-id="abfea-119">String</span></span>|<span data-ttu-id="abfea-120">Значение свойства, служащего триггером обнаружения.</span><span class="sxs-lookup"><span data-stu-id="abfea-120">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="abfea-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="abfea-121">JSON representation</span></span>

<span data-ttu-id="abfea-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="abfea-122">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="abfea-123">Пример</span><span class="sxs-lookup"><span data-stu-id="abfea-123">Example</span></span>

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


