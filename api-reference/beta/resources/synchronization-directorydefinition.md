---
title: Тип ресурса Директоридефинитион
description: Предоставляет сведения о модуле синхронизации для каталога и его объектов.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b18c34a316f9c1f0c91617d7170c5050630af235
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219146"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="c4e0a-103">Тип ресурса Директоридефинитион</span><span class="sxs-lookup"><span data-stu-id="c4e0a-103">directoryDefinition resource type</span></span>

<span data-ttu-id="c4e0a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4e0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4e0a-105">Предоставляет сведения о модуле синхронизации для каталога и его объектов.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-105">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="c4e0a-106">Этот ресурс сообщает обработчику синхронизации, например, что каталог содержит объекты с именем **User** и **Group**, какие атрибуты поддерживаются для этих объектов, и типы этих атрибутов.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-106">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="c4e0a-107">Чтобы объект и атрибут участвовали в [правилах синхронизации](synchronization-synchronizationrule.md) и [сопоставлениях объектов](synchronization-objectmapping.md), они должны быть определены как часть определения каталога.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-107">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="c4e0a-108">Как правило, [схема синхронизации](synchronization-synchronizationschema.md) по умолчанию, предоставляемая как часть [шаблона синхронизации](synchronization-synchronizationtemplate.md) , определяет наиболее часто используемые объекты и атрибуты для этого каталога.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-108">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="c4e0a-109">Тем не менее, если каталог поддерживает добавление настраиваемых атрибутов, можно расширить определение DEFAULT с использованием собственных настраиваемых объектов или атрибутов.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-109">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="c4e0a-110">Дополнительные сведения см. в статье [Настройка синхронизации с настраиваемыми атрибутами](synchronization-configure-with-custom-target-attributes.md) и [Настройка синхронизации с атрибутами расширения каталога](synchronization-configure-with-directory-extension-attributes.md).</span><span class="sxs-lookup"><span data-stu-id="c4e0a-110">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="c4e0a-111">Определения каталогов обновляются в составе [схемы синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="c4e0a-111">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c4e0a-112">Методы</span><span class="sxs-lookup"><span data-stu-id="c4e0a-112">Methods</span></span>

| <span data-ttu-id="c4e0a-113">Метод</span><span class="sxs-lookup"><span data-stu-id="c4e0a-113">Method</span></span>       | <span data-ttu-id="c4e0a-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c4e0a-114">Return Type</span></span>  |<span data-ttu-id="c4e0a-115">Описание</span><span class="sxs-lookup"><span data-stu-id="c4e0a-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c4e0a-116">Обнаружение Директоридефинитион</span><span class="sxs-lookup"><span data-stu-id="c4e0a-116">Discover directoryDefinition</span></span>](../api/directorydefinition-discover.md) | [<span data-ttu-id="c4e0a-117">директоридефинитион</span><span class="sxs-lookup"><span data-stu-id="c4e0a-117">directoryDefinition</span></span>](synchronization-directorydefinition.md) |<span data-ttu-id="c4e0a-118">Определение схемы и поддерживаемых свойств каталога.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-118">Discover the schema and supported properties of the directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="c4e0a-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4e0a-119">Properties</span></span>

| <span data-ttu-id="c4e0a-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4e0a-120">Property</span></span>      | <span data-ttu-id="c4e0a-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c4e0a-121">Type</span></span>      | <span data-ttu-id="c4e0a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c4e0a-122">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="c4e0a-123">id</span><span class="sxs-lookup"><span data-stu-id="c4e0a-123">id</span></span>           |<span data-ttu-id="c4e0a-124">Строка</span><span class="sxs-lookup"><span data-stu-id="c4e0a-124">String</span></span>     |<span data-ttu-id="c4e0a-125">Идентификатор каталога.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-125">Directory identifier.</span></span> <span data-ttu-id="c4e0a-126">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-126">Not nullable.</span></span>|
|<span data-ttu-id="c4e0a-127">метаданных</span><span class="sxs-lookup"><span data-stu-id="c4e0a-127">metadata</span></span>       |<span data-ttu-id="c4e0a-128">Коллекция Метадатаентри</span><span class="sxs-lookup"><span data-stu-id="c4e0a-128">metadataEntry collection</span></span>    |<span data-ttu-id="c4e0a-129">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-129">Additional extension properties.</span></span> <span data-ttu-id="c4e0a-130">Если явно не указано иное, значения метаданных не должны изменяться.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-130">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="c4e0a-131">name</span><span class="sxs-lookup"><span data-stu-id="c4e0a-131">name</span></span>           |<span data-ttu-id="c4e0a-132">String</span><span class="sxs-lookup"><span data-stu-id="c4e0a-132">String</span></span>     |<span data-ttu-id="c4e0a-133">Имя каталога.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-133">Name of the directory.</span></span> <span data-ttu-id="c4e0a-134">Должно быть уникальным в пределах [схемы синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="c4e0a-134">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="c4e0a-135">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-135">Not nullable.</span></span>|
|<span data-ttu-id="c4e0a-136">см</span><span class="sxs-lookup"><span data-stu-id="c4e0a-136">objects</span></span>        |<span data-ttu-id="c4e0a-137">Коллекция [обжектдефинитион](synchronization-objectdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="c4e0a-137">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="c4e0a-138">Коллекция объектов, поддерживаемая каталогом.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-138">Collection of objects supported by the directory.</span></span>|
|<span data-ttu-id="c4e0a-139">version</span><span class="sxs-lookup"><span data-stu-id="c4e0a-139">version</span></span>|<span data-ttu-id="c4e0a-140">String</span><span class="sxs-lookup"><span data-stu-id="c4e0a-140">String</span></span>|<span data-ttu-id="c4e0a-141">Значение только для чтения, которое указывает обнаруженную версию.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-141">Read only value that indicates version discovered.</span></span> <span data-ttu-id="c4e0a-142">Значение null, если обнаружение еще не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-142">Null if discovery has not yet occurred.</span></span>|
|<span data-ttu-id="c4e0a-143">дисковеридатетиме</span><span class="sxs-lookup"><span data-stu-id="c4e0a-143">discoveryDateTime</span></span>|<span data-ttu-id="c4e0a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4e0a-144">DateTimeOffset</span></span>| <span data-ttu-id="c4e0a-145">Представляет дату и время обнаружения с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-145">Represents the discovery date and time using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c4e0a-146">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-146">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c4e0a-147">дисковерабилитиес</span><span class="sxs-lookup"><span data-stu-id="c4e0a-147">discoverabilities</span></span>|<span data-ttu-id="c4e0a-148">string</span><span class="sxs-lookup"><span data-stu-id="c4e0a-148">string</span></span>| <span data-ttu-id="c4e0a-149">Значение только для чтения, указывающее тип обнаружения, поддерживаемый приложением.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-149">Read only value indicating what type of discovery the app supports.</span></span> <span data-ttu-id="c4e0a-150">Возможные значения: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-150">Possible values are: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="c4e0a-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4e0a-151">JSON representation</span></span>

<span data-ttu-id="c4e0a-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4e0a-152">The following is a JSON representation of the resource.</span></span>

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
