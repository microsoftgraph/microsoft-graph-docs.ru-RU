---
title: Тип ресурса Аттрибутедефинитион
description: Описывает атрибут объекта.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4d8a911b7f6ab3b916515eb73d53bfaf489047e0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078103"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="778a2-103">Тип ресурса Аттрибутедефинитион</span><span class="sxs-lookup"><span data-stu-id="778a2-103">attributeDefinition resource type</span></span>

<span data-ttu-id="778a2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="778a2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="778a2-105">Описывает атрибут объекта.</span><span class="sxs-lookup"><span data-stu-id="778a2-105">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="778a2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="778a2-106">Properties</span></span>

| <span data-ttu-id="778a2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="778a2-107">Property</span></span>      | <span data-ttu-id="778a2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="778a2-108">Type</span></span>      | <span data-ttu-id="778a2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="778a2-109">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="778a2-110">сами</span><span class="sxs-lookup"><span data-stu-id="778a2-110">anchor</span></span>         |<span data-ttu-id="778a2-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="778a2-111">Boolean</span></span>    | <span data-ttu-id="778a2-112">`true` значение, если атрибут должен использоваться в качестве привязки объекта.</span><span class="sxs-lookup"><span data-stu-id="778a2-112">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="778a2-113">Атрибуты привязки должны иметь уникальное значение, определяющее объект, и должны быть неизменными.</span><span class="sxs-lookup"><span data-stu-id="778a2-113">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="778a2-114">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="778a2-114">Default is `false`.</span></span> <span data-ttu-id="778a2-115">Только один из атрибутов объекта должен быть назначен в качестве привязки для поддержки синхронизации.</span><span class="sxs-lookup"><span data-stu-id="778a2-115">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="778a2-116">касиксакт</span><span class="sxs-lookup"><span data-stu-id="778a2-116">caseExact</span></span>      |<span data-ttu-id="778a2-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="778a2-117">Boolean</span></span>    |<span data-ttu-id="778a2-118">`true` Если значение этого атрибута должно обрабатываться с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="778a2-118">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="778a2-119">Этот параметр влияет на то, как обработчик синхронизации обнаруживает изменения атрибута.</span><span class="sxs-lookup"><span data-stu-id="778a2-119">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="778a2-120">фловнуллвалуес</span><span class="sxs-lookup"><span data-stu-id="778a2-120">flowNullValues</span></span> |<span data-ttu-id="778a2-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="778a2-121">Boolean</span></span>    |<span data-ttu-id="778a2-122">значение true, чтобы разрешить значения NULL для атрибутов.</span><span class="sxs-lookup"><span data-stu-id="778a2-122">'true' to allow null values for attributes.</span></span>|
|<span data-ttu-id="778a2-123">метаданных</span><span class="sxs-lookup"><span data-stu-id="778a2-123">metadata</span></span>       |<span data-ttu-id="778a2-124">Коллекция [метадатаентри](../resources/synchronization-metadataentry.md)</span><span class="sxs-lookup"><span data-stu-id="778a2-124">[metadataEntry](../resources/synchronization-metadataentry.md) collection</span></span>   |<span data-ttu-id="778a2-125">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="778a2-125">Additional extension properties.</span></span> <span data-ttu-id="778a2-126">Если явно не указано иное, значения метаданных не должны изменяться.</span><span class="sxs-lookup"><span data-stu-id="778a2-126">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="778a2-127">многозначных</span><span class="sxs-lookup"><span data-stu-id="778a2-127">multivalued</span></span>    |<span data-ttu-id="778a2-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="778a2-128">Boolean</span></span>    |<span data-ttu-id="778a2-129">`true` Если атрибут может иметь несколько значений.</span><span class="sxs-lookup"><span data-stu-id="778a2-129">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="778a2-130">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="778a2-130">Default is `false`.</span></span>|
|<span data-ttu-id="778a2-131">измен</span><span class="sxs-lookup"><span data-stu-id="778a2-131">mutability</span></span>     |<span data-ttu-id="778a2-132">String</span><span class="sxs-lookup"><span data-stu-id="778a2-132">String</span></span>     |<span data-ttu-id="778a2-133">Изменяемость атрибута.</span><span class="sxs-lookup"><span data-stu-id="778a2-133">An attribute's mutability.</span></span> <span data-ttu-id="778a2-134">Возможные значения:  `ReadWrite` ,, `ReadOnly` `Immutable` , `WriteOnly` .</span><span class="sxs-lookup"><span data-stu-id="778a2-134">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="778a2-135">Значение по умолчанию: `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="778a2-135">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="778a2-136">name</span><span class="sxs-lookup"><span data-stu-id="778a2-136">name</span></span>           |<span data-ttu-id="778a2-137">String</span><span class="sxs-lookup"><span data-stu-id="778a2-137">String</span></span>     |<span data-ttu-id="778a2-138">Имя атрибута.</span><span class="sxs-lookup"><span data-stu-id="778a2-138">Name of the attribute.</span></span> <span data-ttu-id="778a2-139">Должно быть уникальным в пределах определения объекта.</span><span class="sxs-lookup"><span data-stu-id="778a2-139">Must be unique within the object definition.</span></span> <span data-ttu-id="778a2-140">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="778a2-140">Not nullable.</span></span>|
|<span data-ttu-id="778a2-141">Обязательный</span><span class="sxs-lookup"><span data-stu-id="778a2-141">required</span></span>       |<span data-ttu-id="778a2-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="778a2-142">Boolean</span></span>    |<span data-ttu-id="778a2-143">`true` Если атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="778a2-143">`true` if attribute is required.</span></span> <span data-ttu-id="778a2-144">Объект не может быть создан, если отсутствует необходимый атрибут.</span><span class="sxs-lookup"><span data-stu-id="778a2-144">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="778a2-145">Если во время синхронизации атрибуту required не присвоено значение, будет использоваться значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="778a2-145">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="778a2-146">Если значение по умолчанию не задано, то при синхронизации будет записано сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="778a2-146">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="778a2-147">референцедобжектс</span><span class="sxs-lookup"><span data-stu-id="778a2-147">referencedObjects</span></span>|<span data-ttu-id="778a2-148">Коллекция [референцедобжект](../resources/synchronization-referencedobject.md)</span><span class="sxs-lookup"><span data-stu-id="778a2-148">[referencedObject](../resources/synchronization-referencedobject.md) collection</span></span> |<span data-ttu-id="778a2-149">Для атрибутов с `reference` типом перечисляет объекты, на которые имеются ссылки (например, `manager` атрибут будет `User` указан в качестве упоминаемого объекта).</span><span class="sxs-lookup"><span data-stu-id="778a2-149">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="778a2-150">type</span><span class="sxs-lookup"><span data-stu-id="778a2-150">type</span></span>           |<span data-ttu-id="778a2-151">String</span><span class="sxs-lookup"><span data-stu-id="778a2-151">String</span></span>     |<span data-ttu-id="778a2-152">Тип значения атрибута.</span><span class="sxs-lookup"><span data-stu-id="778a2-152">Attribute value type.</span></span> <span data-ttu-id="778a2-153">Возможные значения: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span><span class="sxs-lookup"><span data-stu-id="778a2-153">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="778a2-154">Значение по умолчанию: `String`.</span><span class="sxs-lookup"><span data-stu-id="778a2-154">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="778a2-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="778a2-155">JSON representation</span></span>

<span data-ttu-id="778a2-156">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="778a2-156">The following is a JSON representation of the resource.</span></span>

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


