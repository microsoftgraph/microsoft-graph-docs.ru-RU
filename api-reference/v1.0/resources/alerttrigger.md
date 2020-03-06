---
title: Тип ресурса Алерттригжер
description: Содержит сведения о свойствах, которые активируют обнаружение (свойства, существующие в объекте Alert).
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 75663b351004d31884f58c53a1ce91e035b0414c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532149"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="9e5aa-103">Тип ресурса Алерттригжер</span><span class="sxs-lookup"><span data-stu-id="9e5aa-103">alertTrigger resource type</span></span>

<span data-ttu-id="9e5aa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e5aa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9e5aa-105">Содержит сведения о свойствах, которые активируют обнаружение (свойства, существующие в объекте Alert).</span><span class="sxs-lookup"><span data-stu-id="9e5aa-105">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="9e5aa-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e5aa-106">Properties</span></span>

| <span data-ttu-id="9e5aa-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e5aa-107">Property</span></span>   | <span data-ttu-id="9e5aa-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9e5aa-108">Type</span></span>|<span data-ttu-id="9e5aa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9e5aa-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e5aa-110">name</span><span class="sxs-lookup"><span data-stu-id="9e5aa-110">name</span></span>|<span data-ttu-id="9e5aa-111">Строка</span><span class="sxs-lookup"><span data-stu-id="9e5aa-111">String</span></span>|<span data-ttu-id="9e5aa-112">Имя свойства, служащего триггером обнаружения.</span><span class="sxs-lookup"><span data-stu-id="9e5aa-112">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="9e5aa-113">type</span><span class="sxs-lookup"><span data-stu-id="9e5aa-113">type</span></span>|<span data-ttu-id="9e5aa-114">String</span><span class="sxs-lookup"><span data-stu-id="9e5aa-114">String</span></span>|<span data-ttu-id="9e5aa-115">Тип свойства в соотношении "ключ: значение" для интерпретации.</span><span class="sxs-lookup"><span data-stu-id="9e5aa-115">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="9e5aa-116">Например, String, Boolean и т. д.</span><span class="sxs-lookup"><span data-stu-id="9e5aa-116">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="9e5aa-117">value</span><span class="sxs-lookup"><span data-stu-id="9e5aa-117">value</span></span>|<span data-ttu-id="9e5aa-118">String</span><span class="sxs-lookup"><span data-stu-id="9e5aa-118">String</span></span>|<span data-ttu-id="9e5aa-119">Значение свойства, служащего триггером обнаружения.</span><span class="sxs-lookup"><span data-stu-id="9e5aa-119">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e5aa-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9e5aa-120">JSON representation</span></span>

<span data-ttu-id="9e5aa-121">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e5aa-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="9e5aa-122">Пример</span><span class="sxs-lookup"><span data-stu-id="9e5aa-122">Example</span></span>

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
