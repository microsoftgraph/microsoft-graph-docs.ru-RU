---
title: Тип ресурса attributeDefinition
description: Описывает атрибут объекта.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 34503f3edf15542db449d56e5211cd33b3d9132e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128815"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="f4faa-103">Тип ресурса attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="f4faa-103">attributeDefinition resource type</span></span>

<span data-ttu-id="f4faa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4faa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4faa-105">Описывает атрибут объекта.</span><span class="sxs-lookup"><span data-stu-id="f4faa-105">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="f4faa-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f4faa-106">Properties</span></span>

| <span data-ttu-id="f4faa-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f4faa-107">Property</span></span>      | <span data-ttu-id="f4faa-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f4faa-108">Type</span></span>      | <span data-ttu-id="f4faa-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f4faa-109">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="f4faa-110">anchor</span><span class="sxs-lookup"><span data-stu-id="f4faa-110">anchor</span></span>         |<span data-ttu-id="f4faa-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4faa-111">Boolean</span></span>    | <span data-ttu-id="f4faa-112">`true` если атрибут должен использоваться в качестве привязки для объекта.</span><span class="sxs-lookup"><span data-stu-id="f4faa-112">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="f4faa-113">Атрибуты привязки должны иметь уникальное значение, идентифицирующие объект, и должны быть неуменяемыми.</span><span class="sxs-lookup"><span data-stu-id="f4faa-113">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="f4faa-114">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="f4faa-114">Default is `false`.</span></span> <span data-ttu-id="f4faa-115">Один и только один атрибуты объекта должны быть назначены в качестве привязки для поддержки синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f4faa-115">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="f4faa-116">caseExact</span><span class="sxs-lookup"><span data-stu-id="f4faa-116">caseExact</span></span>      |<span data-ttu-id="f4faa-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4faa-117">Boolean</span></span>    |<span data-ttu-id="f4faa-118">`true` если значение этого атрибута должно рассматриваться как чувствительный к делу.</span><span class="sxs-lookup"><span data-stu-id="f4faa-118">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="f4faa-119">Этот параметр влияет на то, как механизм синхронизации обнаруживает изменения атрибута.</span><span class="sxs-lookup"><span data-stu-id="f4faa-119">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="f4faa-120">flowNullValues</span><span class="sxs-lookup"><span data-stu-id="f4faa-120">flowNullValues</span></span> |<span data-ttu-id="f4faa-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4faa-121">Boolean</span></span>    |<span data-ttu-id="f4faa-122">Значение true позволяет использовать значения null для атрибутов.</span><span class="sxs-lookup"><span data-stu-id="f4faa-122">'true' to allow null values for attributes.</span></span>|
|<span data-ttu-id="f4faa-123">метаданные</span><span class="sxs-lookup"><span data-stu-id="f4faa-123">metadata</span></span>       |<span data-ttu-id="f4faa-124">[Коллекция metadataEntry](../resources/synchronization-metadataentry.md)</span><span class="sxs-lookup"><span data-stu-id="f4faa-124">[metadataEntry](../resources/synchronization-metadataentry.md) collection</span></span>   |<span data-ttu-id="f4faa-125">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="f4faa-125">Additional extension properties.</span></span> <span data-ttu-id="f4faa-126">Если не было явно упомянуто, значения метаданных не следует менять.</span><span class="sxs-lookup"><span data-stu-id="f4faa-126">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="f4faa-127">multivalued</span><span class="sxs-lookup"><span data-stu-id="f4faa-127">multivalued</span></span>    |<span data-ttu-id="f4faa-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4faa-128">Boolean</span></span>    |<span data-ttu-id="f4faa-129">`true` если атрибут может иметь несколько значений.</span><span class="sxs-lookup"><span data-stu-id="f4faa-129">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="f4faa-130">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="f4faa-130">Default is `false`.</span></span>|
|<span data-ttu-id="f4faa-131">mutability</span><span class="sxs-lookup"><span data-stu-id="f4faa-131">mutability</span></span>     |<span data-ttu-id="f4faa-132">Строка</span><span class="sxs-lookup"><span data-stu-id="f4faa-132">String</span></span>     |<span data-ttu-id="f4faa-133">Мутируемость атрибута.</span><span class="sxs-lookup"><span data-stu-id="f4faa-133">An attribute's mutability.</span></span> <span data-ttu-id="f4faa-134">Возможные значения:  `ReadWrite` , , , `ReadOnly` `Immutable` `WriteOnly` .</span><span class="sxs-lookup"><span data-stu-id="f4faa-134">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="f4faa-135">Значение по умолчанию: `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="f4faa-135">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="f4faa-136">name</span><span class="sxs-lookup"><span data-stu-id="f4faa-136">name</span></span>           |<span data-ttu-id="f4faa-137">String</span><span class="sxs-lookup"><span data-stu-id="f4faa-137">String</span></span>     |<span data-ttu-id="f4faa-138">Имя атрибута.</span><span class="sxs-lookup"><span data-stu-id="f4faa-138">Name of the attribute.</span></span> <span data-ttu-id="f4faa-139">Должен быть уникальным в определении объекта.</span><span class="sxs-lookup"><span data-stu-id="f4faa-139">Must be unique within the object definition.</span></span> <span data-ttu-id="f4faa-140">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="f4faa-140">Not nullable.</span></span>|
|<span data-ttu-id="f4faa-141">Обязательный</span><span class="sxs-lookup"><span data-stu-id="f4faa-141">required</span></span>       |<span data-ttu-id="f4faa-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4faa-142">Boolean</span></span>    |<span data-ttu-id="f4faa-143">`true` если атрибут является требуемым.</span><span class="sxs-lookup"><span data-stu-id="f4faa-143">`true` if attribute is required.</span></span> <span data-ttu-id="f4faa-144">Объект не может быть создан, если отсутствуют какие-либо из необходимых атрибутов.</span><span class="sxs-lookup"><span data-stu-id="f4faa-144">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="f4faa-145">Если во время синхронизации необходимый атрибут не имеет значения, будет использоваться значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f4faa-145">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="f4faa-146">Если значение по умолчанию не установлено, при синхронизации будет записана ошибка.</span><span class="sxs-lookup"><span data-stu-id="f4faa-146">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="f4faa-147">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="f4faa-147">referencedObjects</span></span>|<span data-ttu-id="f4faa-148">[коллекция referencedObject](../resources/synchronization-referencedobject.md)</span><span class="sxs-lookup"><span data-stu-id="f4faa-148">[referencedObject](../resources/synchronization-referencedobject.md) collection</span></span> |<span data-ttu-id="f4faa-149">Для атрибутов с типом перечисляются объекты, на которые ссылается ссылка (например, атрибут будет перечислен как объект, на `reference` `manager` который `User` ссылается ссылка).</span><span class="sxs-lookup"><span data-stu-id="f4faa-149">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="f4faa-150">type</span><span class="sxs-lookup"><span data-stu-id="f4faa-150">type</span></span>           |<span data-ttu-id="f4faa-151">Строка</span><span class="sxs-lookup"><span data-stu-id="f4faa-151">String</span></span>     |<span data-ttu-id="f4faa-152">Тип значения атрибута.</span><span class="sxs-lookup"><span data-stu-id="f4faa-152">Attribute value type.</span></span> <span data-ttu-id="f4faa-153">Возможные значения: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span><span class="sxs-lookup"><span data-stu-id="f4faa-153">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="f4faa-154">Значение по умолчанию: `String`.</span><span class="sxs-lookup"><span data-stu-id="f4faa-154">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4faa-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f4faa-155">JSON representation</span></span>

<span data-ttu-id="f4faa-156">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f4faa-156">The following is a JSON representation of the resource.</span></span>

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


