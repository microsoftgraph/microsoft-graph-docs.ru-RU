---
title: тип ресурса терминов
description: Определяет сущность терминов в магазине терминов.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 5645b85a5d017fd05010e04e118853a904a78b6c
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516180"
---
# <a name="term-resource-type"></a><span data-ttu-id="b9cf1-103">тип ресурса терминов</span><span class="sxs-lookup"><span data-stu-id="b9cf1-103">term resource type</span></span>

<span data-ttu-id="b9cf1-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="b9cf1-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9cf1-105">Представляет термин, используемый в магазине [терминов.]</span><span class="sxs-lookup"><span data-stu-id="b9cf1-105">Represents a term used in a term [store].</span></span> <span data-ttu-id="b9cf1-106">Термин можно использовать для представления объекта, который затем можно использовать в качестве метаданных для тегов контента.</span><span class="sxs-lookup"><span data-stu-id="b9cf1-106">A term can be used to represent an object which can then be used as a metadata to tag content.</span></span> <span data-ttu-id="b9cf1-107">Несколько терминов могут быть организованы иерархическим образом в [наборе].</span><span class="sxs-lookup"><span data-stu-id="b9cf1-107">Multiple terms can be organized in a hierarchical manner within a [set].</span></span>

<span data-ttu-id="b9cf1-108">Наследует от [объекта](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="b9cf1-108">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b9cf1-109">Методы</span><span class="sxs-lookup"><span data-stu-id="b9cf1-109">Methods</span></span>
|<span data-ttu-id="b9cf1-110">Метод</span><span class="sxs-lookup"><span data-stu-id="b9cf1-110">Method</span></span>|<span data-ttu-id="b9cf1-111">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="b9cf1-111">Return type</span></span>|<span data-ttu-id="b9cf1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b9cf1-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b9cf1-113">Список дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="b9cf1-113">List children</span></span>](../api/termstore-term-list-children.md)|<span data-ttu-id="b9cf1-114">[коллекция microsoft.graph.termStore.term](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="b9cf1-114">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="b9cf1-115">Получите детей первого уровня термина в магазине [терминов.]</span><span class="sxs-lookup"><span data-stu-id="b9cf1-115">Get the first level children of a term in a term [store].</span></span>|
|[<span data-ttu-id="b9cf1-116">Отношения списка</span><span class="sxs-lookup"><span data-stu-id="b9cf1-116">List relations</span></span>](../api/termstore-term-list-relations.md)|<span data-ttu-id="b9cf1-117">[коллекция microsoft.graph.termStore.relation](../resources/termstore-relation.md)</span><span class="sxs-lookup"><span data-stu-id="b9cf1-117">[microsoft.graph.termStore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="b9cf1-118">Получите отношения термина в магазине [терминов.]</span><span class="sxs-lookup"><span data-stu-id="b9cf1-118">Get the relations of a term in a term [store].</span></span>|
|[<span data-ttu-id="b9cf1-119">Создание связи</span><span class="sxs-lookup"><span data-stu-id="b9cf1-119">Create relation</span></span>](../api/termstore-relation-post.md)|[<span data-ttu-id="b9cf1-120">microsoft.graph.termStore.relation</span><span class="sxs-lookup"><span data-stu-id="b9cf1-120">microsoft.graph.termStore.relation</span></span>](../resources/termstore-relation.md)|<span data-ttu-id="b9cf1-121">Создание нового отношения для термина или набора [в] магазине [терминов.]</span><span class="sxs-lookup"><span data-stu-id="b9cf1-121">Create a new relation for a term or a [set] in a term [store].</span></span>|
|[<span data-ttu-id="b9cf1-122">Создание термина</span><span class="sxs-lookup"><span data-stu-id="b9cf1-122">Create term</span></span>](../api/termstore-term-post.md)|[<span data-ttu-id="b9cf1-123">microsoft.graph.termStore.term</span><span class="sxs-lookup"><span data-stu-id="b9cf1-123">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="b9cf1-124">Создание нового объекта терминов в магазине [терминов.]</span><span class="sxs-lookup"><span data-stu-id="b9cf1-124">Create a new term object in a term [store].</span></span>|
|[<span data-ttu-id="b9cf1-125">Получить термин</span><span class="sxs-lookup"><span data-stu-id="b9cf1-125">Get term</span></span>](../api/termstore-term-get.md)|[<span data-ttu-id="b9cf1-126">microsoft.graph.termStore.term</span><span class="sxs-lookup"><span data-stu-id="b9cf1-126">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="b9cf1-127">Ознакомьтесь с свойствами и отношениями объекта терминов в магазине [терминов.]</span><span class="sxs-lookup"><span data-stu-id="b9cf1-127">Read the properties and relationships of a term object in a term  [store].</span></span>|
|[<span data-ttu-id="b9cf1-128">Термин Update</span><span class="sxs-lookup"><span data-stu-id="b9cf1-128">Update term</span></span>](../api/termstore-term-update.md)|[<span data-ttu-id="b9cf1-129">microsoft.graph.termStore.term</span><span class="sxs-lookup"><span data-stu-id="b9cf1-129">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="b9cf1-130">Обновление свойств объекта терминов в магазине [терминов.]</span><span class="sxs-lookup"><span data-stu-id="b9cf1-130">Update the properties of a term object in a term [store].</span></span>|
|[<span data-ttu-id="b9cf1-131">Удаление термина</span><span class="sxs-lookup"><span data-stu-id="b9cf1-131">Delete term</span></span>](../api/termstore-term-delete.md)|<span data-ttu-id="b9cf1-132">Нет</span><span class="sxs-lookup"><span data-stu-id="b9cf1-132">None</span></span>|<span data-ttu-id="b9cf1-133">Удаление объекта терминов в магазине [терминов.]</span><span class="sxs-lookup"><span data-stu-id="b9cf1-133">Delete a term object in a term [store].</span></span>|

## <a name="properties"></a><span data-ttu-id="b9cf1-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="b9cf1-134">Properties</span></span>
|<span data-ttu-id="b9cf1-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="b9cf1-135">Property</span></span>|<span data-ttu-id="b9cf1-136">Тип</span><span class="sxs-lookup"><span data-stu-id="b9cf1-136">Type</span></span>|<span data-ttu-id="b9cf1-137">Описание</span><span class="sxs-lookup"><span data-stu-id="b9cf1-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9cf1-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b9cf1-138">createdDateTime</span></span>|<span data-ttu-id="b9cf1-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9cf1-139">DateTimeOffset</span></span>|<span data-ttu-id="b9cf1-140">Дата и время создания терминов.</span><span class="sxs-lookup"><span data-stu-id="b9cf1-140">Date and time of term creation.</span></span> <span data-ttu-id="b9cf1-141">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="b9cf1-141">Read-only</span></span>|
|<span data-ttu-id="b9cf1-142">описания</span><span class="sxs-lookup"><span data-stu-id="b9cf1-142">descriptions</span></span>|<span data-ttu-id="b9cf1-143">[коллекция microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md)</span><span class="sxs-lookup"><span data-stu-id="b9cf1-143">[microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md) collection</span></span>|<span data-ttu-id="b9cf1-144">Описание терминов, зависящих от languageTag</span><span class="sxs-lookup"><span data-stu-id="b9cf1-144">Description about term that is dependent on the languageTag</span></span>|
|<span data-ttu-id="b9cf1-145">id</span><span class="sxs-lookup"><span data-stu-id="b9cf1-145">id</span></span>|<span data-ttu-id="b9cf1-146">Строка</span><span class="sxs-lookup"><span data-stu-id="b9cf1-146">String</span></span>|<span data-ttu-id="b9cf1-147">Уникальный идентификатор термина.</span><span class="sxs-lookup"><span data-stu-id="b9cf1-147">Unique identifier of term.</span></span> <span data-ttu-id="b9cf1-148">Только чтение</span><span class="sxs-lookup"><span data-stu-id="b9cf1-148">Read-Only</span></span>|
|<span data-ttu-id="b9cf1-149">метки</span><span class="sxs-lookup"><span data-stu-id="b9cf1-149">labels</span></span>|<span data-ttu-id="b9cf1-150">[коллекция microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md)</span><span class="sxs-lookup"><span data-stu-id="b9cf1-150">[microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md) collection</span></span>|<span data-ttu-id="b9cf1-151">Метаданные меток для термина</span><span class="sxs-lookup"><span data-stu-id="b9cf1-151">Label metadata for a term</span></span>|
|<span data-ttu-id="b9cf1-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9cf1-152">lastModifiedDateTime</span></span>|<span data-ttu-id="b9cf1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9cf1-153">DateTimeOffset</span></span>|<span data-ttu-id="b9cf1-154">Последняя дата и время изменения срока.</span><span class="sxs-lookup"><span data-stu-id="b9cf1-154">Last date and time of term modification.</span></span> <span data-ttu-id="b9cf1-155">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="b9cf1-155">Read-only</span></span>|
|<span data-ttu-id="b9cf1-156">properties</span><span class="sxs-lookup"><span data-stu-id="b9cf1-156">properties</span></span>|<span data-ttu-id="b9cf1-157">[коллекция microsoft.graph.keyValue](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="b9cf1-157">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="b9cf1-158">Коллекция свойств в термине</span><span class="sxs-lookup"><span data-stu-id="b9cf1-158">Collection of properties on the term</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9cf1-159">Отношения</span><span class="sxs-lookup"><span data-stu-id="b9cf1-159">Relationships</span></span>
|<span data-ttu-id="b9cf1-160">Связь</span><span class="sxs-lookup"><span data-stu-id="b9cf1-160">Relationship</span></span>|<span data-ttu-id="b9cf1-161">Тип</span><span class="sxs-lookup"><span data-stu-id="b9cf1-161">Type</span></span>|<span data-ttu-id="b9cf1-162">Описание</span><span class="sxs-lookup"><span data-stu-id="b9cf1-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9cf1-163">children</span><span class="sxs-lookup"><span data-stu-id="b9cf1-163">children</span></span>|<span data-ttu-id="b9cf1-164">[коллекция microsoft.graph.termStore.term](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="b9cf1-164">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="b9cf1-165">Дети текущего срока</span><span class="sxs-lookup"><span data-stu-id="b9cf1-165">Children of current term</span></span>|
|<span data-ttu-id="b9cf1-166">отношения</span><span class="sxs-lookup"><span data-stu-id="b9cf1-166">relations</span></span>|<span data-ttu-id="b9cf1-167">[коллекция microsoft.graph.termStore.relation](../resources/termstore-relation.md)</span><span class="sxs-lookup"><span data-stu-id="b9cf1-167">[microsoft.graph.termStore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="b9cf1-168">Указать, какие термины связаны с текущим термином как закрепленные или повторно</span><span class="sxs-lookup"><span data-stu-id="b9cf1-168">To indicate which terms are related to the current term as either pinned or reused</span></span>|
|<span data-ttu-id="b9cf1-169">set</span><span class="sxs-lookup"><span data-stu-id="b9cf1-169">set</span></span>|[<span data-ttu-id="b9cf1-170">microsoft.graph.termStore.set</span><span class="sxs-lookup"><span data-stu-id="b9cf1-170">microsoft.graph.termStore.set</span></span>](../resources/termstore-set.md)|<span data-ttu-id="b9cf1-171">[Набор,] в котором создается термин</span><span class="sxs-lookup"><span data-stu-id="b9cf1-171">The [set] in which the term is created</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9cf1-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b9cf1-172">JSON representation</span></span>
<span data-ttu-id="b9cf1-173">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b9cf1-173">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.term",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.term",
  "id": "String (identifier)",
  "labels": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedLabel"
    }
  ],
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "descriptions": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedDescription"
    }
  ],
  "properties": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ]
}
```

[store]: ../resources/termstore-store.md
[set]: ../resources/termstore-set.md
[term]: ../resources/termstore-term.md
[group]: ../resources/termstore-group.md

<!--
{
  "type": "#page.annotation",
  "description": "Term is the entity used for tagging in termStore",
  "keywords": "term,facet,resource",
  "section": "documentation",
  "tocPath": "Terms",
  "tocBookmarks": {
    "Resources/termstore-term": "#"
  },
  "suppressions": []
}
-->


