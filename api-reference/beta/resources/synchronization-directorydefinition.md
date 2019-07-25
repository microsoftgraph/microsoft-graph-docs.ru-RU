---
title: Тип ресурса Директоридефинитион
description: Предоставляет сведения о модуле синхронизации для каталога и его объектов.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 56c1f5a6a15f7ab6724feff68aa38eba1ef22694
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888141"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="0878f-103">Тип ресурса Директоридефинитион</span><span class="sxs-lookup"><span data-stu-id="0878f-103">directoryDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0878f-104">Предоставляет сведения о модуле синхронизации для каталога и его объектов.</span><span class="sxs-lookup"><span data-stu-id="0878f-104">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="0878f-105">Этот ресурс сообщает обработчику синхронизации, например, что каталог содержит объекты с именем **User** и **Group**, какие атрибуты поддерживаются для этих объектов, и типы этих атрибутов.</span><span class="sxs-lookup"><span data-stu-id="0878f-105">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="0878f-106">Чтобы объект и атрибут участвовали в [правилах синхронизации](synchronization-synchronizationrule.md) и сопоставлениях [объектов](synchronization-objectmapping.md), они должны быть определены как часть определения каталога.</span><span class="sxs-lookup"><span data-stu-id="0878f-106">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="0878f-107">Как правило, [схема синхронизации](synchronization-synchronizationschema.md) по умолчанию, предоставляемая как часть [шаблона синхронизации](synchronization-synchronizationtemplate.md) , определяет наиболее часто используемые объекты и атрибуты для этого каталога.</span><span class="sxs-lookup"><span data-stu-id="0878f-107">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="0878f-108">Тем не менее, если каталог поддерживает добавление настраиваемых атрибутов, можно расширить определение DEFAULT с использованием собственных настраиваемых объектов или атрибутов.</span><span class="sxs-lookup"><span data-stu-id="0878f-108">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="0878f-109">Дополнительные сведения см. в статье [Настройка синхронизации с настраиваемыми атрибутами](synchronization-configure-with-custom-target-attributes.md) и [Настройка синхронизации с атрибутами расширения каталога](synchronization-configure-with-directory-extension-attributes.md).</span><span class="sxs-lookup"><span data-stu-id="0878f-109">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="0878f-110">Определения каталогов обновляются в составе [схемы синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="0878f-110">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="0878f-111">Методы</span><span class="sxs-lookup"><span data-stu-id="0878f-111">Methods</span></span>

| <span data-ttu-id="0878f-112">Метод</span><span class="sxs-lookup"><span data-stu-id="0878f-112">Method</span></span>       | <span data-ttu-id="0878f-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0878f-113">Return Type</span></span>  |<span data-ttu-id="0878f-114">Описание</span><span class="sxs-lookup"><span data-stu-id="0878f-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0878f-115">Обнаружение Директоридефинитион</span><span class="sxs-lookup"><span data-stu-id="0878f-115">Discover directoryDefinition</span></span>](../api/directorydefinition-discover.md) | [<span data-ttu-id="0878f-116">Директоридефинитион</span><span class="sxs-lookup"><span data-stu-id="0878f-116">directoryDefinition</span></span>](synchronization-directorydefinition.md) |<span data-ttu-id="0878f-117">Определение схемы и поддерживаемых свойств каталога.</span><span class="sxs-lookup"><span data-stu-id="0878f-117">Discover the schema and supported properties of the directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="0878f-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="0878f-118">Properties</span></span>

