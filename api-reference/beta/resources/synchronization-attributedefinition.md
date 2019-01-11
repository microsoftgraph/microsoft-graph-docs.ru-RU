---
title: Тип ресурса attributeDefinition
description: Описывает атрибут объекта.
localization_priority: Normal
ms.openlocfilehash: 63b7f67808ab6695b30f5464d72aed2814e46c5a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829682"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="b35fe-103">Тип ресурса attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="b35fe-103">attributeDefinition resource type</span></span>

> <span data-ttu-id="b35fe-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b35fe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b35fe-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b35fe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b35fe-106">Описывает атрибут объекта.</span><span class="sxs-lookup"><span data-stu-id="b35fe-106">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="b35fe-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b35fe-107">Properties</span></span>

| <span data-ttu-id="b35fe-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b35fe-108">Property</span></span>      | <span data-ttu-id="b35fe-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b35fe-109">Type</span></span>      | <span data-ttu-id="b35fe-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b35fe-110">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="b35fe-111">привязки</span><span class="sxs-lookup"><span data-stu-id="b35fe-111">anchor</span></span>         |<span data-ttu-id="b35fe-112">Логический</span><span class="sxs-lookup"><span data-stu-id="b35fe-112">Boolean</span></span>    | <span data-ttu-id="b35fe-113">`true`Если атрибут должен использоваться для привязки для объекта.</span><span class="sxs-lookup"><span data-stu-id="b35fe-113">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="b35fe-114">Атрибуты привязки должны иметь уникальное значение, идентифицирующее объект и должны быть постоянным.</span><span class="sxs-lookup"><span data-stu-id="b35fe-114">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="b35fe-115">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="b35fe-115">Default is `false`.</span></span> <span data-ttu-id="b35fe-116">Один и только один из атрибутов объекта должен быть назначен для привязки для поддержки синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b35fe-116">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="b35fe-117">caseExact</span><span class="sxs-lookup"><span data-stu-id="b35fe-117">caseExact</span></span>      |<span data-ttu-id="b35fe-118">Логический</span><span class="sxs-lookup"><span data-stu-id="b35fe-118">Boolean</span></span>    |<span data-ttu-id="b35fe-119">`true`Если значение этого атрибута следует учитывать регистр.</span><span class="sxs-lookup"><span data-stu-id="b35fe-119">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="b35fe-120">Этот параметр влияет на как обработчик синхронизации обнаружены изменения в атрибуте.</span><span class="sxs-lookup"><span data-stu-id="b35fe-120">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="b35fe-121">метаданные</span><span class="sxs-lookup"><span data-stu-id="b35fe-121">metadata</span></span>       |[<span data-ttu-id="b35fe-122">metadataEntry</span><span class="sxs-lookup"><span data-stu-id="b35fe-122">metadataEntry</span></span>](../resources/synchronization-metadataentry.md)    |<span data-ttu-id="b35fe-123">Расширение дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="b35fe-123">Additional extension properties.</span></span> <span data-ttu-id="b35fe-124">Если не указан явно, значения метаданных не должно изменяться.</span><span class="sxs-lookup"><span data-stu-id="b35fe-124">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="b35fe-125">многозначные</span><span class="sxs-lookup"><span data-stu-id="b35fe-125">multivalued</span></span>    |<span data-ttu-id="b35fe-126">Логический</span><span class="sxs-lookup"><span data-stu-id="b35fe-126">Boolean</span></span>    |<span data-ttu-id="b35fe-127">`true`Если атрибут может содержать несколько значений.</span><span class="sxs-lookup"><span data-stu-id="b35fe-127">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="b35fe-128">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="b35fe-128">Default is `false`.</span></span>|
|<span data-ttu-id="b35fe-129">изменения</span><span class="sxs-lookup"><span data-stu-id="b35fe-129">mutability</span></span>     |<span data-ttu-id="b35fe-130">Строка</span><span class="sxs-lookup"><span data-stu-id="b35fe-130">String</span></span>     |<span data-ttu-id="b35fe-131">Изменения атрибута.</span><span class="sxs-lookup"><span data-stu-id="b35fe-131">An attribute's mutability.</span></span> <span data-ttu-id="b35fe-132">Возможные значения: `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span><span class="sxs-lookup"><span data-stu-id="b35fe-132">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="b35fe-133">Значение по умолчанию: `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="b35fe-133">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="b35fe-134">name</span><span class="sxs-lookup"><span data-stu-id="b35fe-134">name</span></span>           |<span data-ttu-id="b35fe-135">Строка</span><span class="sxs-lookup"><span data-stu-id="b35fe-135">String</span></span>     |<span data-ttu-id="b35fe-136">Имя атрибута.</span><span class="sxs-lookup"><span data-stu-id="b35fe-136">Name of the attribute.</span></span> <span data-ttu-id="b35fe-137">Должно быть уникальным в рамках определения объекта.</span><span class="sxs-lookup"><span data-stu-id="b35fe-137">Must be unique within the object definition.</span></span> <span data-ttu-id="b35fe-138">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="b35fe-138">Not nullable.</span></span>|
|<span data-ttu-id="b35fe-139">Обязательный</span><span class="sxs-lookup"><span data-stu-id="b35fe-139">required</span></span>       |<span data-ttu-id="b35fe-140">Логический</span><span class="sxs-lookup"><span data-stu-id="b35fe-140">Boolean</span></span>    |<span data-ttu-id="b35fe-141">`true`Если атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="b35fe-141">`true` if attribute is required.</span></span> <span data-ttu-id="b35fe-142">Объект не может быть создан, если какие-либо обязательные атрибуты отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b35fe-142">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="b35fe-143">Если во время синхронизации, обязательный атрибут не имеет значения, будет использоваться значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b35fe-143">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="b35fe-144">Если значение по умолчанию не задано, синхронизация будет записана ошибка.</span><span class="sxs-lookup"><span data-stu-id="b35fe-144">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="b35fe-145">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="b35fe-145">referencedObjects</span></span>|[<span data-ttu-id="b35fe-146">referencedObject</span><span class="sxs-lookup"><span data-stu-id="b35fe-146">referencedObject</span></span>](../resources/synchronization-referencedobject.md) |<span data-ttu-id="b35fe-147">Для атрибутов с `reference` введите объекты списков (например, `manager` атрибут будет содержать `User` как указанный объект).</span><span class="sxs-lookup"><span data-stu-id="b35fe-147">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="b35fe-148">type</span><span class="sxs-lookup"><span data-stu-id="b35fe-148">type</span></span>           |<span data-ttu-id="b35fe-149">Строка</span><span class="sxs-lookup"><span data-stu-id="b35fe-149">String</span></span>     |<span data-ttu-id="b35fe-150">Тип значения атрибута.</span><span class="sxs-lookup"><span data-stu-id="b35fe-150">Attribute value type.</span></span> <span data-ttu-id="b35fe-151">Возможные значения: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span><span class="sxs-lookup"><span data-stu-id="b35fe-151">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="b35fe-152">Значение по умолчанию: `String`.</span><span class="sxs-lookup"><span data-stu-id="b35fe-152">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b35fe-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b35fe-153">JSON representation</span></span>

<span data-ttu-id="b35fe-154">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b35fe-154">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
