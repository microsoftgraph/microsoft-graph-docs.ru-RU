---
title: Тип ресурса attributeMapping
description: Определяет поток значений для заданного целевого атрибута во время синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: b5f120075b082e50a0f94f05907b413a4c4c4ec6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128752"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="9a2bc-103">Тип ресурса attributeMapping</span><span class="sxs-lookup"><span data-stu-id="9a2bc-103">attributeMapping resource type</span></span>

<span data-ttu-id="9a2bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a2bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a2bc-105">Определяет поток значений для заданного целевого атрибута во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="9a2bc-105">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="9a2bc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9a2bc-106">Properties</span></span>

| <span data-ttu-id="9a2bc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9a2bc-107">Property</span></span>                  | <span data-ttu-id="9a2bc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9a2bc-108">Type</span></span>                      | <span data-ttu-id="9a2bc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9a2bc-109">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="9a2bc-110">defaultValue</span><span class="sxs-lookup"><span data-stu-id="9a2bc-110">defaultValue</span></span>               | <span data-ttu-id="9a2bc-111">Строка</span><span class="sxs-lookup"><span data-stu-id="9a2bc-111">String</span></span>                    |<span data-ttu-id="9a2bc-112">Значение по умолчанию, используемее в случае, если свойство источника было оценено как  `null` .</span><span class="sxs-lookup"><span data-stu-id="9a2bc-112">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="9a2bc-113">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9a2bc-113">Optional.</span></span>|
|<span data-ttu-id="9a2bc-114">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="9a2bc-114">exportMissingReferences</span></span>    |<span data-ttu-id="9a2bc-115">String</span><span class="sxs-lookup"><span data-stu-id="9a2bc-115">String</span></span>                     |<span data-ttu-id="9a2bc-116">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="9a2bc-116">For internal use only.</span></span>|
|<span data-ttu-id="9a2bc-117">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="9a2bc-117">flowBehavior</span></span>               |<span data-ttu-id="9a2bc-118">attributeFlowBehavior</span><span class="sxs-lookup"><span data-stu-id="9a2bc-118">attributeFlowBehavior</span></span>      |<span data-ttu-id="9a2bc-119">Определяет, когда этот атрибут должен экспортироваться в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="9a2bc-119">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="9a2bc-120">Возможные значения: `FlowWhenChanged` и `FlowAlways` .</span><span class="sxs-lookup"><span data-stu-id="9a2bc-120">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="9a2bc-121">Значение по умолчанию: `FlowWhenChanged`.</span><span class="sxs-lookup"><span data-stu-id="9a2bc-121">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="9a2bc-122">flowType</span><span class="sxs-lookup"><span data-stu-id="9a2bc-122">flowType</span></span>                   |<span data-ttu-id="9a2bc-123">attributeFlowType</span><span class="sxs-lookup"><span data-stu-id="9a2bc-123">attributeFlowType</span></span>          |<span data-ttu-id="9a2bc-124">Определяет время обновления этого атрибута в целевом каталоге.</span><span class="sxs-lookup"><span data-stu-id="9a2bc-124">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="9a2bc-125">Возможные значения: (по умолчанию) (только при добавлении нового объекта) (только при добавлении новых значений в атрибут с несколькими `Always` `ObjectAddOnly` `MultiValueAddOnly` значениями).</span><span class="sxs-lookup"><span data-stu-id="9a2bc-125">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="9a2bc-126">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="9a2bc-126">matchingPriority</span></span>           |<span data-ttu-id="9a2bc-127">Int32</span><span class="sxs-lookup"><span data-stu-id="9a2bc-127">Int32</span></span>                      |<span data-ttu-id="9a2bc-128">Если больше 0, этот атрибут будет использоваться для первоначального совпадения объектов между исходным и целевым каталогами.</span><span class="sxs-lookup"><span data-stu-id="9a2bc-128">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="9a2bc-129">Механизм синхронизации попытается найти совпадающий объект с помощью атрибута с наименьшим значением приоритета.</span><span class="sxs-lookup"><span data-stu-id="9a2bc-129">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="9a2bc-130">Если этот атрибут не найден, будет использоваться атрибут с следующим совпадающий приоритетом и так далее до тех пор, пока совпадение не будет найдено или больше совпадающие атрибуты не будут оставлены.</span><span class="sxs-lookup"><span data-stu-id="9a2bc-130">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="9a2bc-131">В качестве совпадающих атрибутов следует использовать только те атрибуты, которые должны иметь уникальные значения, например электронную почту.</span><span class="sxs-lookup"><span data-stu-id="9a2bc-131">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="9a2bc-132">source</span><span class="sxs-lookup"><span data-stu-id="9a2bc-132">source</span></span>                     |[<span data-ttu-id="9a2bc-133">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="9a2bc-133">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="9a2bc-134">Определяет, как значение должно быть извлечено (или преобразовано) из объекта-источника.</span><span class="sxs-lookup"><span data-stu-id="9a2bc-134">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="9a2bc-135">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="9a2bc-135">targetAttributeName</span></span>        |<span data-ttu-id="9a2bc-136">Строка</span><span class="sxs-lookup"><span data-stu-id="9a2bc-136">String</span></span>                     |<span data-ttu-id="9a2bc-137">Имя атрибута в целевом объекте.</span><span class="sxs-lookup"><span data-stu-id="9a2bc-137">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9a2bc-138">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9a2bc-138">JSON representation</span></span>

<span data-ttu-id="9a2bc-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9a2bc-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMapping"
}-->

```json
{
  "defaultValue": "String",
  "exportMissingReferences": true,
  "flowBehavior": "String",
  "flowType": "String",
  "matchingPriority": 1024,
  "source": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "targetAttributeName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


