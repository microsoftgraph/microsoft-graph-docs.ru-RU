---
title: Тип ресурса directoryDefinition
description: Предоставляет механизм синхронизации сведения о каталоге и его объектах.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 77af192ff09cf557eec3e73c1973c4c71dc39a96
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134052"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="e477e-103">Тип ресурса directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="e477e-103">directoryDefinition resource type</span></span>

<span data-ttu-id="e477e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e477e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e477e-105">Предоставляет механизм синхронизации сведения о каталоге и его объектах.</span><span class="sxs-lookup"><span data-stu-id="e477e-105">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="e477e-106">Этот ресурс сообщает механизму синхронизации, например, что каталог имеет объекты с именем **user** и **group,** какие атрибуты поддерживаются для этих объектов, а также типы этих атрибутов.</span><span class="sxs-lookup"><span data-stu-id="e477e-106">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="e477e-107">Чтобы объект и атрибут участвовали [](synchronization-synchronizationrule.md) в правилах синхронизации и сопоставлениях [объектов,](synchronization-objectmapping.md)их необходимо определить как часть определения каталога.</span><span class="sxs-lookup"><span data-stu-id="e477e-107">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="e477e-108">Как правило, [](synchronization-synchronizationschema.md) схема синхронизации по умолчанию, [](synchronization-synchronizationtemplate.md) предоставляемая в рамках шаблона синхронизации, определяет наиболее часто используемые объекты и атрибуты для этого каталога.</span><span class="sxs-lookup"><span data-stu-id="e477e-108">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="e477e-109">Однако если каталог поддерживает добавление настраиваемого атрибута, может потребоваться расширить определение по умолчанию с помощью собственных настраиваемые объекты или атрибуты.</span><span class="sxs-lookup"><span data-stu-id="e477e-109">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="e477e-110">Дополнительные сведения см. в подстройке ["Настройка](synchronization-configure-with-custom-target-attributes.md) синхронизации с настраиваемой атрибутами" и "Настройка синхронизации с атрибутами [расширения каталога".](synchronization-configure-with-directory-extension-attributes.md)</span><span class="sxs-lookup"><span data-stu-id="e477e-110">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="e477e-111">Определения каталогов обновляются в рамках схемы [синхронизации.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="e477e-111">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e477e-112">Методы</span><span class="sxs-lookup"><span data-stu-id="e477e-112">Methods</span></span>

| <span data-ttu-id="e477e-113">Метод</span><span class="sxs-lookup"><span data-stu-id="e477e-113">Method</span></span>       | <span data-ttu-id="e477e-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e477e-114">Return Type</span></span>  |<span data-ttu-id="e477e-115">Описание</span><span class="sxs-lookup"><span data-stu-id="e477e-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e477e-116">Обнаружение directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="e477e-116">Discover directoryDefinition</span></span>](../api/directorydefinition-discover.md) | [<span data-ttu-id="e477e-117">directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="e477e-117">directoryDefinition</span></span>](synchronization-directorydefinition.md) |<span data-ttu-id="e477e-118">Обнаружение схемы и поддерживаемых свойств каталога.</span><span class="sxs-lookup"><span data-stu-id="e477e-118">Discover the schema and supported properties of the directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="e477e-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="e477e-119">Properties</span></span>

