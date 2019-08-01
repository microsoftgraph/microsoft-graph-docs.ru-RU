---
title: Тип ресурса Алерттригжер
description: Содержит сведения о свойствах, которые активируют обнаружение (свойства, существующие в объекте Alert).
author: preetikr
localization_priority: Normal
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 49a262e1ab0aa046f7326b935b8437824dcf8c08
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030116"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="bae0b-103">Тип ресурса Алерттригжер</span><span class="sxs-lookup"><span data-stu-id="bae0b-103">alertTrigger resource type</span></span>

<span data-ttu-id="bae0b-104">Содержит сведения о свойствах, которые активируют обнаружение (свойства, существующие в объекте Alert).</span><span class="sxs-lookup"><span data-stu-id="bae0b-104">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="bae0b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="bae0b-105">Properties</span></span>

| <span data-ttu-id="bae0b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="bae0b-106">Property</span></span>   | <span data-ttu-id="bae0b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="bae0b-107">Type</span></span>|<span data-ttu-id="bae0b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="bae0b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bae0b-109">name</span><span class="sxs-lookup"><span data-stu-id="bae0b-109">name</span></span>|<span data-ttu-id="bae0b-110">Строка</span><span class="sxs-lookup"><span data-stu-id="bae0b-110">String</span></span>|<span data-ttu-id="bae0b-111">Имя свойства, служащего триггером обнаружения.</span><span class="sxs-lookup"><span data-stu-id="bae0b-111">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="bae0b-112">type</span><span class="sxs-lookup"><span data-stu-id="bae0b-112">type</span></span>|<span data-ttu-id="bae0b-113">String</span><span class="sxs-lookup"><span data-stu-id="bae0b-113">String</span></span>|<span data-ttu-id="bae0b-114">Тип свойства в соотношении "ключ: значение" для интерпретации.</span><span class="sxs-lookup"><span data-stu-id="bae0b-114">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="bae0b-115">Например, String, Boolean и т. д.</span><span class="sxs-lookup"><span data-stu-id="bae0b-115">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="bae0b-116">value</span><span class="sxs-lookup"><span data-stu-id="bae0b-116">value</span></span>|<span data-ttu-id="bae0b-117">String</span><span class="sxs-lookup"><span data-stu-id="bae0b-117">String</span></span>|<span data-ttu-id="bae0b-118">Значение свойства, служащего триггером обнаружения.</span><span class="sxs-lookup"><span data-stu-id="bae0b-118">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bae0b-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bae0b-119">JSON representation</span></span>

<span data-ttu-id="bae0b-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bae0b-120">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="bae0b-121">Пример</span><span class="sxs-lookup"><span data-stu-id="bae0b-121">Example</span></span>

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
