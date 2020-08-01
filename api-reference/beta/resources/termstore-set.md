---
title: задать тип ресурса
description: Представляет набор в банке терминов.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 5e74e0a603d088c7964b13fad51018171642c6ec
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539387"
---
# <a name="set-resource-type"></a><span data-ttu-id="e884c-103">задать тип ресурса</span><span class="sxs-lookup"><span data-stu-id="e884c-103">set resource type</span></span>

<span data-ttu-id="e884c-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="e884c-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e884c-105">Представляет набор, используемый в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="e884c-105">Represents the set used in a term [store].</span></span> <span data-ttu-id="e884c-106">Набор представляет единицу измерения, которая содержит коллекцию иерархических терминов.</span><span class="sxs-lookup"><span data-stu-id="e884c-106">The set represents a unit which contains a collection of hierarchical terms.</span></span> <span data-ttu-id="e884c-107">[Группа] может содержать несколько наборов.</span><span class="sxs-lookup"><span data-stu-id="e884c-107">A [group] can contain multiple sets.</span></span>

<span data-ttu-id="e884c-108">Наследуется от [объекта Entity](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="e884c-108">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e884c-109">Методы</span><span class="sxs-lookup"><span data-stu-id="e884c-109">Methods</span></span>
|<span data-ttu-id="e884c-110">Метод</span><span class="sxs-lookup"><span data-stu-id="e884c-110">Method</span></span>|<span data-ttu-id="e884c-111">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="e884c-111">Return type</span></span>|<span data-ttu-id="e884c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e884c-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e884c-113">Наборы списков</span><span class="sxs-lookup"><span data-stu-id="e884c-113">List sets</span></span>](../api/termstore-group-list-sets.md)|<span data-ttu-id="e884c-114">Коллекция [Microsoft. Graph. банка. Set]</span><span class="sxs-lookup"><span data-stu-id="e884c-114">collection [microsoft.graph.termStore.set]</span></span> | <span data-ttu-id="e884c-115">Возвращает список наборов, содержащихся в [группе] [банка] терминов.</span><span class="sxs-lookup"><span data-stu-id="e884c-115">Returns list of sets contained within a [group] of a term [store]</span></span> |
|[<span data-ttu-id="e884c-116">Создание набора</span><span class="sxs-lookup"><span data-stu-id="e884c-116">Create set</span></span>](../api/termstore-set-post.md)|[<span data-ttu-id="e884c-117">Microsoft. Graph. банка. Set</span><span class="sxs-lookup"><span data-stu-id="e884c-117">microsoft.graph.termStore.set</span></span>](../resources/termstore-set.md)|<span data-ttu-id="e884c-118">Создайте новый объект set в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="e884c-118">Create a new set object in a term [store].</span></span>|
|[<span data-ttu-id="e884c-119">Создание термина</span><span class="sxs-lookup"><span data-stu-id="e884c-119">Create term</span></span>](../api/termstore-term-post.md)|[<span data-ttu-id="e884c-120">Microsoft. Graph. Банк. Term</span><span class="sxs-lookup"><span data-stu-id="e884c-120">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="e884c-121">Создайте новый объект [Term] в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="e884c-121">Create a new [term] object in a term [store].</span></span>|
|[<span data-ttu-id="e884c-122">Получение набора</span><span class="sxs-lookup"><span data-stu-id="e884c-122">Get set</span></span>](../api/termstore-set-get.md)|[<span data-ttu-id="e884c-123">Microsoft. Graph. банка. Set</span><span class="sxs-lookup"><span data-stu-id="e884c-123">microsoft.graph.termStore.set</span></span>](../resources/termstore-set.md)| <span data-ttu-id="e884c-124">Получение объекта Set в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="e884c-124">Get a set object in a term [store].</span></span>|
|[<span data-ttu-id="e884c-125">Получение термина</span><span class="sxs-lookup"><span data-stu-id="e884c-125">Get term</span></span>](../api/termstore-term-get.md)|[<span data-ttu-id="e884c-126">Microsoft. Graph. Банк. Term</span><span class="sxs-lookup"><span data-stu-id="e884c-126">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)| <span data-ttu-id="e884c-127">Получение объекта [Term] в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="e884c-127">Get a [term] object in a term [store].</span></span>|
|[<span data-ttu-id="e884c-128">Набор обновлений</span><span class="sxs-lookup"><span data-stu-id="e884c-128">Update set</span></span>](../api/termstore-set-update.md)|[<span data-ttu-id="e884c-129">Microsoft. Graph. банка. Set</span><span class="sxs-lookup"><span data-stu-id="e884c-129">microsoft.graph.termStore.set</span></span>](../resources/termstore-set.md)|<span data-ttu-id="e884c-130">Обновление свойств объекта Set в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="e884c-130">Update the properties of a set object in a term [store].</span></span>|
|[<span data-ttu-id="e884c-131">Удаление набора</span><span class="sxs-lookup"><span data-stu-id="e884c-131">Delete set</span></span>](../api/termstore-set-delete.md)|<span data-ttu-id="e884c-132">Нет</span><span class="sxs-lookup"><span data-stu-id="e884c-132">None</span></span>|<span data-ttu-id="e884c-133">Удаляет объект set в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="e884c-133">Deletes a set object in a term [store].</span></span>|

## <a name="properties"></a><span data-ttu-id="e884c-134">Свойства</span><span class="sxs-lookup"><span data-stu-id="e884c-134">Properties</span></span>
|<span data-ttu-id="e884c-135">Свойство</span><span class="sxs-lookup"><span data-stu-id="e884c-135">Property</span></span>|<span data-ttu-id="e884c-136">Тип</span><span class="sxs-lookup"><span data-stu-id="e884c-136">Type</span></span>|<span data-ttu-id="e884c-137">Описание</span><span class="sxs-lookup"><span data-stu-id="e884c-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e884c-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e884c-138">createdDateTime</span></span>|<span data-ttu-id="e884c-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e884c-139">DateTimeOffset</span></span>|<span data-ttu-id="e884c-140">Дата и время создания набора.</span><span class="sxs-lookup"><span data-stu-id="e884c-140">Date and time of set creation.</span></span> <span data-ttu-id="e884c-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e884c-141">Read-only.</span></span>|
|<span data-ttu-id="e884c-142">description</span><span class="sxs-lookup"><span data-stu-id="e884c-142">description</span></span>|<span data-ttu-id="e884c-143">String</span><span class="sxs-lookup"><span data-stu-id="e884c-143">String</span></span>|<span data-ttu-id="e884c-144">Описание, содержащее сведения об использовании терминов.</span><span class="sxs-lookup"><span data-stu-id="e884c-144">Description giving details on the term usage.</span></span>|
|<span data-ttu-id="e884c-145">id</span><span class="sxs-lookup"><span data-stu-id="e884c-145">id</span></span>|<span data-ttu-id="e884c-146">Строка</span><span class="sxs-lookup"><span data-stu-id="e884c-146">String</span></span>|<span data-ttu-id="e884c-147">Уникальный идентификатор.</span><span class="sxs-lookup"><span data-stu-id="e884c-147">Unique identifier.</span></span> <span data-ttu-id="e884c-148">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e884c-148">Read-only.</span></span>|
|<span data-ttu-id="e884c-149">локализеднамес</span><span class="sxs-lookup"><span data-stu-id="e884c-149">localizedNames</span></span>|<span data-ttu-id="e884c-150">Коллекция [Microsoft. Graph. банка Microsoft. Graph. локализеднаме](../resources/termstore-localizedname.md)</span><span class="sxs-lookup"><span data-stu-id="e884c-150">[microsoft.graph.termStore.localizedName](../resources/termstore-localizedname.md) collection</span></span>|<span data-ttu-id="e884c-151">Имя набора для каждого Лангуажетаг.</span><span class="sxs-lookup"><span data-stu-id="e884c-151">Name of the set for each languageTag.</span></span>|
|<span data-ttu-id="e884c-152">properties</span><span class="sxs-lookup"><span data-stu-id="e884c-152">properties</span></span>|<span data-ttu-id="e884c-153">Коллекция [Microsoft. Graph. ключзначение](../resources/keyvalue.md)</span><span class="sxs-lookup"><span data-stu-id="e884c-153">[microsoft.graph.keyValue](../resources/keyvalue.md) collection</span></span>|<span data-ttu-id="e884c-154">Настраиваемые свойства для набора.</span><span class="sxs-lookup"><span data-stu-id="e884c-154">Custom properties for the set.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e884c-155">Связи</span><span class="sxs-lookup"><span data-stu-id="e884c-155">Relationships</span></span>
|<span data-ttu-id="e884c-156">Связь</span><span class="sxs-lookup"><span data-stu-id="e884c-156">Relationship</span></span>|<span data-ttu-id="e884c-157">Тип</span><span class="sxs-lookup"><span data-stu-id="e884c-157">Type</span></span>|<span data-ttu-id="e884c-158">Описание</span><span class="sxs-lookup"><span data-stu-id="e884c-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e884c-159">children</span><span class="sxs-lookup"><span data-stu-id="e884c-159">children</span></span>|<span data-ttu-id="e884c-160">Коллекция [Microsoft. Graph. Банк терминов Microsoft. Graph.](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="e884c-160">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="e884c-161">Дочерние термины набора в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="e884c-161">Children terms of set in term [store].</span></span>|
|<span data-ttu-id="e884c-162">парентграуп</span><span class="sxs-lookup"><span data-stu-id="e884c-162">parentGroup</span></span>|[<span data-ttu-id="e884c-163">Microsoft. Graph. Банк.</span><span class="sxs-lookup"><span data-stu-id="e884c-163">microsoft.graph.termStore.group</span></span>](../resources/termstore-group.md)|<span data-ttu-id="e884c-164">Родительская [Группа] , содержащая набор.</span><span class="sxs-lookup"><span data-stu-id="e884c-164">The parent [group] that contains the set.</span></span>|
|<span data-ttu-id="e884c-165">отношениях</span><span class="sxs-lookup"><span data-stu-id="e884c-165">relations</span></span>|<span data-ttu-id="e884c-166">Коллекция [Microsoft. Graph. Банк. relation](../resources/termstore-relation.md)</span><span class="sxs-lookup"><span data-stu-id="e884c-166">[microsoft.graph.termStore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="e884c-167">Указывает, какие термины были закреплены или повторно использованы непосредственно в наборе.</span><span class="sxs-lookup"><span data-stu-id="e884c-167">Indicates which terms have been pinned or reused directly under the set.</span></span>|
|<span data-ttu-id="e884c-168">терм</span><span class="sxs-lookup"><span data-stu-id="e884c-168">terms</span></span>|<span data-ttu-id="e884c-169">Коллекция [Microsoft. Graph. Банк терминов Microsoft. Graph.](../resources/termstore-term.md)</span><span class="sxs-lookup"><span data-stu-id="e884c-169">[microsoft.graph.termStore.term](../resources/termstore-term.md) collection</span></span>|<span data-ttu-id="e884c-170">Все термины в наборе.</span><span class="sxs-lookup"><span data-stu-id="e884c-170">All the terms under the set.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e884c-171">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e884c-171">JSON representation</span></span>
<span data-ttu-id="e884c-172">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e884c-172">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.set",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.set",
  "id": "String (identifier)",
  "localizedNames": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedName"
    }
  ],
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "properties": [
    {
      "@odata.type": "microsoft.graph.termStore.keyValue"
    }
  ]
}
```

[microsoft.graph.termStore.term]: termstore-term.md
[Microsoft. Graph. банка. Set]: termstore-set.md
[microsoft.graph.termStore.set]: termstore-set.md
[microsoft.graph.termStore.group]: termstore-group.md
[microsoft.graph.termStore.relation]: termstore-relation.md
[microsoft.graph.termStore.store]: termstore-store.md
[microsoft.graph.termStore.localizedName]: termstore-localizedname.md
[восстановлен]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md
[group]: ../resources/termstore-group.md
[set]: ../resources/termstore-set.md
[банком]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md


<!--
{
  "type": "#page.annotation",
  "description": "TermSet is the entity containing the particular taxonomy for a tenant",
  "keywords": "termSet,facet,resource",
  "section": "documentation",
  "tocPath": "TermSet",
  "tocBookmarks": {
    "Resources/termStore.set": "#"
  },
  "suppressions": []
}
-->
