---
title: тип ресурса directoryDefinition
description: Предоставляет сведения о каталоге и его объектах в движке синхронизации.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: cb0eb46feebb743a30593bf6e1d2b0142077cc7e
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718459"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="74d86-103">тип ресурса directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="74d86-103">directoryDefinition resource type</span></span>

<span data-ttu-id="74d86-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74d86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="74d86-105">Предоставляет сведения о каталоге и его объектах в движке синхронизации.</span><span class="sxs-lookup"><span data-stu-id="74d86-105">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="74d86-106">Этот ресурс сообщает механизму синхронизации, например, что в каталоге есть объекты с именем **пользователя** и **группы,** атрибуты которых поддерживаются для этих объектов, и типы для этих атрибутов.</span><span class="sxs-lookup"><span data-stu-id="74d86-106">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="74d86-107">Чтобы объект и атрибут участвовали [](synchronization-synchronizationrule.md) в правилах синхронизации и сопоставлениях [объектов,](synchronization-objectmapping.md)их необходимо определить как часть определения каталога.</span><span class="sxs-lookup"><span data-stu-id="74d86-107">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="74d86-108">Как правило, [](synchronization-synchronizationschema.md) схема синхронизации по умолчанию, [](synchronization-synchronizationtemplate.md) предоставляемая в рамках шаблона синхронизации, будет определять наиболее часто используемые объекты и атрибуты для этого каталога.</span><span class="sxs-lookup"><span data-stu-id="74d86-108">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="74d86-109">Однако если каталог поддерживает добавление настраиваемого атрибута, может потребоваться расширить определение по умолчанию с помощью собственных настраиваемых объектов или атрибутов.</span><span class="sxs-lookup"><span data-stu-id="74d86-109">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="74d86-110">Дополнительные сведения см. в [рублях Настройка](synchronization-configure-with-custom-target-attributes.md) синхронизации с пользовательскими атрибутами и настройка синхронизации с атрибутами [расширения каталогов.](synchronization-configure-with-directory-extension-attributes.md)</span><span class="sxs-lookup"><span data-stu-id="74d86-110">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="74d86-111">Определения каталогов обновляются в рамках схемы [синхронизации.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="74d86-111">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="74d86-112">Методы</span><span class="sxs-lookup"><span data-stu-id="74d86-112">Methods</span></span>

| <span data-ttu-id="74d86-113">Метод</span><span class="sxs-lookup"><span data-stu-id="74d86-113">Method</span></span>       | <span data-ttu-id="74d86-114">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="74d86-114">Return Type</span></span>  |<span data-ttu-id="74d86-115">Описание</span><span class="sxs-lookup"><span data-stu-id="74d86-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="74d86-116">Обнаружение directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="74d86-116">Discover directoryDefinition</span></span>](../api/directorydefinition-discover.md) | [<span data-ttu-id="74d86-117">directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="74d86-117">directoryDefinition</span></span>](synchronization-directorydefinition.md) |<span data-ttu-id="74d86-118">Откройте схему и поддерживаемые свойства каталога.</span><span class="sxs-lookup"><span data-stu-id="74d86-118">Discover the schema and supported properties of the directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="74d86-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="74d86-119">Properties</span></span>

