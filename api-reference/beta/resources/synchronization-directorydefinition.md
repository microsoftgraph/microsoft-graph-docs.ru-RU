---
title: тип ресурса directoryDefinition
description: Предоставляет сведения о каталоге и его объектах в движке синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 8e3adb4679233fa35a53574b6f8d0c2b806be110
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956801"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="e137c-103">тип ресурса directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="e137c-103">directoryDefinition resource type</span></span>

<span data-ttu-id="e137c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e137c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e137c-105">Предоставляет сведения о каталоге и его объектах в движке синхронизации.</span><span class="sxs-lookup"><span data-stu-id="e137c-105">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="e137c-106">Этот ресурс сообщает механизму синхронизации, например, что в каталоге есть объекты с именем **пользователя** и **группы,** атрибуты которых поддерживаются для этих объектов, и типы для этих атрибутов.</span><span class="sxs-lookup"><span data-stu-id="e137c-106">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="e137c-107">Чтобы объект и атрибут участвовали [](synchronization-synchronizationrule.md) в правилах синхронизации и сопоставлениях [объектов,](synchronization-objectmapping.md)их необходимо определить как часть определения каталога.</span><span class="sxs-lookup"><span data-stu-id="e137c-107">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="e137c-108">Как правило, [](synchronization-synchronizationschema.md) схема синхронизации по умолчанию, [](synchronization-synchronizationtemplate.md) предоставляемая в рамках шаблона синхронизации, будет определять наиболее часто используемые объекты и атрибуты для этого каталога.</span><span class="sxs-lookup"><span data-stu-id="e137c-108">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="e137c-109">Однако если каталог поддерживает добавление настраиваемого атрибута, может потребоваться расширить определение по умолчанию с помощью собственных настраиваемых объектов или атрибутов.</span><span class="sxs-lookup"><span data-stu-id="e137c-109">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="e137c-110">Дополнительные сведения см. в [рублях Настройка](synchronization-configure-with-custom-target-attributes.md) синхронизации с пользовательскими атрибутами и настройка синхронизации с атрибутами [расширения каталогов.](synchronization-configure-with-directory-extension-attributes.md)</span><span class="sxs-lookup"><span data-stu-id="e137c-110">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="e137c-111">Определения каталогов обновляются в рамках схемы [синхронизации.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="e137c-111">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e137c-112">Методы</span><span class="sxs-lookup"><span data-stu-id="e137c-112">Methods</span></span>

| <span data-ttu-id="e137c-113">Метод</span><span class="sxs-lookup"><span data-stu-id="e137c-113">Method</span></span>       | <span data-ttu-id="e137c-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e137c-114">Return Type</span></span>  |<span data-ttu-id="e137c-115">Описание</span><span class="sxs-lookup"><span data-stu-id="e137c-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e137c-116">Обнаружение directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="e137c-116">Discover directoryDefinition</span></span>](../api/directorydefinition-discover.md) | [<span data-ttu-id="e137c-117">directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="e137c-117">directoryDefinition</span></span>](synchronization-directorydefinition.md) |<span data-ttu-id="e137c-118">Откройте схему и поддерживаемые свойства каталога.</span><span class="sxs-lookup"><span data-stu-id="e137c-118">Discover the schema and supported properties of the directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="e137c-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="e137c-119">Properties</span></span>

| <span data-ttu-id="e137c-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="e137c-120">Property</span></span>      | <span data-ttu-id="e137c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="e137c-121">Type</span></span>      | <span data-ttu-id="e137c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e137c-122">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="e137c-123">id</span><span class="sxs-lookup"><span data-stu-id="e137c-123">id</span></span>           |<span data-ttu-id="e137c-124">Строка</span><span class="sxs-lookup"><span data-stu-id="e137c-124">String</span></span>     |<span data-ttu-id="e137c-125">Идентификатор Directory.</span><span class="sxs-lookup"><span data-stu-id="e137c-125">Directory identifier.</span></span> <span data-ttu-id="e137c-126">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="e137c-126">Not nullable.</span></span>|
|<span data-ttu-id="e137c-127">метаданные</span><span class="sxs-lookup"><span data-stu-id="e137c-127">metadata</span></span>       |<span data-ttu-id="e137c-128">коллекция metadataEntry</span><span class="sxs-lookup"><span data-stu-id="e137c-128">metadataEntry collection</span></span>    |<span data-ttu-id="e137c-129">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="e137c-129">Additional extension properties.</span></span> <span data-ttu-id="e137c-130">Если не упомянуть явно, значения метаданных не следует менять.</span><span class="sxs-lookup"><span data-stu-id="e137c-130">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="e137c-131">name</span><span class="sxs-lookup"><span data-stu-id="e137c-131">name</span></span>           |<span data-ttu-id="e137c-132">String</span><span class="sxs-lookup"><span data-stu-id="e137c-132">String</span></span>     |<span data-ttu-id="e137c-133">Имя каталога.</span><span class="sxs-lookup"><span data-stu-id="e137c-133">Name of the directory.</span></span> <span data-ttu-id="e137c-134">Должна быть уникальной в [схеме синхронизации.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="e137c-134">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="e137c-135">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="e137c-135">Not nullable.</span></span>|
|<span data-ttu-id="e137c-136">объекты</span><span class="sxs-lookup"><span data-stu-id="e137c-136">objects</span></span>        |<span data-ttu-id="e137c-137">[коллекция objectDefinition](synchronization-objectdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="e137c-137">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="e137c-138">Коллекция объектов, поддерживаемых каталогом.</span><span class="sxs-lookup"><span data-stu-id="e137c-138">Collection of objects supported by the directory.</span></span>|
|<span data-ttu-id="e137c-139">version</span><span class="sxs-lookup"><span data-stu-id="e137c-139">version</span></span>|<span data-ttu-id="e137c-140">String</span><span class="sxs-lookup"><span data-stu-id="e137c-140">String</span></span>|<span data-ttu-id="e137c-141">Чтение только значения, которое указывает обнаруженную версию.</span><span class="sxs-lookup"><span data-stu-id="e137c-141">Read only value that indicates version discovered.</span></span> <span data-ttu-id="e137c-142">`null` если обнаружение еще не произошло.</span><span class="sxs-lookup"><span data-stu-id="e137c-142">`null` if discovery has not yet occurred.</span></span>|
|<span data-ttu-id="e137c-143">discoveryDateTime</span><span class="sxs-lookup"><span data-stu-id="e137c-143">discoveryDateTime</span></span>|<span data-ttu-id="e137c-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e137c-144">DateTimeOffset</span></span>| <span data-ttu-id="e137c-145">Представляет дату и время обнаружения с помощью формата ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="e137c-145">Represents the discovery date and time using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e137c-146">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="e137c-146">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="e137c-147">discoverabilities</span><span class="sxs-lookup"><span data-stu-id="e137c-147">discoverabilities</span></span>|<span data-ttu-id="e137c-148">directoryDefinitionDiscoverabilities</span><span class="sxs-lookup"><span data-stu-id="e137c-148">directoryDefinitionDiscoverabilities</span></span>| <span data-ttu-id="e137c-149">Прочитайте только значение, указывающее тип обнаружения, поддерживаемого приложением.</span><span class="sxs-lookup"><span data-stu-id="e137c-149">Read only value indicating what type of discovery the app supports.</span></span> <span data-ttu-id="e137c-150">Возможные значения: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e137c-150">Possible values are: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="e137c-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e137c-151">JSON representation</span></span>

<span data-ttu-id="e137c-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e137c-152">The following is a JSON representation of the resource.</span></span>

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


