---
title: Тип ресурса Аттрибутемаппинг
description: Определяет, как должны передаваться значения для данного целевого атрибута во время синхронизации.
localization_priority: Normal
ms.openlocfilehash: 16235cce73a17b462f6f44aedf0c8759277983c1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582118"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="fb4fb-103">Тип ресурса Аттрибутемаппинг</span><span class="sxs-lookup"><span data-stu-id="fb4fb-103">attributeMapping resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb4fb-104">Определяет, как должны передаваться значения для данного целевого атрибута во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="fb4fb-104">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="fb4fb-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb4fb-105">Properties</span></span>

| <span data-ttu-id="fb4fb-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb4fb-106">Property</span></span>                  | <span data-ttu-id="fb4fb-107">Тип</span><span class="sxs-lookup"><span data-stu-id="fb4fb-107">Type</span></span>                      | <span data-ttu-id="fb4fb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fb4fb-108">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="fb4fb-109">Значение</span><span class="sxs-lookup"><span data-stu-id="fb4fb-109">defaultValue</span></span>               | <span data-ttu-id="fb4fb-110">String</span><span class="sxs-lookup"><span data-stu-id="fb4fb-110">String</span></span>                    |<span data-ttu-id="fb4fb-111">Значение по умолчанию, используемое в \*\*\*\* случае, если свойство Source `null`было оценено.</span><span class="sxs-lookup"><span data-stu-id="fb4fb-111">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="fb4fb-112">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="fb4fb-112">Optional.</span></span>|
|<span data-ttu-id="fb4fb-113">Експортмиссингреференцес</span><span class="sxs-lookup"><span data-stu-id="fb4fb-113">exportMissingReferences</span></span>    |<span data-ttu-id="fb4fb-114">String</span><span class="sxs-lookup"><span data-stu-id="fb4fb-114">String</span></span>                     |<span data-ttu-id="fb4fb-115">Только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="fb4fb-115">For internal use only.</span></span>|
|<span data-ttu-id="fb4fb-116">Фловбехавиор</span><span class="sxs-lookup"><span data-stu-id="fb4fb-116">flowBehavior</span></span>               |<span data-ttu-id="fb4fb-117">Аттрибутефловбехавиор</span><span class="sxs-lookup"><span data-stu-id="fb4fb-117">attributeFlowBehavior</span></span>      |<span data-ttu-id="fb4fb-118">Определяет, когда этот атрибут должен быть экспортирован в целевой каталог.</span><span class="sxs-lookup"><span data-stu-id="fb4fb-118">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="fb4fb-119">Возможные значения: `FlowWhenChanged` и `FlowAlways`.</span><span class="sxs-lookup"><span data-stu-id="fb4fb-119">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="fb4fb-120">Значение по умолчанию: `FlowWhenChanged`.</span><span class="sxs-lookup"><span data-stu-id="fb4fb-120">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="fb4fb-121">Фловтипе</span><span class="sxs-lookup"><span data-stu-id="fb4fb-121">flowType</span></span>                   |<span data-ttu-id="fb4fb-122">Аттрибутефловтипе</span><span class="sxs-lookup"><span data-stu-id="fb4fb-122">attributeFlowType</span></span>          |<span data-ttu-id="fb4fb-123">Определяет, когда этот атрибут должен быть обновлен в целевом каталоге.</span><span class="sxs-lookup"><span data-stu-id="fb4fb-123">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="fb4fb-124">Возможные значения: `Always` (по умолчанию) `ObjectAddOnly` (только при создании нового объекта) `MultiValueAddOnly` (только когда изменение добавляет новые значения в атрибут с несколькими значениями).</span><span class="sxs-lookup"><span data-stu-id="fb4fb-124">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="fb4fb-125">Матчингприорити</span><span class="sxs-lookup"><span data-stu-id="fb4fb-125">matchingPriority</span></span>           |<span data-ttu-id="fb4fb-126">Int32</span><span class="sxs-lookup"><span data-stu-id="fb4fb-126">Int32</span></span>                      |<span data-ttu-id="fb4fb-127">Если значение больше 0, этот атрибут будет использоваться для выполнения начального сопоставления объектов между исходным и целевым каталогами.</span><span class="sxs-lookup"><span data-stu-id="fb4fb-127">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="fb4fb-128">Обработчик синхронизации попытается найти совпадающий объект с использованием атрибута с наименьшим значением приоритета совпадения первыми.</span><span class="sxs-lookup"><span data-stu-id="fb4fb-128">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="fb4fb-129">Если этот параметр не найден, будет использоваться атрибут с соответствующим приоритетом, и поэтому при обнаружении совпадения и других атрибутах совпадения не осталось.</span><span class="sxs-lookup"><span data-stu-id="fb4fb-129">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="fb4fb-130">В качестве искомых атрибутов следует использовать только те атрибуты, которые должны иметь уникальные значения (например, электронная почта).</span><span class="sxs-lookup"><span data-stu-id="fb4fb-130">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="fb4fb-131">source</span><span class="sxs-lookup"><span data-stu-id="fb4fb-131">source</span></span>                     |[<span data-ttu-id="fb4fb-132">Аттрибутемаппингсаурце</span><span class="sxs-lookup"><span data-stu-id="fb4fb-132">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="fb4fb-133">Определяет способ извлечения (или преобразования) значения из исходного объекта.</span><span class="sxs-lookup"><span data-stu-id="fb4fb-133">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="fb4fb-134">Таржетаттрибутенаме</span><span class="sxs-lookup"><span data-stu-id="fb4fb-134">targetAttributeName</span></span>        |<span data-ttu-id="fb4fb-135">String</span><span class="sxs-lookup"><span data-stu-id="fb4fb-135">String</span></span>                     |<span data-ttu-id="fb4fb-136">Имя атрибута в целевом объекте.</span><span class="sxs-lookup"><span data-stu-id="fb4fb-136">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="fb4fb-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb4fb-137">JSON representation</span></span>

<span data-ttu-id="fb4fb-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb4fb-138">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemapping.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