| <span data-ttu-id="74d86-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="74d86-120">Property</span></span>      | <span data-ttu-id="74d86-121">Тип</span><span class="sxs-lookup"><span data-stu-id="74d86-121">Type</span></span>      | <span data-ttu-id="74d86-122">Описание</span><span class="sxs-lookup"><span data-stu-id="74d86-122">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="74d86-123">id</span><span class="sxs-lookup"><span data-stu-id="74d86-123">id</span></span>           |<span data-ttu-id="74d86-124">String</span><span class="sxs-lookup"><span data-stu-id="74d86-124">String</span></span>     |<span data-ttu-id="74d86-125">Идентификатор Directory.</span><span class="sxs-lookup"><span data-stu-id="74d86-125">Directory identifier.</span></span> <span data-ttu-id="74d86-126">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="74d86-126">Not nullable.</span></span>|
|<span data-ttu-id="74d86-127">метаданные</span><span class="sxs-lookup"><span data-stu-id="74d86-127">metadata</span></span>       |<span data-ttu-id="74d86-128">коллекция metadataEntry</span><span class="sxs-lookup"><span data-stu-id="74d86-128">metadataEntry collection</span></span>    |<span data-ttu-id="74d86-129">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="74d86-129">Additional extension properties.</span></span> <span data-ttu-id="74d86-130">Если не упомянуть явно, значения метаданных не следует менять.</span><span class="sxs-lookup"><span data-stu-id="74d86-130">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="74d86-131">name</span><span class="sxs-lookup"><span data-stu-id="74d86-131">name</span></span>           |<span data-ttu-id="74d86-132">String</span><span class="sxs-lookup"><span data-stu-id="74d86-132">String</span></span>     |<span data-ttu-id="74d86-133">Имя каталога.</span><span class="sxs-lookup"><span data-stu-id="74d86-133">Name of the directory.</span></span> <span data-ttu-id="74d86-134">Должна быть уникальной в [схеме синхронизации.](synchronization-synchronizationschema.md)</span><span class="sxs-lookup"><span data-stu-id="74d86-134">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="74d86-135">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="74d86-135">Not nullable.</span></span>|
|<span data-ttu-id="74d86-136">объекты</span><span class="sxs-lookup"><span data-stu-id="74d86-136">objects</span></span>        |<span data-ttu-id="74d86-137">[коллекция objectDefinition](synchronization-objectdefinition.md)</span><span class="sxs-lookup"><span data-stu-id="74d86-137">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="74d86-138">Коллекция объектов, поддерживаемых каталогом.</span><span class="sxs-lookup"><span data-stu-id="74d86-138">Collection of objects supported by the directory.</span></span>|
|<span data-ttu-id="74d86-139">version</span><span class="sxs-lookup"><span data-stu-id="74d86-139">version</span></span>|<span data-ttu-id="74d86-140">String</span><span class="sxs-lookup"><span data-stu-id="74d86-140">String</span></span>|<span data-ttu-id="74d86-141">Чтение только значения, которое указывает обнаруженную версию.</span><span class="sxs-lookup"><span data-stu-id="74d86-141">Read only value that indicates version discovered.</span></span> <span data-ttu-id="74d86-142">Null, если обнаружение еще не произошло.</span><span class="sxs-lookup"><span data-stu-id="74d86-142">Null if discovery has not yet occurred.</span></span>|
|<span data-ttu-id="74d86-143">discoveryDateTime</span><span class="sxs-lookup"><span data-stu-id="74d86-143">discoveryDateTime</span></span>|<span data-ttu-id="74d86-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74d86-144">DateTimeOffset</span></span>| <span data-ttu-id="74d86-145">Представляет дату и время обнаружения с помощью формата ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="74d86-145">Represents the discovery date and time using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="74d86-146">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="74d86-146">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="74d86-147">discoverabilities</span><span class="sxs-lookup"><span data-stu-id="74d86-147">discoverabilities</span></span>|<span data-ttu-id="74d86-148">Строка</span><span class="sxs-lookup"><span data-stu-id="74d86-148">string</span></span>| <span data-ttu-id="74d86-149">Прочитайте только значение, указывающее тип обнаружения, поддерживаемого приложением.</span><span class="sxs-lookup"><span data-stu-id="74d86-149">Read only value indicating what type of discovery the app supports.</span></span> <span data-ttu-id="74d86-150">Возможные значения: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="74d86-150">Possible values are: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="74d86-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="74d86-151">JSON representation</span></span>

<span data-ttu-id="74d86-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="74d86-152">The following is a JSON representation of the resource.</span></span>

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


