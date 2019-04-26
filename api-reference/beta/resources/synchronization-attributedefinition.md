---
title: Тип ресурса Аттрибутедефинитион
description: Описывает атрибут объекта.
localization_priority: Normal
ms.openlocfilehash: 04ee5ffb6cda3cc48f89a722caab3a4e46500379
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345647"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="631f7-103">Тип ресурса Аттрибутедефинитион</span><span class="sxs-lookup"><span data-stu-id="631f7-103">attributeDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="631f7-104">Описывает атрибут объекта.</span><span class="sxs-lookup"><span data-stu-id="631f7-104">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="631f7-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="631f7-105">Properties</span></span>

| <span data-ttu-id="631f7-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="631f7-106">Property</span></span>      | <span data-ttu-id="631f7-107">Тип</span><span class="sxs-lookup"><span data-stu-id="631f7-107">Type</span></span>      | <span data-ttu-id="631f7-108">Описание</span><span class="sxs-lookup"><span data-stu-id="631f7-108">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="631f7-109">сами</span><span class="sxs-lookup"><span data-stu-id="631f7-109">anchor</span></span>         |<span data-ttu-id="631f7-110">Логический</span><span class="sxs-lookup"><span data-stu-id="631f7-110">Boolean</span></span>    | <span data-ttu-id="631f7-111">`true`значение, если атрибут должен использоваться в качестве привязки объекта.</span><span class="sxs-lookup"><span data-stu-id="631f7-111">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="631f7-112">Атрибуты привязки должны иметь уникальное значение, определяющее объект, и должны быть неизменными.</span><span class="sxs-lookup"><span data-stu-id="631f7-112">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="631f7-113">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="631f7-113">Default is `false`.</span></span> <span data-ttu-id="631f7-114">Только один из атрибутов объекта должен быть назначен в качестве привязки для поддержки синхронизации.</span><span class="sxs-lookup"><span data-stu-id="631f7-114">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="631f7-115">Касиксакт</span><span class="sxs-lookup"><span data-stu-id="631f7-115">caseExact</span></span>      |<span data-ttu-id="631f7-116">Логический</span><span class="sxs-lookup"><span data-stu-id="631f7-116">Boolean</span></span>    |<span data-ttu-id="631f7-117">`true`Если значение этого атрибута должно обрабатываться с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="631f7-117">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="631f7-118">Этот параметр влияет на то, как обработчик синхронизации обнаруживает изменения атрибута.</span><span class="sxs-lookup"><span data-stu-id="631f7-118">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="631f7-119">метаданных</span><span class="sxs-lookup"><span data-stu-id="631f7-119">metadata</span></span>       |<span data-ttu-id="631f7-120">Коллекция [метадатаентри](../resources/synchronization-metadataentry.md)</span><span class="sxs-lookup"><span data-stu-id="631f7-120">[metadataEntry](../resources/synchronization-metadataentry.md) collection</span></span>   |<span data-ttu-id="631f7-121">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="631f7-121">Additional extension properties.</span></span> <span data-ttu-id="631f7-122">Если явно не указано иное, значения метаданных не должны изменяться.</span><span class="sxs-lookup"><span data-stu-id="631f7-122">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="631f7-123">многозначных</span><span class="sxs-lookup"><span data-stu-id="631f7-123">multivalued</span></span>    |<span data-ttu-id="631f7-124">Логический</span><span class="sxs-lookup"><span data-stu-id="631f7-124">Boolean</span></span>    |<span data-ttu-id="631f7-125">`true`Если атрибут может иметь несколько значений.</span><span class="sxs-lookup"><span data-stu-id="631f7-125">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="631f7-126">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="631f7-126">Default is `false`.</span></span>|
|<span data-ttu-id="631f7-127">измен</span><span class="sxs-lookup"><span data-stu-id="631f7-127">mutability</span></span>     |<span data-ttu-id="631f7-128">String</span><span class="sxs-lookup"><span data-stu-id="631f7-128">String</span></span>     |<span data-ttu-id="631f7-129">Изменяемость атрибута.</span><span class="sxs-lookup"><span data-stu-id="631f7-129">An attribute's mutability.</span></span> <span data-ttu-id="631f7-130">`ReadWrite`Возможные значения: `ReadOnly`,, `Immutable`,. `WriteOnly`</span><span class="sxs-lookup"><span data-stu-id="631f7-130">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="631f7-131">Значение по умолчанию: `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="631f7-131">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="631f7-132">name</span><span class="sxs-lookup"><span data-stu-id="631f7-132">name</span></span>           |<span data-ttu-id="631f7-133">String</span><span class="sxs-lookup"><span data-stu-id="631f7-133">String</span></span>     |<span data-ttu-id="631f7-134">Имя атрибута.</span><span class="sxs-lookup"><span data-stu-id="631f7-134">Name of the attribute.</span></span> <span data-ttu-id="631f7-135">Должно быть уникальным в пределах определения объекта.</span><span class="sxs-lookup"><span data-stu-id="631f7-135">Must be unique within the object definition.</span></span> <span data-ttu-id="631f7-136">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="631f7-136">Not nullable.</span></span>|
|<span data-ttu-id="631f7-137">Обязательный</span><span class="sxs-lookup"><span data-stu-id="631f7-137">required</span></span>       |<span data-ttu-id="631f7-138">Логический</span><span class="sxs-lookup"><span data-stu-id="631f7-138">Boolean</span></span>    |<span data-ttu-id="631f7-139">`true`Если атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="631f7-139">`true` if attribute is required.</span></span> <span data-ttu-id="631f7-140">Объект не может быть создан, если отсутствует необходимый атрибут.</span><span class="sxs-lookup"><span data-stu-id="631f7-140">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="631f7-141">Если во время синхронизации атрибуту required не присвоено значение, будет использоваться значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="631f7-141">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="631f7-142">Если значение по умолчанию не задано, то при синхронизации будет записано сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="631f7-142">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="631f7-143">Референцедобжектс</span><span class="sxs-lookup"><span data-stu-id="631f7-143">referencedObjects</span></span>|<span data-ttu-id="631f7-144">Коллекция [референцедобжект](../resources/synchronization-referencedobject.md)</span><span class="sxs-lookup"><span data-stu-id="631f7-144">[referencedObject](../resources/synchronization-referencedobject.md) collection</span></span> |<span data-ttu-id="631f7-145">Для атрибутов с `reference` типом перечисляет объекты, на которые имеются ссылки (например `manager` , атрибут будет `User` указан в качестве упоминаемого объекта).</span><span class="sxs-lookup"><span data-stu-id="631f7-145">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="631f7-146">type</span><span class="sxs-lookup"><span data-stu-id="631f7-146">type</span></span>           |<span data-ttu-id="631f7-147">String</span><span class="sxs-lookup"><span data-stu-id="631f7-147">String</span></span>     |<span data-ttu-id="631f7-148">Тип значения атрибута.</span><span class="sxs-lookup"><span data-stu-id="631f7-148">Attribute value type.</span></span> <span data-ttu-id="631f7-149">Возможные значения: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span><span class="sxs-lookup"><span data-stu-id="631f7-149">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="631f7-150">Значение по умолчанию: `String`.</span><span class="sxs-lookup"><span data-stu-id="631f7-150">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="631f7-151">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="631f7-151">JSON representation</span></span>

<span data-ttu-id="631f7-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="631f7-152">The following is a JSON representation of the resource.</span></span>

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
