---
title: Тип ресурса Аттрибутедефинитион
description: Описывает атрибут объекта.
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a82fb5dcfd14f8c8fb09713a3a60c0f8c1e1f917
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384390"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="f418d-103">Тип ресурса Аттрибутедефинитион</span><span class="sxs-lookup"><span data-stu-id="f418d-103">attributeDefinition resource type</span></span>

<span data-ttu-id="f418d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f418d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f418d-105">Описывает атрибут объекта.</span><span class="sxs-lookup"><span data-stu-id="f418d-105">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="f418d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f418d-106">Properties</span></span>

| <span data-ttu-id="f418d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f418d-107">Property</span></span>      | <span data-ttu-id="f418d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f418d-108">Type</span></span>      | <span data-ttu-id="f418d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f418d-109">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="f418d-110">сами</span><span class="sxs-lookup"><span data-stu-id="f418d-110">anchor</span></span>         |<span data-ttu-id="f418d-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="f418d-111">Boolean</span></span>    | <span data-ttu-id="f418d-112">`true`значение, если атрибут должен использоваться в качестве привязки объекта.</span><span class="sxs-lookup"><span data-stu-id="f418d-112">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="f418d-113">Атрибуты привязки должны иметь уникальное значение, определяющее объект, и должны быть неизменными.</span><span class="sxs-lookup"><span data-stu-id="f418d-113">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="f418d-114">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="f418d-114">Default is `false`.</span></span> <span data-ttu-id="f418d-115">Только один из атрибутов объекта должен быть назначен в качестве привязки для поддержки синхронизации.</span><span class="sxs-lookup"><span data-stu-id="f418d-115">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="f418d-116">касиксакт</span><span class="sxs-lookup"><span data-stu-id="f418d-116">caseExact</span></span>      |<span data-ttu-id="f418d-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="f418d-117">Boolean</span></span>    |<span data-ttu-id="f418d-118">`true`Если значение этого атрибута должно обрабатываться с учетом регистра.</span><span class="sxs-lookup"><span data-stu-id="f418d-118">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="f418d-119">Этот параметр влияет на то, как обработчик синхронизации обнаруживает изменения атрибута.</span><span class="sxs-lookup"><span data-stu-id="f418d-119">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="f418d-120">фловнуллвалуес</span><span class="sxs-lookup"><span data-stu-id="f418d-120">flowNullValues</span></span> |<span data-ttu-id="f418d-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="f418d-121">Boolean</span></span>    |<span data-ttu-id="f418d-122">значение true, чтобы разрешить значения NULL для атрибутов.</span><span class="sxs-lookup"><span data-stu-id="f418d-122">'true' to allow null values for attributes.</span></span>|
|<span data-ttu-id="f418d-123">метаданных</span><span class="sxs-lookup"><span data-stu-id="f418d-123">metadata</span></span>       |<span data-ttu-id="f418d-124">Коллекция [метадатаентри](../resources/synchronization-metadataentry.md)</span><span class="sxs-lookup"><span data-stu-id="f418d-124">[metadataEntry](../resources/synchronization-metadataentry.md) collection</span></span>   |<span data-ttu-id="f418d-125">Дополнительные свойства расширения.</span><span class="sxs-lookup"><span data-stu-id="f418d-125">Additional extension properties.</span></span> <span data-ttu-id="f418d-126">Если явно не указано иное, значения метаданных не должны изменяться.</span><span class="sxs-lookup"><span data-stu-id="f418d-126">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="f418d-127">многозначных</span><span class="sxs-lookup"><span data-stu-id="f418d-127">multivalued</span></span>    |<span data-ttu-id="f418d-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="f418d-128">Boolean</span></span>    |<span data-ttu-id="f418d-129">`true`Если атрибут может иметь несколько значений.</span><span class="sxs-lookup"><span data-stu-id="f418d-129">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="f418d-130">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="f418d-130">Default is `false`.</span></span>|
|<span data-ttu-id="f418d-131">измен</span><span class="sxs-lookup"><span data-stu-id="f418d-131">mutability</span></span>     |<span data-ttu-id="f418d-132">String</span><span class="sxs-lookup"><span data-stu-id="f418d-132">String</span></span>     |<span data-ttu-id="f418d-133">Изменяемость атрибута.</span><span class="sxs-lookup"><span data-stu-id="f418d-133">An attribute's mutability.</span></span> <span data-ttu-id="f418d-134">Возможные значения: `ReadWrite` ,, `ReadOnly` `Immutable` , `WriteOnly` .</span><span class="sxs-lookup"><span data-stu-id="f418d-134">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="f418d-135">Значение по умолчанию: `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="f418d-135">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="f418d-136">name</span><span class="sxs-lookup"><span data-stu-id="f418d-136">name</span></span>           |<span data-ttu-id="f418d-137">String</span><span class="sxs-lookup"><span data-stu-id="f418d-137">String</span></span>     |<span data-ttu-id="f418d-138">Имя атрибута.</span><span class="sxs-lookup"><span data-stu-id="f418d-138">Name of the attribute.</span></span> <span data-ttu-id="f418d-139">Должно быть уникальным в пределах определения объекта.</span><span class="sxs-lookup"><span data-stu-id="f418d-139">Must be unique within the object definition.</span></span> <span data-ttu-id="f418d-140">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="f418d-140">Not nullable.</span></span>|
|<span data-ttu-id="f418d-141">Обязательный</span><span class="sxs-lookup"><span data-stu-id="f418d-141">required</span></span>       |<span data-ttu-id="f418d-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="f418d-142">Boolean</span></span>    |<span data-ttu-id="f418d-143">`true`Если атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="f418d-143">`true` if attribute is required.</span></span> <span data-ttu-id="f418d-144">Объект не может быть создан, если отсутствует необходимый атрибут.</span><span class="sxs-lookup"><span data-stu-id="f418d-144">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="f418d-145">Если во время синхронизации атрибуту required не присвоено значение, будет использоваться значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f418d-145">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="f418d-146">Если значение по умолчанию не задано, то при синхронизации будет записано сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="f418d-146">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="f418d-147">референцедобжектс</span><span class="sxs-lookup"><span data-stu-id="f418d-147">referencedObjects</span></span>|<span data-ttu-id="f418d-148">Коллекция [референцедобжект](../resources/synchronization-referencedobject.md)</span><span class="sxs-lookup"><span data-stu-id="f418d-148">[referencedObject](../resources/synchronization-referencedobject.md) collection</span></span> |<span data-ttu-id="f418d-149">Для атрибутов с `reference` типом перечисляет объекты, на которые имеются ссылки (например, `manager` атрибут будет `User` указан в качестве упоминаемого объекта).</span><span class="sxs-lookup"><span data-stu-id="f418d-149">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="f418d-150">type</span><span class="sxs-lookup"><span data-stu-id="f418d-150">type</span></span>           |<span data-ttu-id="f418d-151">String</span><span class="sxs-lookup"><span data-stu-id="f418d-151">String</span></span>     |<span data-ttu-id="f418d-152">Тип значения атрибута.</span><span class="sxs-lookup"><span data-stu-id="f418d-152">Attribute value type.</span></span> <span data-ttu-id="f418d-153">Возможные значения: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span><span class="sxs-lookup"><span data-stu-id="f418d-153">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="f418d-154">Значение по умолчанию: `String`.</span><span class="sxs-lookup"><span data-stu-id="f418d-154">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f418d-155">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f418d-155">JSON representation</span></span>

<span data-ttu-id="f418d-156">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f418d-156">The following is a JSON representation of the resource.</span></span>

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
