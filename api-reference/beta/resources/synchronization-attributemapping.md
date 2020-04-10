---
title: Тип ресурса Аттрибутемаппинг
description: Определяет, как должны передаваться значения для данного целевого атрибута во время синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bbc671c6796d985cfee910f773fafc4d71eab51c
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219188"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="febf2-103">Тип ресурса Аттрибутемаппинг</span><span class="sxs-lookup"><span data-stu-id="febf2-103">attributeMapping resource type</span></span>

<span data-ttu-id="febf2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="febf2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="febf2-105">Определяет, как должны передаваться значения для данного целевого атрибута во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="febf2-105">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="febf2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="febf2-106">Properties</span></span>

| <span data-ttu-id="febf2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="febf2-107">Property</span></span>                  | <span data-ttu-id="febf2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="febf2-108">Type</span></span>                      | <span data-ttu-id="febf2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="febf2-109">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="febf2-110">Значение</span><span class="sxs-lookup"><span data-stu-id="febf2-110">defaultValue</span></span>               | <span data-ttu-id="febf2-111">Строка</span><span class="sxs-lookup"><span data-stu-id="febf2-111">String</span></span>                    |<span data-ttu-id="febf2-112">Значение по умолчанию, используемое в **source** случае, если свойство Source `null`было оценено.</span><span class="sxs-lookup"><span data-stu-id="febf2-112">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="febf2-113">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="febf2-113">Optional.</span></span>|
|<span data-ttu-id="febf2-114">експортмиссингреференцес</span><span class="sxs-lookup"><span data-stu-id="febf2-114">exportMissingReferences</span></span>    |<span data-ttu-id="febf2-115">String</span><span class="sxs-lookup"><span data-stu-id="febf2-115">String</span></span>                     |<span data-ttu-id="febf2-116">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="febf2-116">For internal use only.</span></span>|
|<span data-ttu-id="febf2-117">фловбехавиор</span><span class="sxs-lookup"><span data-stu-id="febf2-117">flowBehavior</span></span>               |<span data-ttu-id="febf2-118">аттрибутефловбехавиор</span><span class="sxs-lookup"><span data-stu-id="febf2-118">attributeFlowBehavior</span></span>      |<span data-ttu-id="febf2-119">Определяет, когда этот атрибут должен быть экспортирован в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="febf2-119">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="febf2-120">Возможные значения: `FlowWhenChanged` и `FlowAlways`.</span><span class="sxs-lookup"><span data-stu-id="febf2-120">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="febf2-121">Значение по умолчанию: `FlowWhenChanged`.</span><span class="sxs-lookup"><span data-stu-id="febf2-121">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="febf2-122">фловтипе</span><span class="sxs-lookup"><span data-stu-id="febf2-122">flowType</span></span>                   |<span data-ttu-id="febf2-123">аттрибутефловтипе</span><span class="sxs-lookup"><span data-stu-id="febf2-123">attributeFlowType</span></span>          |<span data-ttu-id="febf2-124">Определяет, когда этот атрибут должен быть обновлен в целевом каталоге.</span><span class="sxs-lookup"><span data-stu-id="febf2-124">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="febf2-125">Возможные значения: `Always` (по умолчанию) `ObjectAddOnly` (только при создании нового объекта) `MultiValueAddOnly` (только когда изменение добавляет новые значения в атрибут с несколькими значениями).</span><span class="sxs-lookup"><span data-stu-id="febf2-125">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="febf2-126">матчингприорити</span><span class="sxs-lookup"><span data-stu-id="febf2-126">matchingPriority</span></span>           |<span data-ttu-id="febf2-127">Int32</span><span class="sxs-lookup"><span data-stu-id="febf2-127">Int32</span></span>                      |<span data-ttu-id="febf2-128">Если значение больше 0, этот атрибут будет использоваться для выполнения начального сопоставления объектов между исходным и целевым каталогами.</span><span class="sxs-lookup"><span data-stu-id="febf2-128">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="febf2-129">Обработчик синхронизации попытается найти совпадающий объект с использованием атрибута с наименьшим значением приоритета совпадения первыми.</span><span class="sxs-lookup"><span data-stu-id="febf2-129">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="febf2-130">Если этот параметр не найден, будет использоваться атрибут с соответствующим приоритетом, и поэтому при обнаружении совпадения и других атрибутах совпадения не осталось.</span><span class="sxs-lookup"><span data-stu-id="febf2-130">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="febf2-131">В качестве искомых атрибутов следует использовать только те атрибуты, которые должны иметь уникальные значения (например, электронная почта).</span><span class="sxs-lookup"><span data-stu-id="febf2-131">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="febf2-132">source</span><span class="sxs-lookup"><span data-stu-id="febf2-132">source</span></span>                     |[<span data-ttu-id="febf2-133">аттрибутемаппингсаурце</span><span class="sxs-lookup"><span data-stu-id="febf2-133">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="febf2-134">Определяет способ извлечения (или преобразования) значения из исходного объекта.</span><span class="sxs-lookup"><span data-stu-id="febf2-134">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="febf2-135">таржетаттрибутенаме</span><span class="sxs-lookup"><span data-stu-id="febf2-135">targetAttributeName</span></span>        |<span data-ttu-id="febf2-136">Строка</span><span class="sxs-lookup"><span data-stu-id="febf2-136">String</span></span>                     |<span data-ttu-id="febf2-137">Имя атрибута в целевом объекте.</span><span class="sxs-lookup"><span data-stu-id="febf2-137">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="febf2-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="febf2-138">JSON representation</span></span>

<span data-ttu-id="febf2-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="febf2-139">The following is a JSON representation of the resource.</span></span>

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
