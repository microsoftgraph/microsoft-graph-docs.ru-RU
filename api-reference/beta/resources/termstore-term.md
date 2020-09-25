---
title: Тип ресурса термина
description: Определяет сущность термина в банке терминов.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 71c22c86d2ebbb02587a20355adb1d461479297d
ms.sourcegitcommit: 3c0fa2d13ede0fdfa66d966d4ec32cb468c3befa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/25/2020
ms.locfileid: "48273580"
---
# <a name="term-resource-type"></a><span data-ttu-id="538ef-103">Тип ресурса термина</span><span class="sxs-lookup"><span data-stu-id="538ef-103">term resource type</span></span>

<span data-ttu-id="538ef-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="538ef-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="538ef-105">Представляет термин, используемый в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="538ef-105">Represents a term used in a term [store].</span></span> <span data-ttu-id="538ef-106">Термин можно использовать для представления объекта, который затем можно использовать в качестве метаданных для контента.</span><span class="sxs-lookup"><span data-stu-id="538ef-106">A term can be used to represent an object which can then be used as a metadata to tag content.</span></span> <span data-ttu-id="538ef-107">Несколько терминов можно организовать иерархически в пределах [набора].</span><span class="sxs-lookup"><span data-stu-id="538ef-107">Multiple terms can be organized in a hierarchical manner within a [set].</span></span>

