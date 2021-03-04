---
title: Тип ресурса тегов
description: Представляет тег eDiscovery, который используется для маркировки документов во время проверки для отдельного отзывчивого и не отзывчивого контента.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: dee53c5a7d8320822101addcf5764420456e703f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447551"
---
# <a name="tag-resource-type"></a><span data-ttu-id="358a9-103">Тип ресурса тегов</span><span class="sxs-lookup"><span data-stu-id="358a9-103">tag resource type</span></span>

<span data-ttu-id="358a9-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="358a9-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="358a9-105">Представляет тег eDiscovery, который используется для маркировки документов во время проверки, чтобы разделять отзывчивый и не отзывчивый контент.</span><span class="sxs-lookup"><span data-stu-id="358a9-105">Represents an eDiscovery tag, which is used to mark documents during review to separate responsive and non-responsive content.</span></span>

<span data-ttu-id="358a9-106">Наследует от [объекта](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="358a9-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="358a9-107">Методы</span><span class="sxs-lookup"><span data-stu-id="358a9-107">Methods</span></span>

|<span data-ttu-id="358a9-108">Метод</span><span class="sxs-lookup"><span data-stu-id="358a9-108">Method</span></span>|<span data-ttu-id="358a9-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="358a9-109">Return type</span></span>|<span data-ttu-id="358a9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="358a9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="358a9-111">Теги списка</span><span class="sxs-lookup"><span data-stu-id="358a9-111">List tags</span></span>](../api/ediscovery-case-list-tags.md)|<span data-ttu-id="358a9-112">[коллекция microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="358a9-112">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection</span></span>|<span data-ttu-id="358a9-113">Получите список объектов **тегов** и их свойств.</span><span class="sxs-lookup"><span data-stu-id="358a9-113">Get a list of the **tag** objects and their properties.</span></span>|
|[<span data-ttu-id="358a9-114">Создание тега</span><span class="sxs-lookup"><span data-stu-id="358a9-114">Create tag</span></span>](../api/ediscovery-case-post-tags.md)|[<span data-ttu-id="358a9-115">microsoft.graph.ediscovery.tag</span><span class="sxs-lookup"><span data-stu-id="358a9-115">microsoft.graph.ediscovery.tag</span></span>](../resources/ediscovery-tag.md)|<span data-ttu-id="358a9-116">Создайте новый **объект тегов.**</span><span class="sxs-lookup"><span data-stu-id="358a9-116">Create a new **tag** object.</span></span>|
|[<span data-ttu-id="358a9-117">Получить тег</span><span class="sxs-lookup"><span data-stu-id="358a9-117">Get tag</span></span>](../api/ediscovery-tag-get.md)|[<span data-ttu-id="358a9-118">microsoft.graph.ediscovery.tag</span><span class="sxs-lookup"><span data-stu-id="358a9-118">microsoft.graph.ediscovery.tag</span></span>](../resources/ediscovery-tag.md)|<span data-ttu-id="358a9-119">Ознакомьтесь с свойствами и отношениями объекта **тегов.**</span><span class="sxs-lookup"><span data-stu-id="358a9-119">Read the properties and relationships of a **tag** object.</span></span>|
|[<span data-ttu-id="358a9-120">Тег обновления</span><span class="sxs-lookup"><span data-stu-id="358a9-120">Update tag</span></span>](../api/ediscovery-tag-update.md)|[<span data-ttu-id="358a9-121">microsoft.graph.ediscovery.tag</span><span class="sxs-lookup"><span data-stu-id="358a9-121">microsoft.graph.ediscovery.tag</span></span>](../resources/ediscovery-tag.md)|<span data-ttu-id="358a9-122">Обновление свойств объекта **тегов.**</span><span class="sxs-lookup"><span data-stu-id="358a9-122">Update the properties of a **tag** object.</span></span>|
|[<span data-ttu-id="358a9-123">Удаление тега</span><span class="sxs-lookup"><span data-stu-id="358a9-123">Delete tag</span></span>](../api/ediscovery-tag-delete.md)|<span data-ttu-id="358a9-124">Нет</span><span class="sxs-lookup"><span data-stu-id="358a9-124">None</span></span>|<span data-ttu-id="358a9-125">Удаление объекта **тега.**</span><span class="sxs-lookup"><span data-stu-id="358a9-125">Delete a **tag** object.</span></span>|
|[<span data-ttu-id="358a9-126">asHierarchy</span><span class="sxs-lookup"><span data-stu-id="358a9-126">asHierarchy</span></span>](../api/ediscovery-tag-ashierarchy.md)|<span data-ttu-id="358a9-127">[коллекция microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="358a9-127">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection</span></span>|<span data-ttu-id="358a9-128">Списки всех тегов, включая их иерархию.</span><span class="sxs-lookup"><span data-stu-id="358a9-128">Lists all tags, including their hierarchy.</span></span>|
|[<span data-ttu-id="358a9-129">Список childTags</span><span class="sxs-lookup"><span data-stu-id="358a9-129">List childTags</span></span>](../api/ediscovery-tag-childtags.md)|<span data-ttu-id="358a9-130">[коллекция microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="358a9-130">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection</span></span>|<span data-ttu-id="358a9-131">Получите список объектов детских **тегов,** связанных с тегом.</span><span class="sxs-lookup"><span data-stu-id="358a9-131">Get a list of child **tag** objects associated with a tag.</span></span>|

## <a name="properties"></a><span data-ttu-id="358a9-132">Свойства</span><span class="sxs-lookup"><span data-stu-id="358a9-132">Properties</span></span>

|<span data-ttu-id="358a9-133">Свойство</span><span class="sxs-lookup"><span data-stu-id="358a9-133">Property</span></span>|<span data-ttu-id="358a9-134">Тип</span><span class="sxs-lookup"><span data-stu-id="358a9-134">Type</span></span>|<span data-ttu-id="358a9-135">Описание</span><span class="sxs-lookup"><span data-stu-id="358a9-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="358a9-136">childSelectability</span><span class="sxs-lookup"><span data-stu-id="358a9-136">childSelectability</span></span>|[<span data-ttu-id="358a9-137">microsoft.graph.ediscovery.childSelectability</span><span class="sxs-lookup"><span data-stu-id="358a9-137">microsoft.graph.ediscovery.childSelectability</span></span>](../resources/ediscovery-tag.md#childselectability-values)|<span data-ttu-id="358a9-138">Указывает, можно ли связывать один или несколько детских тегов с документом.</span><span class="sxs-lookup"><span data-stu-id="358a9-138">Indicates whether a single or multiple child tags can be associated with a document.</span></span> <span data-ttu-id="358a9-139">Возможные значения: `One`, `Many`.</span><span class="sxs-lookup"><span data-stu-id="358a9-139">Possible values are: `One`, `Many`.</span></span>  <span data-ttu-id="358a9-140">Это значение контролирует, представляет ли UX теги в качестве почтовых ящиков или группы кнопок радио.</span><span class="sxs-lookup"><span data-stu-id="358a9-140">This value controls whether the UX presents the tags as checkboxes or a radio button group.</span></span>|
|<span data-ttu-id="358a9-141">createdBy</span><span class="sxs-lookup"><span data-stu-id="358a9-141">createdBy</span></span>|[<span data-ttu-id="358a9-142">identitySet</span><span class="sxs-lookup"><span data-stu-id="358a9-142">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="358a9-143">Пользователь, создавший тег.</span><span class="sxs-lookup"><span data-stu-id="358a9-143">The user who created the tag.</span></span>|
|<span data-ttu-id="358a9-144">description</span><span class="sxs-lookup"><span data-stu-id="358a9-144">description</span></span>|<span data-ttu-id="358a9-145">String</span><span class="sxs-lookup"><span data-stu-id="358a9-145">String</span></span>|<span data-ttu-id="358a9-146">Описание тега.</span><span class="sxs-lookup"><span data-stu-id="358a9-146">The description for the tag.</span></span>|
|<span data-ttu-id="358a9-147">displayName</span><span class="sxs-lookup"><span data-stu-id="358a9-147">displayName</span></span>|<span data-ttu-id="358a9-148">String</span><span class="sxs-lookup"><span data-stu-id="358a9-148">String</span></span>|<span data-ttu-id="358a9-149">Отображение имени тега.</span><span class="sxs-lookup"><span data-stu-id="358a9-149">Display name of the tag.</span></span>|
|<span data-ttu-id="358a9-150">id</span><span class="sxs-lookup"><span data-stu-id="358a9-150">id</span></span>|<span data-ttu-id="358a9-151">String</span><span class="sxs-lookup"><span data-stu-id="358a9-151">String</span></span>|<span data-ttu-id="358a9-152">Уникальный идентификатор тега.</span><span class="sxs-lookup"><span data-stu-id="358a9-152">Unique identifier for the tag.</span></span>|
|<span data-ttu-id="358a9-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="358a9-153">lastModifiedDateTime</span></span>|<span data-ttu-id="358a9-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="358a9-154">DateTimeOffset</span></span>|<span data-ttu-id="358a9-155">Дата и время последнего изменения тега.</span><span class="sxs-lookup"><span data-stu-id="358a9-155">The date and time the tag was last modified.</span></span>|

### <a name="childselectability-values"></a><span data-ttu-id="358a9-156">значения childSelectability</span><span class="sxs-lookup"><span data-stu-id="358a9-156">childSelectability values</span></span>

|<span data-ttu-id="358a9-157">Member</span><span class="sxs-lookup"><span data-stu-id="358a9-157">Member</span></span>|<span data-ttu-id="358a9-158">Описание</span><span class="sxs-lookup"><span data-stu-id="358a9-158">Description</span></span>|
|:----|-----------|
|<span data-ttu-id="358a9-159">Один</span><span class="sxs-lookup"><span data-stu-id="358a9-159">One</span></span>|<span data-ttu-id="358a9-160">Можно выбрать только одного ребенка.</span><span class="sxs-lookup"><span data-stu-id="358a9-160">Only one child can be selected.</span></span> <span data-ttu-id="358a9-161">Это соответствует пользовательскому интерфейсу, который представляет теги с кнопками радио.</span><span class="sxs-lookup"><span data-stu-id="358a9-161">This corresponds to a UI that presents the tags with radio buttons.</span></span>|
|<span data-ttu-id="358a9-162">Многие</span><span class="sxs-lookup"><span data-stu-id="358a9-162">Many</span></span>|<span data-ttu-id="358a9-163">Ноль или много детей могут быть выбраны.</span><span class="sxs-lookup"><span data-stu-id="358a9-163">Zero or many children can be selected.</span></span> <span data-ttu-id="358a9-164">Это соответствует пользовательскому интерфейсу, который представляет теги с почтовыми ящиками.</span><span class="sxs-lookup"><span data-stu-id="358a9-164">This corresponds to a UI that presents the tags with checkboxes.</span></span>|

## <a name="relationships"></a><span data-ttu-id="358a9-165">Связи</span><span class="sxs-lookup"><span data-stu-id="358a9-165">Relationships</span></span>

|<span data-ttu-id="358a9-166">Связь</span><span class="sxs-lookup"><span data-stu-id="358a9-166">Relationship</span></span>|<span data-ttu-id="358a9-167">Тип</span><span class="sxs-lookup"><span data-stu-id="358a9-167">Type</span></span>|<span data-ttu-id="358a9-168">Описание</span><span class="sxs-lookup"><span data-stu-id="358a9-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="358a9-169">childTags</span><span class="sxs-lookup"><span data-stu-id="358a9-169">childTags</span></span>|<span data-ttu-id="358a9-170">[коллекция microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)</span><span class="sxs-lookup"><span data-stu-id="358a9-170">[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection</span></span>|<span data-ttu-id="358a9-171">Возвращает теги, которые являются ребенком тега.</span><span class="sxs-lookup"><span data-stu-id="358a9-171">Returns the tags that are a child of a tag.</span></span>|
|<span data-ttu-id="358a9-172">родитель</span><span class="sxs-lookup"><span data-stu-id="358a9-172">parent</span></span>|[<span data-ttu-id="358a9-173">microsoft.graph.ediscovery.tag</span><span class="sxs-lookup"><span data-stu-id="358a9-173">microsoft.graph.ediscovery.tag</span></span>](../resources/ediscovery-tag.md)|<span data-ttu-id="358a9-174">Возвращает родительский тег указанного тега.</span><span class="sxs-lookup"><span data-stu-id="358a9-174">Returns the parent tag of the specified tag.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="358a9-175">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="358a9-175">JSON representation</span></span>

<span data-ttu-id="358a9-176">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="358a9-176">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.tag",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.tag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "childSelectability": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```
