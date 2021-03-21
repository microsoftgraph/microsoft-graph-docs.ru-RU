---
title: тип ресурса attributeDefinition
description: Описывает атрибут объекта.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: a9c50721c1ee19505edc2507313cc346a6adabfd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956816"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="843cb-103">тип ресурса attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="843cb-103">attributeDefinition resource type</span></span>

<span data-ttu-id="843cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="843cb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="843cb-105">Описывает атрибут объекта.</span><span class="sxs-lookup"><span data-stu-id="843cb-105">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="843cb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="843cb-106">Properties</span></span>

| <span data-ttu-id="843cb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="843cb-107">Property</span></span>      | <span data-ttu-id="843cb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="843cb-108">Type</span></span>      | <span data-ttu-id="843cb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="843cb-109">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="843cb-110">якорь</span><span class="sxs-lookup"><span data-stu-id="843cb-110">anchor</span></span>         |<span data-ttu-id="843cb-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="843cb-111">Boolean</span></span>    | <span data-ttu-id="843cb-112">`true` если атрибут должен использоваться в качестве якоря для объекта.</span><span class="sxs-lookup"><span data-stu-id="843cb-112">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="843cb-113">Атрибуты Anchor должны иметь уникальное значение, определяющие объект, и должны быть неоменяемыми.</span><span class="sxs-lookup"><span data-stu-id="843cb-113">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="843cb-114">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="843cb-114">Default is `false`.</span></span> <span data-ttu-id="843cb-115">Один и только один атрибуты объекта должны быть назначены в качестве якоря для поддержки синхронизации.</span><span class="sxs-lookup"><span data-stu-id="843cb-115">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="843cb-116">caseExact</span><span class="sxs-lookup"><span data-stu-id="843cb-116">caseExact</span></span>      |<span data-ttu-id="843cb-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="843cb-117">Boolean</span></span>    |<span data-ttu-id="843cb-118">`true` если значение этого атрибута должно рассматриваться как чувствительное к делу.</span><span class="sxs-lookup"><span data-stu-id="843cb-118">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="843cb-119">Этот параметр влияет на то, как механизм синхронизации обнаруживает изменения атрибута.</span><span class="sxs-lookup"><span data-stu-id="843cb-119">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="843cb-120">flowNullValues</span><span class="sxs-lookup"><span data-stu-id="843cb-120">flowNullValues</span></span> |<span data-ttu-id="843cb-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="843cb-121">Boolean</span></span>    |<span data-ttu-id="843cb-122">"True", чтобы разрешить значения null для атрибутов.</span><span class="sxs-lookup"><span data-stu-id="843cb-122">'true' to allow null values for attributes.</span></span>|
|<span data-ttu-id="843cb-123">метаданные</span><span class="sxs-lookup"><span data-stu-id="843cb-123">metadata</span></span>       |<span data-ttu-id="843cb-124">[коллекция metadataEntry](../resources/synchronization-metadataentry.md)</span><span class="sxs-lookup"><span data-stu-id="843cb-124">[metadataEntry](../resources/synchronization-metadataentry.md) collection</span></span>   |<span data-ttu-id="843cb-125">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="843cb-125">Additional extension properties.</span></span> <span data-ttu-id="843cb-126">Если не упомянуть явно, значения метаданных не следует менять.</span><span class="sxs-lookup"><span data-stu-id="843cb-126">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="843cb-127">многооценная</span><span class="sxs-lookup"><span data-stu-id="843cb-127">multivalued</span></span>    |<span data-ttu-id="843cb-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="843cb-128">Boolean</span></span>    |<span data-ttu-id="843cb-129">`true` если атрибут может иметь несколько значений.</span><span class="sxs-lookup"><span data-stu-id="843cb-129">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="843cb-130">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="843cb-130">Default is `false`.</span></span>|
|<span data-ttu-id="843cb-131">мутируемость</span><span class="sxs-lookup"><span data-stu-id="843cb-131">mutability</span></span>     |<span data-ttu-id="843cb-132">мутируемость</span><span class="sxs-lookup"><span data-stu-id="843cb-132">mutability</span></span>     |<span data-ttu-id="843cb-133">Мутируемость атрибута.</span><span class="sxs-lookup"><span data-stu-id="843cb-133">An attribute's mutability.</span></span> <span data-ttu-id="843cb-134">Возможные значения:  `ReadWrite` `ReadOnly` , , `Immutable` `WriteOnly` .</span><span class="sxs-lookup"><span data-stu-id="843cb-134">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="843cb-135">Значение по умолчанию: `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="843cb-135">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="843cb-136">name</span><span class="sxs-lookup"><span data-stu-id="843cb-136">name</span></span>           |<span data-ttu-id="843cb-137">String</span><span class="sxs-lookup"><span data-stu-id="843cb-137">String</span></span>     |<span data-ttu-id="843cb-138">Имя атрибута.</span><span class="sxs-lookup"><span data-stu-id="843cb-138">Name of the attribute.</span></span> <span data-ttu-id="843cb-139">Должно быть уникальным в определении объекта.</span><span class="sxs-lookup"><span data-stu-id="843cb-139">Must be unique within the object definition.</span></span> <span data-ttu-id="843cb-140">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="843cb-140">Not nullable.</span></span>|
|<span data-ttu-id="843cb-141">Обязательный</span><span class="sxs-lookup"><span data-stu-id="843cb-141">required</span></span>       |<span data-ttu-id="843cb-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="843cb-142">Boolean</span></span>    |<span data-ttu-id="843cb-143">`true` если атрибут необходим.</span><span class="sxs-lookup"><span data-stu-id="843cb-143">`true` if attribute is required.</span></span> <span data-ttu-id="843cb-144">Объект не может быть создан, если отсутствуют какие-либо из необходимых атрибутов.</span><span class="sxs-lookup"><span data-stu-id="843cb-144">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="843cb-145">Если во время синхронизации необходимый атрибут не имеет значения, будет использоваться значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="843cb-145">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="843cb-146">Если по умолчанию значение не установлено, синхронизация зафиксировать ошибку.</span><span class="sxs-lookup"><span data-stu-id="843cb-146">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="843cb-147">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="843cb-147">referencedObjects</span></span>|<span data-ttu-id="843cb-148">[коллекция referencedObject](../resources/synchronization-referencedobject.md)</span><span class="sxs-lookup"><span data-stu-id="843cb-148">[referencedObject](../resources/synchronization-referencedobject.md) collection</span></span> |<span data-ttu-id="843cb-149">Для атрибутов с типом перечислены ссылки на объекты (например, атрибут будет `reference` `manager` перечисляться как `User` объект со ссылкой).</span><span class="sxs-lookup"><span data-stu-id="843cb-149">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="843cb-150">type</span><span class="sxs-lookup"><span data-stu-id="843cb-150">type</span></span>           |<span data-ttu-id="843cb-151">attributeType</span><span class="sxs-lookup"><span data-stu-id="843cb-151">attributeType</span></span>     |<span data-ttu-id="843cb-152">Тип значения атрибута.</span><span class="sxs-lookup"><span data-stu-id="843cb-152">Attribute value type.</span></span> <span data-ttu-id="843cb-153">Возможные значения: `String` `Integer` , , , `Reference` , `Binary` `Boolean` `DateTime` .</span><span class="sxs-lookup"><span data-stu-id="843cb-153">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`,`DateTime`.</span></span> <span data-ttu-id="843cb-154">Значение по умолчанию: `String`.</span><span class="sxs-lookup"><span data-stu-id="843cb-154">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="843cb-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="843cb-155">JSON representation</span></span>

<span data-ttu-id="843cb-156">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="843cb-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeDefinition"
}-->

```json
{
  "anchor": true,
  "caseExact": true,
  "defaultValue": "String",
  "flowNullValues": true,
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "multivalued": true,
  "mutability": "String",
  "name": "String",
  "referencedObjects": [{"@odata.type": "microsoft.graph.referencedObject"}],
  "required": true,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