<span data-ttu-id="538ef-108">Наследуется от [объекта Entity](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="538ef-108">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="538ef-109">Методы</span><span class="sxs-lookup"><span data-stu-id="538ef-109">Methods</span></span>
|<span data-ttu-id="538ef-110">Метод</span><span class="sxs-lookup"><span data-stu-id="538ef-110">Method</span></span>|<span data-ttu-id="538ef-111">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="538ef-111">Return type</span></span>|<span data-ttu-id="538ef-112">Описание</span><span class="sxs-lookup"><span data-stu-id="538ef-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="538ef-113">Список дочерних элементов</span><span class="sxs-lookup"><span data-stu-id="538ef-113">List children</span></span>](../api/termstore-term-list-children.md)|<span data-ttu-id="538ef-114">Коллекция [Microsoft. Graph. Банк терминов Microsoft. Graph.](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="538ef-114">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="538ef-115">Получение потомков первого уровня термина в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="538ef-115">Get the first level children of a term in a term [store].</span></span>|
|[<span data-ttu-id="538ef-116">Список отношений</span><span class="sxs-lookup"><span data-stu-id="538ef-116">List relations</span></span>](../api/termstore-term-list-relations.md)|<span data-ttu-id="538ef-117">Коллекция [Microsoft. Graph. Банк. relation](../resources/termstore-relation.md)</span><span class="sxs-lookup"><span data-stu-id="538ef-117">[microsoft.graph.termStore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="538ef-118">Получение отношений терминов в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="538ef-118">Get the relations of a term in a term [store].</span></span>|
|[<span data-ttu-id="538ef-119">Создание отношения</span><span class="sxs-lookup"><span data-stu-id="538ef-119">Create relation</span></span>](../api/termstore-relation-post.md)|[<span data-ttu-id="538ef-120">Microsoft. Graph. Банк. отношение</span><span class="sxs-lookup"><span data-stu-id="538ef-120">microsoft.graph.termStore.relation</span></span>](../resources/termstore-relation.md)|<span data-ttu-id="538ef-121">Создание нового отношения для термина или [набора] в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="538ef-121">Create a new relation for a term or a [set] in a term [store].</span></span>|
|[<span data-ttu-id="538ef-122">Создание термина</span><span class="sxs-lookup"><span data-stu-id="538ef-122">Create term</span></span>](../api/termstore-term-post.md)|[<span data-ttu-id="538ef-123">Microsoft. Graph. Банк. Term</span><span class="sxs-lookup"><span data-stu-id="538ef-123">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="538ef-124">Создайте новый объект Term в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="538ef-124">Create a new term object in a term [store].</span></span>|
|[<span data-ttu-id="538ef-125">Получение термина</span><span class="sxs-lookup"><span data-stu-id="538ef-125">Get term</span></span>](../api/termstore-term-get.md)|[<span data-ttu-id="538ef-126">Microsoft. Graph. Банк. Term</span><span class="sxs-lookup"><span data-stu-id="538ef-126">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="538ef-127">Чтение свойств и связей объекта Term в  [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="538ef-127">Read the properties and relationships of a term object in a term  [store].</span></span>|
|[<span data-ttu-id="538ef-128">Обновление термина</span><span class="sxs-lookup"><span data-stu-id="538ef-128">Update term</span></span>](../api/termstore-term-update.md)|[<span data-ttu-id="538ef-129">Microsoft. Graph. Банк. Term</span><span class="sxs-lookup"><span data-stu-id="538ef-129">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="538ef-130">Обновление свойств объекта Term в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="538ef-130">Update the properties of a term object in a term [store].</span></span>|
|[<span data-ttu-id="538ef-131">Удаление термина</span><span class="sxs-lookup"><span data-stu-id="538ef-131">Delete term</span></span>](../api/termstore-term-delete.md)|<span data-ttu-id="538ef-132">Нет</span><span class="sxs-lookup"><span data-stu-id="538ef-132">None</span></span>|<span data-ttu-id="538ef-133">Удаление объекта Term в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="538ef-133">Delete a term object in a term [store].</span></span>|

## <a name="properties"></a><span data-ttu-id="538ef-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="538ef-134">Properties</span></span>
|<span data-ttu-id="538ef-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="538ef-135">Property</span></span>|<span data-ttu-id="538ef-136">Тип</span><span class="sxs-lookup"><span data-stu-id="538ef-136">Type</span></span>|<span data-ttu-id="538ef-137">Описание</span><span class="sxs-lookup"><span data-stu-id="538ef-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="538ef-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="538ef-138">createdDateTime</span></span>|<span data-ttu-id="538ef-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="538ef-139">DateTimeOffset</span></span>|<span data-ttu-id="538ef-140">Дата и время создания терминов.</span><span class="sxs-lookup"><span data-stu-id="538ef-140">Date and time of term creation.</span></span> <span data-ttu-id="538ef-141">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="538ef-141">Read-only</span></span>|
|<span data-ttu-id="538ef-142">состояний</span><span class="sxs-lookup"><span data-stu-id="538ef-142">descriptions</span></span>|<span data-ttu-id="538ef-143">Коллекция [Microsoft. Graph. банка Microsoft. Graph. локализеддескриптион](../resources/termstore-localizeddescription.md)</span><span class="sxs-lookup"><span data-stu-id="538ef-143">[microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md) collection</span></span>|<span data-ttu-id="538ef-144">Описание термина, зависящего от Лангуажетаг</span><span class="sxs-lookup"><span data-stu-id="538ef-144">Description about term that is dependent on the languageTag</span></span>|
|<span data-ttu-id="538ef-145">id</span><span class="sxs-lookup"><span data-stu-id="538ef-145">id</span></span>|<span data-ttu-id="538ef-146">String</span><span class="sxs-lookup"><span data-stu-id="538ef-146">String</span></span>|<span data-ttu-id="538ef-147">Уникальный идентификатор термина.</span><span class="sxs-lookup"><span data-stu-id="538ef-147">Unique identifier of term.</span></span> <span data-ttu-id="538ef-148">Только чтение</span><span class="sxs-lookup"><span data-stu-id="538ef-148">Read-Only</span></span>|
|<span data-ttu-id="538ef-149">Метка</span><span class="sxs-lookup"><span data-stu-id="538ef-149">labels</span></span>|<span data-ttu-id="538ef-150">Коллекция [Microsoft. Graph. банка Microsoft. Graph. локализедлабел](../resources/termstore-localizedlabel.md)</span><span class="sxs-lookup"><span data-stu-id="538ef-150">[microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md) collection</span></span>||<span data-ttu-id="538ef-151">Метаданные метки для термина</span><span class="sxs-lookup"><span data-stu-id="538ef-151">Label metadata for a term</span></span>|
|<span data-ttu-id="538ef-152">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="538ef-152">lastModifiedDateTime</span></span>|<span data-ttu-id="538ef-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="538ef-153">DateTimeOffset</span></span>|<span data-ttu-id="538ef-154">Дата и время последнего изменения термина.</span><span class="sxs-lookup"><span data-stu-id="538ef-154">Last date and time of term modification.</span></span> <span data-ttu-id="538ef-155">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="538ef-155">Read-only</span></span>|
|<span data-ttu-id="538ef-156">properties</span><span class="sxs-lookup"><span data-stu-id="538ef-156">properties</span></span>|<span data-ttu-id="538ef-157">Коллекция [Microsoft. Graph. ключзначение](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="538ef-157">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="538ef-158">Коллекция свойств термина</span><span class="sxs-lookup"><span data-stu-id="538ef-158">Collection of properties on the term</span></span>|

## <a name="relationships"></a><span data-ttu-id="538ef-159">Связи</span><span class="sxs-lookup"><span data-stu-id="538ef-159">Relationships</span></span>
|<span data-ttu-id="538ef-160">Связь</span><span class="sxs-lookup"><span data-stu-id="538ef-160">Relationship</span></span>|<span data-ttu-id="538ef-161">Тип</span><span class="sxs-lookup"><span data-stu-id="538ef-161">Type</span></span>|<span data-ttu-id="538ef-162">Описание</span><span class="sxs-lookup"><span data-stu-id="538ef-162">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="538ef-163">children</span><span class="sxs-lookup"><span data-stu-id="538ef-163">children</span></span>|<span data-ttu-id="538ef-164">Коллекция [Microsoft. Graph. Банк терминов Microsoft. Graph.](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="538ef-164">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="538ef-165">Дочерние элементы текущего термина</span><span class="sxs-lookup"><span data-stu-id="538ef-165">Children of current term</span></span>|
|<span data-ttu-id="538ef-166">отношениях</span><span class="sxs-lookup"><span data-stu-id="538ef-166">relations</span></span>|<span data-ttu-id="538ef-167">Коллекция [Microsoft. Graph. Банк. relation](../resources/termstore-relation.md)</span><span class="sxs-lookup"><span data-stu-id="538ef-167">[microsoft.graph.termStore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="538ef-168">Указание терминов, связанных с текущим термином, в качестве закрепления или повторного использования</span><span class="sxs-lookup"><span data-stu-id="538ef-168">To indicate which terms are related to the current term as either pinned or reused</span></span>|
|<span data-ttu-id="538ef-169">set</span><span class="sxs-lookup"><span data-stu-id="538ef-169">set</span></span>|[<span data-ttu-id="538ef-170">Microsoft. Graph. банка. Set</span><span class="sxs-lookup"><span data-stu-id="538ef-170">microsoft.graph.termStore.set</span></span>](../resources/termstore-set.md)|<span data-ttu-id="538ef-171">[Набор] , в котором создается термин</span><span class="sxs-lookup"><span data-stu-id="538ef-171">The [set] in which the term is created</span></span>|

## <a name="json-representation"></a><span data-ttu-id="538ef-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="538ef-172">JSON representation</span></span>
<span data-ttu-id="538ef-173">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="538ef-173">The following is a JSON representation of the resource.</span></span>
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


