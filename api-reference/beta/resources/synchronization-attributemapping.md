---
title: Тип ресурса attributeMapping
description: Определяет, как значения для атрибута заданный целевой поток во время синхронизации.
localization_priority: Normal
ms.openlocfilehash: 6c7a6367684b3e11013355b6d4726afe3346dab9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825279"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="c9dcc-103">Тип ресурса attributeMapping</span><span class="sxs-lookup"><span data-stu-id="c9dcc-103">attributeMapping resource type</span></span>

> <span data-ttu-id="c9dcc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c9dcc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9dcc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c9dcc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c9dcc-106">Определяет, как значения для атрибута заданный целевой поток во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="c9dcc-106">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="c9dcc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c9dcc-107">Properties</span></span>

| <span data-ttu-id="c9dcc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c9dcc-108">Property</span></span>                  | <span data-ttu-id="c9dcc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c9dcc-109">Type</span></span>                      | <span data-ttu-id="c9dcc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c9dcc-110">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="c9dcc-111">defaultValue</span><span class="sxs-lookup"><span data-stu-id="c9dcc-111">defaultValue</span></span>               | <span data-ttu-id="c9dcc-112">String</span><span class="sxs-lookup"><span data-stu-id="c9dcc-112">String</span></span>                    |<span data-ttu-id="c9dcc-113">По умолчанию значение для использования в случае, если свойство **source** проверялись `null`.</span><span class="sxs-lookup"><span data-stu-id="c9dcc-113">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="c9dcc-114">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="c9dcc-114">Optional.</span></span>|
|<span data-ttu-id="c9dcc-115">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="c9dcc-115">exportMissingReferences</span></span>    |<span data-ttu-id="c9dcc-116">Строка</span><span class="sxs-lookup"><span data-stu-id="c9dcc-116">String</span></span>                     |<span data-ttu-id="c9dcc-117">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="c9dcc-117">For internal use only.</span></span>|
|<span data-ttu-id="c9dcc-118">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="c9dcc-118">flowBehavior</span></span>               |<span data-ttu-id="c9dcc-119">attributeFlowBehavior</span><span class="sxs-lookup"><span data-stu-id="c9dcc-119">attributeFlowBehavior</span></span>      |<span data-ttu-id="c9dcc-120">Определяет, когда этот атрибут, должны быть экспортированы в конечный каталог.</span><span class="sxs-lookup"><span data-stu-id="c9dcc-120">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="c9dcc-121">Возможные значения: `FlowWhenChanged` и `FlowAlways`.</span><span class="sxs-lookup"><span data-stu-id="c9dcc-121">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="c9dcc-122">Значение по умолчанию: `FlowWhenChanged`.</span><span class="sxs-lookup"><span data-stu-id="c9dcc-122">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="c9dcc-123">flowType</span><span class="sxs-lookup"><span data-stu-id="c9dcc-123">flowType</span></span>                   |<span data-ttu-id="c9dcc-124">attributeFlowType</span><span class="sxs-lookup"><span data-stu-id="c9dcc-124">attributeFlowType</span></span>          |<span data-ttu-id="c9dcc-125">Определяет, когда этот атрибут следует обновить в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="c9dcc-125">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="c9dcc-126">Возможные значения: `Always` (по умолчанию), `ObjectAddOnly` (только если создается новый объект), `MultiValueAddOnly` (только при изменении добавляет новые значения это многозначный атрибут).</span><span class="sxs-lookup"><span data-stu-id="c9dcc-126">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="c9dcc-127">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="c9dcc-127">matchingPriority</span></span>           |<span data-ttu-id="c9dcc-128">Int32</span><span class="sxs-lookup"><span data-stu-id="c9dcc-128">Int32</span></span>                      |<span data-ttu-id="c9dcc-129">Если больше 0, этот атрибут будет использоваться для выполнения первоначальной совпадение объектов между исходный и конечный каталоги.</span><span class="sxs-lookup"><span data-stu-id="c9dcc-129">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="c9dcc-130">Обработчик синхронизации попытается найти соответствующий объект, с помощью атрибута с наименьшее значение сначала совпадающих приоритет.</span><span class="sxs-lookup"><span data-stu-id="c9dcc-130">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="c9dcc-131">Если не найден, атрибута с помощью следующего соответствия приоритет будет использоваться и так далее до совпадения или исключаются соответствующие атрибуты.</span><span class="sxs-lookup"><span data-stu-id="c9dcc-131">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="c9dcc-132">Только атрибуты, которые должны иметь уникальные значения, такие как электронной почтой, следует использовать в качестве соответствующие атрибуты.</span><span class="sxs-lookup"><span data-stu-id="c9dcc-132">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="c9dcc-133">source</span><span class="sxs-lookup"><span data-stu-id="c9dcc-133">source</span></span>                     |[<span data-ttu-id="c9dcc-134">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="c9dcc-134">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="c9dcc-135">Определяет, как должно быть значение извлечены (или преобразовать) из исходного объекта.</span><span class="sxs-lookup"><span data-stu-id="c9dcc-135">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="c9dcc-136">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="c9dcc-136">targetAttributeName</span></span>        |<span data-ttu-id="c9dcc-137">Строка</span><span class="sxs-lookup"><span data-stu-id="c9dcc-137">String</span></span>                     |<span data-ttu-id="c9dcc-138">Имя атрибута для конечного объекта.</span><span class="sxs-lookup"><span data-stu-id="c9dcc-138">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c9dcc-139">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c9dcc-139">JSON representation</span></span>

<span data-ttu-id="c9dcc-140">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c9dcc-140">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
