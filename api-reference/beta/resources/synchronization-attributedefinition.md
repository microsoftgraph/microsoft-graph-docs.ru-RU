---
title: Тип ресурса Аттрибутедефинитион
description: Описывает атрибут объекта.
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9dd3bc69636f6717917979d94c58b4d030b58991
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520263"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="b862e-103">Тип ресурса Аттрибутедефинитион</span><span class="sxs-lookup"><span data-stu-id="b862e-103">attributeDefinition resource type</span></span>

<span data-ttu-id="b862e-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b862e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b862e-105">Описывает атрибут объекта.</span><span class="sxs-lookup"><span data-stu-id="b862e-105">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="b862e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b862e-106">Properties</span></span>

| <span data-ttu-id="b862e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b862e-107">Property</span></span>      | <span data-ttu-id="b862e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b862e-108">Type</span></span>      | <span data-ttu-id="b862e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b862e-109">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="b862e-110">сами</span><span class="sxs-lookup"><span data-stu-id="b862e-110">anchor</span></span>         |<span data-ttu-id="b862e-111">Логический</span><span class="sxs-lookup"><span data-stu-id="b862e-111">Boolean</span></span>    | <span data-ttu-id="b862e-112">`true`значение, если атрибут должен использоваться в качестве привязки объекта.</span><span class="sxs-lookup"><span data-stu-id="b862e-112">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="b862e-113">Атрибуты привязки должны иметь уникальное значение, определяющее объект, и должны быть неизменными.</span><span class="sxs-lookup"><span data-stu-id="b862e-113">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="b862e-114">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="b862e-114">Default is `false`.</span></span> <span data-ttu-id="b862e-115">Только один из атрибутов объекта должен быть назначен в качестве привязки для поддержки синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b862e-115">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="b862e-116">касиксакт</span><span class="sxs-lookup"><span data-stu-id="b862e-116">caseExact</span></span>      |<span data-ttu-id="b862e-117">Логический</span><span class="sxs-lookup"><span data-stu-id="b862e-117">Boolean</span></span>    |<span data-ttu-id="b862e-118">`true`Если значение этого атрибута должно обрабатываться с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="b862e-118">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="b862e-119">Этот параметр влияет на то, как обработчик синхронизации обнаруживает изменения атрибута.</span><span class="sxs-lookup"><span data-stu-id="b862e-119">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="b862e-120">метаданных</span><span class="sxs-lookup"><span data-stu-id="b862e-120">metadata</span></span>       |<span data-ttu-id="b862e-121">Коллекция [метадатаентри](../resources/synchronization-metadataentry.md)</span><span class="sxs-lookup"><span data-stu-id="b862e-121">[metadataEntry](../resources/synchronization-metadataentry.md) collection</span></span>   |<span data-ttu-id="b862e-122">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="b862e-122">Additional extension properties.</span></span> <span data-ttu-id="b862e-123">Если явно не указано иное, значения метаданных не должны изменяться.</span><span class="sxs-lookup"><span data-stu-id="b862e-123">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="b862e-124">многозначных</span><span class="sxs-lookup"><span data-stu-id="b862e-124">multivalued</span></span>    |<span data-ttu-id="b862e-125">Логический</span><span class="sxs-lookup"><span data-stu-id="b862e-125">Boolean</span></span>    |<span data-ttu-id="b862e-126">`true`Если атрибут может иметь несколько значений.</span><span class="sxs-lookup"><span data-stu-id="b862e-126">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="b862e-127">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="b862e-127">Default is `false`.</span></span>|
|<span data-ttu-id="b862e-128">измен</span><span class="sxs-lookup"><span data-stu-id="b862e-128">mutability</span></span>     |<span data-ttu-id="b862e-129">String</span><span class="sxs-lookup"><span data-stu-id="b862e-129">String</span></span>     |<span data-ttu-id="b862e-130">Изменяемость атрибута.</span><span class="sxs-lookup"><span data-stu-id="b862e-130">An attribute's mutability.</span></span> <span data-ttu-id="b862e-131">`ReadWrite`Возможные значения: `ReadOnly`,, `Immutable`,. `WriteOnly`</span><span class="sxs-lookup"><span data-stu-id="b862e-131">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="b862e-132">Значение по умолчанию: `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="b862e-132">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="b862e-133">name</span><span class="sxs-lookup"><span data-stu-id="b862e-133">name</span></span>           |<span data-ttu-id="b862e-134">String</span><span class="sxs-lookup"><span data-stu-id="b862e-134">String</span></span>     |<span data-ttu-id="b862e-135">Имя атрибута.</span><span class="sxs-lookup"><span data-stu-id="b862e-135">Name of the attribute.</span></span> <span data-ttu-id="b862e-136">Должно быть уникальным в пределах определения объекта.</span><span class="sxs-lookup"><span data-stu-id="b862e-136">Must be unique within the object definition.</span></span> <span data-ttu-id="b862e-137">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="b862e-137">Not nullable.</span></span>|
|<span data-ttu-id="b862e-138">Обязательный</span><span class="sxs-lookup"><span data-stu-id="b862e-138">required</span></span>       |<span data-ttu-id="b862e-139">Логический</span><span class="sxs-lookup"><span data-stu-id="b862e-139">Boolean</span></span>    |<span data-ttu-id="b862e-140">`true`Если атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="b862e-140">`true` if attribute is required.</span></span> <span data-ttu-id="b862e-141">Объект не может быть создан, если отсутствует необходимый атрибут.</span><span class="sxs-lookup"><span data-stu-id="b862e-141">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="b862e-142">Если во время синхронизации атрибуту required не присвоено значение, будет использоваться значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b862e-142">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="b862e-143">Если значение по умолчанию не задано, то при синхронизации будет записано сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="b862e-143">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="b862e-144">референцедобжектс</span><span class="sxs-lookup"><span data-stu-id="b862e-144">referencedObjects</span></span>|<span data-ttu-id="b862e-145">Коллекция [референцедобжект](../resources/synchronization-referencedobject.md)</span><span class="sxs-lookup"><span data-stu-id="b862e-145">[referencedObject](../resources/synchronization-referencedobject.md) collection</span></span> |<span data-ttu-id="b862e-146">Для атрибутов с `reference` типом перечисляет объекты, на которые имеются ссылки (например `manager` , атрибут будет `User` указан в качестве упоминаемого объекта).</span><span class="sxs-lookup"><span data-stu-id="b862e-146">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="b862e-147">type</span><span class="sxs-lookup"><span data-stu-id="b862e-147">type</span></span>           |<span data-ttu-id="b862e-148">String</span><span class="sxs-lookup"><span data-stu-id="b862e-148">String</span></span>     |<span data-ttu-id="b862e-149">Тип значения атрибута.</span><span class="sxs-lookup"><span data-stu-id="b862e-149">Attribute value type.</span></span> <span data-ttu-id="b862e-150">Возможные значения: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span><span class="sxs-lookup"><span data-stu-id="b862e-150">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="b862e-151">Значение по умолчанию: `String`.</span><span class="sxs-lookup"><span data-stu-id="b862e-151">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b862e-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b862e-152">JSON representation</span></span>

<span data-ttu-id="b862e-153">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b862e-153">The following is a JSON representation of the resource.</span></span>

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