| <span data-ttu-id="e477e-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="e477e-120">Property</span></span>      | <span data-ttu-id="e477e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e477e-121">Type</span></span>      | <span data-ttu-id="e477e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e477e-122">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="e477e-123">id</span><span class="sxs-lookup"><span data-stu-id="e477e-123">id</span></span>           |<span data-ttu-id="e477e-124">Строка</span><span class="sxs-lookup"><span data-stu-id="e477e-124">String</span></span>     |<span data-ttu-id="e477e-125">Идентификатор каталога.</span><span class="sxs-lookup"><span data-stu-id="e477e-125">Directory identifier.</span></span> <span data-ttu-id="e477e-126">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="e477e-126">Not nullable.</span></span>|
|<span data-ttu-id="e477e-127">метаданные</span><span class="sxs-lookup"><span data-stu-id="e477e-127">metadata</span></span>       |<span data-ttu-id="e477e-128">Коллекция metadataEntry</span><span class="sxs-lookup"><span data-stu-id="e477e-128">metadataEntry collection</span></span>    |<span data-ttu-id="e477e-129">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="e477e-129">Additional extension properties.</span></span> <span data-ttu-id="e477e-130">Если не было явно упомянуто, значения метаданных не следует менять.</span><span class="sxs-lookup"><span data-stu-id="e477e-130">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="e477e-131">name</span><span class="sxs-lookup"><span data-stu-id="e477e-131">name</span></span>           |<span data-ttu-id="e477e-132">String</span><span class="sxs-lookup"><span data-stu-id="e477e-132">String</span></span>     |<span data-ttu-id="e477e-133">Имя каталога.</span><span class="sxs-lookup"><span data-stu-id="e477e-133">Name of the directory.</span></span> <span data-ttu-id="e477e-134">Должен быть уникальным в [схеме синхронизации.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="e477e-134">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="e477e-135">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="e477e-135">Not nullable.</span></span>|
|<span data-ttu-id="e477e-136">objects</span><span class="sxs-lookup"><span data-stu-id="e477e-136">objects</span></span>        |<span data-ttu-id="e477e-137">[Коллекция objectDefinition](synchronization-objectdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e477e-137">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="e477e-138">Коллекция объектов, поддерживаемых каталогом.</span><span class="sxs-lookup"><span data-stu-id="e477e-138">Collection of objects supported by the directory.</span></span>|
|<span data-ttu-id="e477e-139">version</span><span class="sxs-lookup"><span data-stu-id="e477e-139">version</span></span>|<span data-ttu-id="e477e-140">String</span><span class="sxs-lookup"><span data-stu-id="e477e-140">String</span></span>|<span data-ttu-id="e477e-141">Только для чтения значения, которое указывает обнаруженную версию.</span><span class="sxs-lookup"><span data-stu-id="e477e-141">Read only value that indicates version discovered.</span></span> <span data-ttu-id="e477e-142">NULL, если обнаружение еще не произошло.</span><span class="sxs-lookup"><span data-stu-id="e477e-142">Null if discovery has not yet occurred.</span></span>|
|<span data-ttu-id="e477e-143">discoveryDateTime</span><span class="sxs-lookup"><span data-stu-id="e477e-143">discoveryDateTime</span></span>|<span data-ttu-id="e477e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e477e-144">DateTimeOffset</span></span>| <span data-ttu-id="e477e-145">Представляет дату и время обнаружения в формате ISO 8601 и всегда используется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="e477e-145">Represents the discovery date and time using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e477e-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="e477e-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e477e-147">discoverabilities</span><span class="sxs-lookup"><span data-stu-id="e477e-147">discoverabilities</span></span>|<span data-ttu-id="e477e-148">string</span><span class="sxs-lookup"><span data-stu-id="e477e-148">string</span></span>| <span data-ttu-id="e477e-149">Только для чтения, указывающее тип обнаружения, поддерживаемого приложением.</span><span class="sxs-lookup"><span data-stu-id="e477e-149">Read only value indicating what type of discovery the app supports.</span></span> <span data-ttu-id="e477e-150">Возможные значения: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e477e-150">Possible values are: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="e477e-151">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e477e-151">JSON representation</span></span>

<span data-ttu-id="e477e-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e477e-152">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryDefinition"
}-->

```json
{
  "discoverabilities": "String",
  "discoveryDateTime": "DateTimeOffset",
  "id": "String",
  "metadata": [{"@odata.type": "microsoft.graph.stringKeyStringValuePair"}],
  "name": "String",
  "objects": [{"@odata.type": "microsoft.graph.objectDefinition"}],
  "version": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