| <span data-ttu-id="0878f-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="0878f-119">Property</span></span>      | <span data-ttu-id="0878f-120">Тип</span><span class="sxs-lookup"><span data-stu-id="0878f-120">Type</span></span>      | <span data-ttu-id="0878f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0878f-121">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="0878f-122">id</span><span class="sxs-lookup"><span data-stu-id="0878f-122">id</span></span>           |<span data-ttu-id="0878f-123">Строка</span><span class="sxs-lookup"><span data-stu-id="0878f-123">String</span></span>     |<span data-ttu-id="0878f-124">Идентификатор каталога.</span><span class="sxs-lookup"><span data-stu-id="0878f-124">Directory identifier.</span></span> <span data-ttu-id="0878f-125">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="0878f-125">Not nullable.</span></span>|
|<span data-ttu-id="0878f-126">метаданных</span><span class="sxs-lookup"><span data-stu-id="0878f-126">metadata</span></span>       |<span data-ttu-id="0878f-127">Коллекция Метадатаентри</span><span class="sxs-lookup"><span data-stu-id="0878f-127">metadataEntry collection</span></span>    |<span data-ttu-id="0878f-128">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="0878f-128">Additional extension properties.</span></span> <span data-ttu-id="0878f-129">Если явно не указано иное, значения метаданных не должны изменяться.</span><span class="sxs-lookup"><span data-stu-id="0878f-129">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="0878f-130">name</span><span class="sxs-lookup"><span data-stu-id="0878f-130">name</span></span>           |<span data-ttu-id="0878f-131">String</span><span class="sxs-lookup"><span data-stu-id="0878f-131">String</span></span>     |<span data-ttu-id="0878f-132">Имя каталога.</span><span class="sxs-lookup"><span data-stu-id="0878f-132">Name of the directory.</span></span> <span data-ttu-id="0878f-133">Должно быть уникальным в пределах [схемы синхронизации](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="0878f-133">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="0878f-134">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="0878f-134">Not nullable.</span></span>|
|<span data-ttu-id="0878f-135">см</span><span class="sxs-lookup"><span data-stu-id="0878f-135">objects</span></span>        |<span data-ttu-id="0878f-136">Коллекция [обжектдефинитион](synchronization-objectdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="0878f-136">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="0878f-137">Коллекция объектов, поддерживаемая каталогом.</span><span class="sxs-lookup"><span data-stu-id="0878f-137">Collection of objects supported by the directory.</span></span>|
|<span data-ttu-id="0878f-138">version</span><span class="sxs-lookup"><span data-stu-id="0878f-138">version</span></span>|<span data-ttu-id="0878f-139">String</span><span class="sxs-lookup"><span data-stu-id="0878f-139">String</span></span>|<span data-ttu-id="0878f-140">Значение только для чтения, которое указывает обнаруженную версию.</span><span class="sxs-lookup"><span data-stu-id="0878f-140">Read only value that indicates version discovered.</span></span> <span data-ttu-id="0878f-141">Значение null, если обнаружение еще не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="0878f-141">Null if discovery has not yet occurred.</span></span>|
|<span data-ttu-id="0878f-142">Дисковеридатетиме</span><span class="sxs-lookup"><span data-stu-id="0878f-142">discoveryDateTime</span></span>|<span data-ttu-id="0878f-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0878f-143">DateTimeOffset</span></span>| <span data-ttu-id="0878f-144">Представляет дату и время обнаружения с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="0878f-144">Represents the discovery date and time using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0878f-145">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="0878f-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0878f-146">дисковерабилитиес</span><span class="sxs-lookup"><span data-stu-id="0878f-146">discoverabilities</span></span>|<span data-ttu-id="0878f-147">string</span><span class="sxs-lookup"><span data-stu-id="0878f-147">string</span></span>| <span data-ttu-id="0878f-148">Значение только для чтения, указывающее тип обнаружения, поддерживаемый приложением.</span><span class="sxs-lookup"><span data-stu-id="0878f-148">Read only value indicating what type of discovery the app supports.</span></span> <span data-ttu-id="0878f-149">Возможные значения: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="0878f-149">Possible values are: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="0878f-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0878f-150">JSON representation</span></span>

<span data-ttu-id="0878f-151">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0878f-151">The following is a JSON representation of the resource.</span></span>

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
