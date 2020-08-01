---
title: Тип ресурса связи
description: Представляет связь между терминами в банке терминов.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: c4e12069ff50362a667a94aec28b715096616917
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/01/2020
ms.locfileid: "46539388"
---
# <a name="relation-resource-type"></a><span data-ttu-id="28564-103">Тип ресурса связи</span><span class="sxs-lookup"><span data-stu-id="28564-103">relation resource type</span></span>

<span data-ttu-id="28564-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="28564-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28564-105">Представляет связь между [терминами](../resources/termstore-term.md) в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="28564-105">Represents the relationship between [terms](../resources/termstore-term.md) in a term [store].</span></span> <span data-ttu-id="28564-106">В настоящее время поддерживаются два типа отношений: ПИН-код и повторное использование.</span><span class="sxs-lookup"><span data-stu-id="28564-106">Currently two types of relationships are supported: pin and reuse.</span></span> 

<span data-ttu-id="28564-107">В контактном отношении термин может быть закреплен под другим термином в другом наборе терминов.</span><span class="sxs-lookup"><span data-stu-id="28564-107">In a pin relationship, a term can be pinned under a different term in a different term set.</span></span> <span data-ttu-id="28564-108">В закрепленной связи новые дочерние элементы для термина можно добавить только в набор терминов, в котором был создан термин.</span><span class="sxs-lookup"><span data-stu-id="28564-108">In a pinned relationship, new children to the term can only be added in the term set in which the term was created.</span></span> <span data-ttu-id="28564-109">Любое изменение в иерархии под термином отражается на тех наборах, в которых термин был закреплен.</span><span class="sxs-lookup"><span data-stu-id="28564-109">Any change in the hierarchy under the term is reflected across the sets in which the term was pinned.</span></span> 

<span data-ttu-id="28564-110">Отношение повторного использования аналогично закрепленному отношению, за исключением того, что изменения повторно используемого термина можно выполнить из любой иерархии, в которой этот термин используется повторно.</span><span class="sxs-lookup"><span data-stu-id="28564-110">The reuse relationship is similar to the pinned relationship except that changes to the reused term can be made from any hierarchy in which the term is reused.</span></span> <span data-ttu-id="28564-111">Кроме того, изменение иерархии, выполненное для повторно используемого термина, не отражается в других наборах терминов, в которых термин используется повторно.</span><span class="sxs-lookup"><span data-stu-id="28564-111">Also, a change in hierarchy made to the reused term does not get reflected in the other term sets in which the term is reused.</span></span>

