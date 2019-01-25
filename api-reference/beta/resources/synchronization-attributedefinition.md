---
title: Тип ресурса attributeDefinition
description: Описывает атрибут объекта.
localization_priority: Normal
ms.openlocfilehash: f9268bf61fec397c53744c9999635ba159b047f4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514343"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="51b6b-103">Тип ресурса attributeDefinition</span><span class="sxs-lookup"><span data-stu-id="51b6b-103">attributeDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51b6b-104">Описывает атрибут объекта.</span><span class="sxs-lookup"><span data-stu-id="51b6b-104">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="51b6b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="51b6b-105">Properties</span></span>

| <span data-ttu-id="51b6b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="51b6b-106">Property</span></span>      | <span data-ttu-id="51b6b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="51b6b-107">Type</span></span>      | <span data-ttu-id="51b6b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="51b6b-108">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="51b6b-109">Anchor</span><span class="sxs-lookup"><span data-stu-id="51b6b-109">anchor</span></span>         |<span data-ttu-id="51b6b-110">Логическое</span><span class="sxs-lookup"><span data-stu-id="51b6b-110">Boolean</span></span>    | <span data-ttu-id="51b6b-111">`true`Если атрибут должен использоваться для привязки для объекта.</span><span class="sxs-lookup"><span data-stu-id="51b6b-111">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="51b6b-112">Атрибуты привязки должны иметь уникальное значение, идентифицирующее объект и должны быть постоянным.</span><span class="sxs-lookup"><span data-stu-id="51b6b-112">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="51b6b-113">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="51b6b-113">Default is `false`.</span></span> <span data-ttu-id="51b6b-114">Один и только один из атрибутов объекта должен быть назначен для привязки для поддержки синхронизации.</span><span class="sxs-lookup"><span data-stu-id="51b6b-114">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="51b6b-115">caseExact</span><span class="sxs-lookup"><span data-stu-id="51b6b-115">caseExact</span></span>      |<span data-ttu-id="51b6b-116">Логическое</span><span class="sxs-lookup"><span data-stu-id="51b6b-116">Boolean</span></span>    |<span data-ttu-id="51b6b-117">`true`Если значение этого атрибута следует учитывать регистр.</span><span class="sxs-lookup"><span data-stu-id="51b6b-117">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="51b6b-118">Этот параметр влияет на как обработчик синхронизации обнаружены изменения в атрибуте.</span><span class="sxs-lookup"><span data-stu-id="51b6b-118">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="51b6b-119">Метаданные</span><span class="sxs-lookup"><span data-stu-id="51b6b-119">metadata</span></span>       |[<span data-ttu-id="51b6b-120">metadataEntry</span><span class="sxs-lookup"><span data-stu-id="51b6b-120">metadataEntry</span></span>](../resources/synchronization-metadataentry.md)    |<span data-ttu-id="51b6b-121">Расширение дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="51b6b-121">Additional extension properties.</span></span> <span data-ttu-id="51b6b-122">Если не указан явно, значения метаданных не должно изменяться.</span><span class="sxs-lookup"><span data-stu-id="51b6b-122">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="51b6b-123">многозначные</span><span class="sxs-lookup"><span data-stu-id="51b6b-123">multivalued</span></span>    |<span data-ttu-id="51b6b-124">Логическое</span><span class="sxs-lookup"><span data-stu-id="51b6b-124">Boolean</span></span>    |<span data-ttu-id="51b6b-125">`true`Если атрибут может содержать несколько значений.</span><span class="sxs-lookup"><span data-stu-id="51b6b-125">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="51b6b-126">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="51b6b-126">Default is `false`.</span></span>|
|<span data-ttu-id="51b6b-127">изменения</span><span class="sxs-lookup"><span data-stu-id="51b6b-127">mutability</span></span>     |<span data-ttu-id="51b6b-128">String</span><span class="sxs-lookup"><span data-stu-id="51b6b-128">String</span></span>     |<span data-ttu-id="51b6b-129">Изменения атрибута.</span><span class="sxs-lookup"><span data-stu-id="51b6b-129">An attribute's mutability.</span></span> <span data-ttu-id="51b6b-130">Возможные значения: `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span><span class="sxs-lookup"><span data-stu-id="51b6b-130">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="51b6b-131">Значение по умолчанию: `ReadWrite`.</span><span class="sxs-lookup"><span data-stu-id="51b6b-131">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="51b6b-132">name</span><span class="sxs-lookup"><span data-stu-id="51b6b-132">name</span></span>           |<span data-ttu-id="51b6b-133">String</span><span class="sxs-lookup"><span data-stu-id="51b6b-133">String</span></span>     |<span data-ttu-id="51b6b-134">Имя атрибута.</span><span class="sxs-lookup"><span data-stu-id="51b6b-134">Name of the attribute.</span></span> <span data-ttu-id="51b6b-135">Должно быть уникальным в рамках определения объекта.</span><span class="sxs-lookup"><span data-stu-id="51b6b-135">Must be unique within the object definition.</span></span> <span data-ttu-id="51b6b-136">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="51b6b-136">Not nullable.</span></span>|
|<span data-ttu-id="51b6b-137">Обязательный</span><span class="sxs-lookup"><span data-stu-id="51b6b-137">required</span></span>       |<span data-ttu-id="51b6b-138">Логическое</span><span class="sxs-lookup"><span data-stu-id="51b6b-138">Boolean</span></span>    |<span data-ttu-id="51b6b-139">`true`Если атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="51b6b-139">`true` if attribute is required.</span></span> <span data-ttu-id="51b6b-140">Объект не может быть создан, если какие-либо обязательные атрибуты отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="51b6b-140">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="51b6b-141">Если во время синхронизации, обязательный атрибут не имеет значения, будет использоваться значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="51b6b-141">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="51b6b-142">Если значение по умолчанию не задано, синхронизация будет записана ошибка.</span><span class="sxs-lookup"><span data-stu-id="51b6b-142">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="51b6b-143">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="51b6b-143">referencedObjects</span></span>|[<span data-ttu-id="51b6b-144">referencedObject</span><span class="sxs-lookup"><span data-stu-id="51b6b-144">referencedObject</span></span>](../resources/synchronization-referencedobject.md) |<span data-ttu-id="51b6b-145">Для атрибутов с `reference` введите объекты списков (например, `manager` атрибут будет содержать `User` как указанный объект).</span><span class="sxs-lookup"><span data-stu-id="51b6b-145">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="51b6b-146">type</span><span class="sxs-lookup"><span data-stu-id="51b6b-146">type</span></span>           |<span data-ttu-id="51b6b-147">String</span><span class="sxs-lookup"><span data-stu-id="51b6b-147">String</span></span>     |<span data-ttu-id="51b6b-148">Тип значения атрибута.</span><span class="sxs-lookup"><span data-stu-id="51b6b-148">Attribute value type.</span></span> <span data-ttu-id="51b6b-149">Возможные значения: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span><span class="sxs-lookup"><span data-stu-id="51b6b-149">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="51b6b-150">Значение по умолчанию: `String`.</span><span class="sxs-lookup"><span data-stu-id="51b6b-150">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="51b6b-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51b6b-151">JSON representation</span></span>

<span data-ttu-id="51b6b-152">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51b6b-152">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributedefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
