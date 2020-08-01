---
title: Тип ресурса термина
description: Определяет сущность термина в банке терминов.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 77f907ee80c0710e33771efb33c3a3eee893f2ed
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539448"
---
# <a name="term-resource-type"></a><span data-ttu-id="be5be-103">Тип ресурса термина</span><span class="sxs-lookup"><span data-stu-id="be5be-103">term resource type</span></span>

<span data-ttu-id="be5be-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="be5be-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be5be-105">Представляет термин, используемый в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="be5be-105">Represents a term used in a term [store].</span></span> <span data-ttu-id="be5be-106">Термин можно использовать для представления объекта, который затем можно использовать в качестве метаданных для тега конент.</span><span class="sxs-lookup"><span data-stu-id="be5be-106">A term can be used to represent an object which can then be used as a metadata to tag conent.</span></span> <span data-ttu-id="be5be-107">Несколько терминов можно организовать иерархически в пределах [набора].</span><span class="sxs-lookup"><span data-stu-id="be5be-107">Multiple terms can be organized in a hierarchical manner within a [set].</span></span>

<span data-ttu-id="be5be-108">Наследуется от [объекта Entity](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="be5be-108">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="be5be-109">Методы</span><span class="sxs-lookup"><span data-stu-id="be5be-109">Methods</span></span>
|<span data-ttu-id="be5be-110">Метод</span><span class="sxs-lookup"><span data-stu-id="be5be-110">Method</span></span>|<span data-ttu-id="be5be-111">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="be5be-111">Return type</span></span>|<span data-ttu-id="be5be-112">Описание</span><span class="sxs-lookup"><span data-stu-id="be5be-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="be5be-113">Список дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="be5be-113">List children</span></span>](../api/termstore-term-list-children.md)|<span data-ttu-id="be5be-114">Коллекция [Microsoft. Graph. Банк терминов Microsoft. Graph.](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="be5be-114">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="be5be-115">Получение потомков первого уровня термина в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="be5be-115">Get the first level children of a term in a term [store].</span></span>|
|[<span data-ttu-id="be5be-116">Список отношений</span><span class="sxs-lookup"><span data-stu-id="be5be-116">List relations</span></span>](../api/termstore-term-list-relations.md)|<span data-ttu-id="be5be-117">Коллекция [Microsoft. Graph. Банк. relation](../resources/termstore-relation.md)</span><span class="sxs-lookup"><span data-stu-id="be5be-117">[microsoft.graph.termStore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="be5be-118">Получение отношений терминов в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="be5be-118">Get the relations of a term in a term [store].</span></span>|
|[<span data-ttu-id="be5be-119">Создание отношения</span><span class="sxs-lookup"><span data-stu-id="be5be-119">Create relation</span></span>](../api/termstore-relation-post.md)|[<span data-ttu-id="be5be-120">Microsoft. Graph. Банк. отношение</span><span class="sxs-lookup"><span data-stu-id="be5be-120">microsoft.graph.termStore.relation</span></span>](../resources/termstore-relation.md)|<span data-ttu-id="be5be-121">Создание нового отношения для термина или [набора] в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="be5be-121">Create a new relation for a term or a [set] in a term [store].</span></span>|
|[<span data-ttu-id="be5be-122">Создание термина</span><span class="sxs-lookup"><span data-stu-id="be5be-122">Create term</span></span>](../api/termstore-term-post.md)|[<span data-ttu-id="be5be-123">Microsoft. Graph. Банк. Term</span><span class="sxs-lookup"><span data-stu-id="be5be-123">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="be5be-124">Создайте новый объект Term в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="be5be-124">Create a new term object in a term [store].</span></span>|
|[<span data-ttu-id="be5be-125">Получение термина</span><span class="sxs-lookup"><span data-stu-id="be5be-125">Get term</span></span>](../api/termstore-term-get.md)|[<span data-ttu-id="be5be-126">Microsoft. Graph. Банк. Term</span><span class="sxs-lookup"><span data-stu-id="be5be-126">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="be5be-127">Чтение свойств и связей объекта Term в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="be5be-127">Read the properties and relationships of a term object in a term  [store].</span></span>|
|[<span data-ttu-id="be5be-128">Обновление термина</span><span class="sxs-lookup"><span data-stu-id="be5be-128">Update term</span></span>](../api/termstore-term-update.md)|[<span data-ttu-id="be5be-129">Microsoft. Graph. Банк. Term</span><span class="sxs-lookup"><span data-stu-id="be5be-129">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="be5be-130">Обновление свойств объекта Term в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="be5be-130">Update the properties of a term object in a term [store].</span></span>|
|[<span data-ttu-id="be5be-131">Удаление термина</span><span class="sxs-lookup"><span data-stu-id="be5be-131">Delete term</span></span>](../api/termstore-term-delete.md)|<span data-ttu-id="be5be-132">Нет</span><span class="sxs-lookup"><span data-stu-id="be5be-132">None</span></span>|<span data-ttu-id="be5be-133">Удаление объекта Term в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="be5be-133">Delete a term object in a term [store].</span></span>|

## <a name="properties"></a><span data-ttu-id="be5be-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="be5be-134">Properties</span></span>
|<span data-ttu-id="be5be-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="be5be-135">Property</span></span>|<span data-ttu-id="be5be-136">Тип</span><span class="sxs-lookup"><span data-stu-id="be5be-136">Type</span></span>|<span data-ttu-id="be5be-137">Описание</span><span class="sxs-lookup"><span data-stu-id="be5be-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be5be-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="be5be-138">createdDateTime</span></span>|<span data-ttu-id="be5be-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be5be-139">DateTimeOffset</span></span>|<span data-ttu-id="be5be-140">Дата и время создания терминов.</span><span class="sxs-lookup"><span data-stu-id="be5be-140">Date and time of term creation.</span></span> <span data-ttu-id="be5be-141">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="be5be-141">Read-only</span></span>|
|<span data-ttu-id="be5be-142">состояний</span><span class="sxs-lookup"><span data-stu-id="be5be-142">descriptions</span></span>|<span data-ttu-id="be5be-143">Коллекция [Microsoft. Graph. банка Microsoft. Graph. локализеддескриптион](../resources/termstore-localizeddescription.md)</span><span class="sxs-lookup"><span data-stu-id="be5be-143">[microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md) collection</span></span>|<span data-ttu-id="be5be-144">Описание термина, зависящего от Лангуажетаг</span><span class="sxs-lookup"><span data-stu-id="be5be-144">Description about term that is dependent on the languageTag</span></span>|
|<span data-ttu-id="be5be-145">id</span><span class="sxs-lookup"><span data-stu-id="be5be-145">id</span></span>|<span data-ttu-id="be5be-146">String</span><span class="sxs-lookup"><span data-stu-id="be5be-146">String</span></span>|<span data-ttu-id="be5be-147">Уникальный идентификатор термина.</span><span class="sxs-lookup"><span data-stu-id="be5be-147">Unique identifier of term.</span></span> <span data-ttu-id="be5be-148">Только чтение</span><span class="sxs-lookup"><span data-stu-id="be5be-148">Read-Only</span></span>|
|<span data-ttu-id="be5be-149">Метка</span><span class="sxs-lookup"><span data-stu-id="be5be-149">labels</span></span>|<span data-ttu-id="be5be-150">Коллекция [Microsoft. Graph. банка Microsoft. Graph. локализедлабел](../resources/termstore-localizedlabel.md)</span><span class="sxs-lookup"><span data-stu-id="be5be-150">[microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md) collection</span></span>||<span data-ttu-id="be5be-151">Метаданные метки для термина</span><span class="sxs-lookup"><span data-stu-id="be5be-151">Label metadata for a term</span></span>|
|<span data-ttu-id="be5be-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="be5be-152">lastModifiedDateTime</span></span>|<span data-ttu-id="be5be-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="be5be-153">DateTimeOffset</span></span>|<span data-ttu-id="be5be-154">Дата и время последнего изменения термина.</span><span class="sxs-lookup"><span data-stu-id="be5be-154">Last date and time of term modification.</span></span> <span data-ttu-id="be5be-155">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="be5be-155">Read-only</span></span>|
|<span data-ttu-id="be5be-156">properties</span><span class="sxs-lookup"><span data-stu-id="be5be-156">properties</span></span>|<span data-ttu-id="be5be-157">Коллекция [Microsoft. Graph. ключзначение](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="be5be-157">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="be5be-158">Коллекция свойств термина</span><span class="sxs-lookup"><span data-stu-id="be5be-158">Collection of properties on the term</span></span>|

## <a name="relationships"></a><span data-ttu-id="be5be-159">Связи</span><span class="sxs-lookup"><span data-stu-id="be5be-159">Relationships</span></span>
|<span data-ttu-id="be5be-160">Связь</span><span class="sxs-lookup"><span data-stu-id="be5be-160">Relationship</span></span>|<span data-ttu-id="be5be-161">Тип</span><span class="sxs-lookup"><span data-stu-id="be5be-161">Type</span></span>|<span data-ttu-id="be5be-162">Описание</span><span class="sxs-lookup"><span data-stu-id="be5be-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be5be-163">children</span><span class="sxs-lookup"><span data-stu-id="be5be-163">children</span></span>|<span data-ttu-id="be5be-164">Коллекция [Microsoft. Graph. Банк терминов Microsoft. Graph.](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="be5be-164">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="be5be-165">Дочерние элементы текущего термина</span><span class="sxs-lookup"><span data-stu-id="be5be-165">Children of current term</span></span>|
|<span data-ttu-id="be5be-166">отношениях</span><span class="sxs-lookup"><span data-stu-id="be5be-166">relations</span></span>|<span data-ttu-id="be5be-167">Коллекция [Microsoft. Graph. Банк. relation](../resources/termstore-relation.md)</span><span class="sxs-lookup"><span data-stu-id="be5be-167">[microsoft.graph.termStore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="be5be-168">Указание терминов, связанных с текущим термином, в качестве закрепления или повторного использования</span><span class="sxs-lookup"><span data-stu-id="be5be-168">To indicate which terms are related to the current term as either pinned or reused</span></span>|
|<span data-ttu-id="be5be-169">set</span><span class="sxs-lookup"><span data-stu-id="be5be-169">set</span></span>|[<span data-ttu-id="be5be-170">Microsoft. Graph. банка. Set</span><span class="sxs-lookup"><span data-stu-id="be5be-170">microsoft.graph.termStore.set</span></span>](../resources/termstore-set.md)|<span data-ttu-id="be5be-171">[Набор] , в котором создается термин</span><span class="sxs-lookup"><span data-stu-id="be5be-171">The [set] in which the term is created</span></span>|

## <a name="json-representation"></a><span data-ttu-id="be5be-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be5be-172">JSON representation</span></span>
<span data-ttu-id="be5be-173">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be5be-173">The following is a JSON representation of the resource.</span></span>
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

[восстановлен]: ../resources/termstore-store.md
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