<span data-ttu-id="28564-112">Наследуется от [объекта Entity](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="28564-112">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="28564-113">Методы</span><span class="sxs-lookup"><span data-stu-id="28564-113">Methods</span></span>
|<span data-ttu-id="28564-114">Метод</span><span class="sxs-lookup"><span data-stu-id="28564-114">Method</span></span>|<span data-ttu-id="28564-115">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="28564-115">Return type</span></span>|<span data-ttu-id="28564-116">Описание</span><span class="sxs-lookup"><span data-stu-id="28564-116">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="28564-117">Список отношений</span><span class="sxs-lookup"><span data-stu-id="28564-117">List relations</span></span>](../api/termstore-term-list-relations.md)|<span data-ttu-id="28564-118">Коллекция [Microsoft. Graph. Банк. relation](../resources/termstore-relation.md)</span><span class="sxs-lookup"><span data-stu-id="28564-118">[microsoft.graph.termstore.relation](../resources/termstore-relation.md) collection</span></span>|<span data-ttu-id="28564-119">Получение списка объектов **relation** .</span><span class="sxs-lookup"><span data-stu-id="28564-119">Retrieve a list of **relation** objects.</span></span>|
|[<span data-ttu-id="28564-120">Создание отношения</span><span class="sxs-lookup"><span data-stu-id="28564-120">Create relation</span></span>](../api/termstore-relation-post.md)|[<span data-ttu-id="28564-121">Microsoft. Graph. Банк. отношение</span><span class="sxs-lookup"><span data-stu-id="28564-121">microsoft.graph.termstore.relation</span></span>](../resources/termstore-relation.md)|<span data-ttu-id="28564-122">Создание объекта **связи** .</span><span class="sxs-lookup"><span data-stu-id="28564-122">Create a new **relation** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="28564-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="28564-123">Properties</span></span>
|<span data-ttu-id="28564-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="28564-124">Property</span></span>|<span data-ttu-id="28564-125">Тип</span><span class="sxs-lookup"><span data-stu-id="28564-125">Type</span></span>|<span data-ttu-id="28564-126">Описание</span><span class="sxs-lookup"><span data-stu-id="28564-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28564-127">id</span><span class="sxs-lookup"><span data-stu-id="28564-127">id</span></span>|<span data-ttu-id="28564-128">String</span><span class="sxs-lookup"><span data-stu-id="28564-128">String</span></span>|<span data-ttu-id="28564-129">Идентификатор отношения.</span><span class="sxs-lookup"><span data-stu-id="28564-129">The ID of the relation.</span></span>|
|<span data-ttu-id="28564-130">Отношение</span><span class="sxs-lookup"><span data-stu-id="28564-130">relationship</span></span>|<span data-ttu-id="28564-131">String</span><span class="sxs-lookup"><span data-stu-id="28564-131">String</span></span>|<span data-ttu-id="28564-132">Тип отношения.</span><span class="sxs-lookup"><span data-stu-id="28564-132">The type of relation.</span></span> <span data-ttu-id="28564-133">Возможные значения: `pin`, `reuse`.</span><span class="sxs-lookup"><span data-stu-id="28564-133">Possible values are: `pin`, `reuse`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28564-134">Связи</span><span class="sxs-lookup"><span data-stu-id="28564-134">Relationships</span></span>
|<span data-ttu-id="28564-135">Связь</span><span class="sxs-lookup"><span data-stu-id="28564-135">Relationship</span></span>|<span data-ttu-id="28564-136">Тип</span><span class="sxs-lookup"><span data-stu-id="28564-136">Type</span></span>|<span data-ttu-id="28564-137">Описание</span><span class="sxs-lookup"><span data-stu-id="28564-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28564-138">фромтерм</span><span class="sxs-lookup"><span data-stu-id="28564-138">fromTerm</span></span>|[<span data-ttu-id="28564-139">Microsoft. Graph. Банк. Term</span><span class="sxs-lookup"><span data-stu-id="28564-139">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="28564-140">[Термин] "от" отношения.</span><span class="sxs-lookup"><span data-stu-id="28564-140">The from [term] of the relation.</span></span> <span data-ttu-id="28564-141">Термин, в котором определено отношение.</span><span class="sxs-lookup"><span data-stu-id="28564-141">The term from which the relationship is defined.</span></span> <span data-ttu-id="28564-142">Значение NULL указывает на то, что отношение напрямую с [набором].</span><span class="sxs-lookup"><span data-stu-id="28564-142">A null value would indicate the relation is directly with the [set].</span></span> |
|<span data-ttu-id="28564-143">set</span><span class="sxs-lookup"><span data-stu-id="28564-143">set</span></span>|[<span data-ttu-id="28564-144">Microsoft. Graph. банка. Set</span><span class="sxs-lookup"><span data-stu-id="28564-144">microsoft.graph.termStore.set</span></span>](../resources/termstore-set.md)|<span data-ttu-id="28564-145">[Набор] , в котором соотношение является релевантным.</span><span class="sxs-lookup"><span data-stu-id="28564-145">The [set] in which the relation is relevant.</span></span>|
|<span data-ttu-id="28564-146">тотерм</span><span class="sxs-lookup"><span data-stu-id="28564-146">toTerm</span></span>|[<span data-ttu-id="28564-147">Microsoft. Graph. Банк. Term</span><span class="sxs-lookup"><span data-stu-id="28564-147">microsoft.graph.termStore.term</span></span>](../resources/termstore-term.md)|<span data-ttu-id="28564-148">[Термин] "Кому" отношения.</span><span class="sxs-lookup"><span data-stu-id="28564-148">The to [term] of the relation.</span></span> <span data-ttu-id="28564-149">Термин, для которого определен реалтионшип.</span><span class="sxs-lookup"><span data-stu-id="28564-149">The term to which the realtionship is defined.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="28564-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="28564-150">JSON representation</span></span>
<span data-ttu-id="28564-151">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="28564-151">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.relation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.relation",
  "id": "String (identifier)",
  "relationship": "String"
}
```

[microsoft.graph.termStore.term]: termstore-term.md
[microsoft.graph.termStore.set]: termstore-set.md
[microsoft.graph.termStore.relations]: termstore-relation.md
[microsoft.graph.termStore.relation]: termstore-relation.md
[восстановлен]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md
[банком]: ../resources/termstore-term.md
[term]: ../resources/termstore-term.md
[set]: ../resources/termstore-set.md

<!--
{
  "type": "#page.annotation",
  "description": "TermRelation is the entity for mapping relations between different terms",
  "keywords": "termRelation,facet,resource",
  "section": "documentation",
  "tocPath": "TermRelation",
  "tocBookmarks": {
    "Resources/termStore.relation": "#"
  },
  "suppressions": []
}
-->
