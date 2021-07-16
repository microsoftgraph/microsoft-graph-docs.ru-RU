---
author: mohitpcad
title: Тип группового ресурса
doc_type: resourcePageType
description: Представляет группу, используемую в магазине терминов.
localization_priority: Normal
ms.prod: taxonomy
ms.openlocfilehash: ec2e9609b2de278d2596d42b18cae2fe450efd86
ms.sourcegitcommit: 73bbf84e6f5dbc8c3db8ed2c48cc5ab9ae3cff78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/16/2021
ms.locfileid: "53456361"
---
# <a name="group-resource-type"></a><span data-ttu-id="11c0f-103">Тип группового ресурса</span><span class="sxs-lookup"><span data-stu-id="11c0f-103">Group resource type</span></span>

<span data-ttu-id="11c0f-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="11c0f-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="11c0f-105">Представляет группу, используемую в магазине [терминов.](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="11c0f-105">Represents a group used in a term [store](../resources/termstore-store.md).</span></span> <span data-ttu-id="11c0f-106">Группа — это логическая иерархия, которая содержит коллекцию наборов под ней.</span><span class="sxs-lookup"><span data-stu-id="11c0f-106">A group is a logical hierarchy that contains a collection of sets under it.</span></span> 

<span data-ttu-id="11c0f-107">Наследует от [объекта](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="11c0f-107">Inherits from [entity](../resources/entity.md).</span></span>


## <a name="methods"></a><span data-ttu-id="11c0f-108">Методы</span><span class="sxs-lookup"><span data-stu-id="11c0f-108">Methods</span></span>

| <span data-ttu-id="11c0f-109">Метод</span><span class="sxs-lookup"><span data-stu-id="11c0f-109">Method</span></span>                                                   | <span data-ttu-id="11c0f-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="11c0f-110">Return type</span></span>       |    <span data-ttu-id="11c0f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="11c0f-111">Description</span></span>
|:---------------------------------------------------------|:------------------|:---------------------
| [<span data-ttu-id="11c0f-112">Создание группы</span><span class="sxs-lookup"><span data-stu-id="11c0f-112">Create group</span></span>](../api/termstore-group-post.md)                     | <span data-ttu-id="11c0f-113">[microsoft.graph.termStore.group]</span><span class="sxs-lookup"><span data-stu-id="11c0f-113">[microsoft.graph.termStore.group]</span></span> | <span data-ttu-id="11c0f-114">Создание группы в магазине [терминов.]</span><span class="sxs-lookup"><span data-stu-id="11c0f-114">Create a group in a term [store].</span></span>
| [<span data-ttu-id="11c0f-115">Получение группы</span><span class="sxs-lookup"><span data-stu-id="11c0f-115">Get group</span></span>](../api/termstore-group-get.md)                           | <span data-ttu-id="11c0f-116">[microsoft.graph.termStore.group]</span><span class="sxs-lookup"><span data-stu-id="11c0f-116">[microsoft.graph.termStore.group]</span></span> | <span data-ttu-id="11c0f-117">Извлечение данных группы в магазине [терминов.]</span><span class="sxs-lookup"><span data-stu-id="11c0f-117">Retrieve the data of a group in a term [store].</span></span>
| [<span data-ttu-id="11c0f-118">Удаление группы</span><span class="sxs-lookup"><span data-stu-id="11c0f-118">Delete group</span></span>](../api/termstore-group-delete.md)                     | <span data-ttu-id="11c0f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="11c0f-119">None</span></span> |  <span data-ttu-id="11c0f-120">Удаление группы в магазине [терминов].</span><span class="sxs-lookup"><span data-stu-id="11c0f-120">Delete a group in a term [store].</span></span>

## <a name="properties"></a><span data-ttu-id="11c0f-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="11c0f-121">Properties</span></span>

| <span data-ttu-id="11c0f-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="11c0f-122">Property</span></span>             | <span data-ttu-id="11c0f-123">Тип</span><span class="sxs-lookup"><span data-stu-id="11c0f-123">Type</span></span>               | <span data-ttu-id="11c0f-124">Описание</span><span class="sxs-lookup"><span data-stu-id="11c0f-124">Description</span></span>
|:---------------------|:-------------------|:------------------------------------
| <span data-ttu-id="11c0f-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="11c0f-125">createdDateTime</span></span>      | <span data-ttu-id="11c0f-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11c0f-126">DateTimeOffset</span></span>     | <span data-ttu-id="11c0f-127">Дата и время создания группы.</span><span class="sxs-lookup"><span data-stu-id="11c0f-127">Date and time of group creation.</span></span> <span data-ttu-id="11c0f-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="11c0f-128">Read-only.</span></span>
| <span data-ttu-id="11c0f-129">description</span><span class="sxs-lookup"><span data-stu-id="11c0f-129">description</span></span>          | <span data-ttu-id="11c0f-130">string</span><span class="sxs-lookup"><span data-stu-id="11c0f-130">string</span></span>             | <span data-ttu-id="11c0f-131">Описание с подробными сведениями об использовании термина.</span><span class="sxs-lookup"><span data-stu-id="11c0f-131">Description giving details on the term usage.</span></span>
| <span data-ttu-id="11c0f-132">id</span><span class="sxs-lookup"><span data-stu-id="11c0f-132">id</span></span>                   | <span data-ttu-id="11c0f-133">string</span><span class="sxs-lookup"><span data-stu-id="11c0f-133">string</span></span>             | <span data-ttu-id="11c0f-134">Уникальный идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="11c0f-134">Unique identifier of group.</span></span> <span data-ttu-id="11c0f-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="11c0f-135">Read-Only.</span></span>
| <span data-ttu-id="11c0f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="11c0f-136">displayName</span></span>          | <span data-ttu-id="11c0f-137">string</span><span class="sxs-lookup"><span data-stu-id="11c0f-137">string</span></span>             | <span data-ttu-id="11c0f-138">Имя группы.</span><span class="sxs-lookup"><span data-stu-id="11c0f-138">Name of group.</span></span>
| <span data-ttu-id="11c0f-139">scope</span><span class="sxs-lookup"><span data-stu-id="11c0f-139">scope</span></span>                | <span data-ttu-id="11c0f-140">string</span><span class="sxs-lookup"><span data-stu-id="11c0f-140">string</span></span>              | <span data-ttu-id="11c0f-141">Возвращает тип группы.</span><span class="sxs-lookup"><span data-stu-id="11c0f-141">Returns type of group.</span></span> <span data-ttu-id="11c0f-142">Возможные значения : "глобальный", "системный" и "siteCollection".</span><span class="sxs-lookup"><span data-stu-id="11c0f-142">Possible values are 'global', 'system' and 'siteCollection'.</span></span>
| <span data-ttu-id="11c0f-143">parentSiteId</span><span class="sxs-lookup"><span data-stu-id="11c0f-143">parentSiteId</span></span>         | <span data-ttu-id="11c0f-144">String</span><span class="sxs-lookup"><span data-stu-id="11c0f-144">string</span></span>             | <span data-ttu-id="11c0f-145">Id родительского сайта этой группы.</span><span class="sxs-lookup"><span data-stu-id="11c0f-145">Id of the parent site of this group.</span></span>

## <a name="relationships"></a><span data-ttu-id="11c0f-146">Связи</span><span class="sxs-lookup"><span data-stu-id="11c0f-146">Relationships</span></span>
| <span data-ttu-id="11c0f-147">Связь</span><span class="sxs-lookup"><span data-stu-id="11c0f-147">Relationship</span></span>       | <span data-ttu-id="11c0f-148">Тип</span><span class="sxs-lookup"><span data-stu-id="11c0f-148">Type</span></span>                        | <span data-ttu-id="11c0f-149">Описание</span><span class="sxs-lookup"><span data-stu-id="11c0f-149">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="11c0f-150">наборы</span><span class="sxs-lookup"><span data-stu-id="11c0f-150">sets</span></span>           | <span data-ttu-id="11c0f-151">[коллекция microsoft.graph.termStore.set][]</span><span class="sxs-lookup"><span data-stu-id="11c0f-151">[microsoft.graph.termStore.set][] collection</span></span> | <span data-ttu-id="11c0f-152">Все наборы в группе в магазине [терминов].</span><span class="sxs-lookup"><span data-stu-id="11c0f-152">All sets under the group in a term [store].</span></span>

## <a name="json-representation"></a><span data-ttu-id="11c0f-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="11c0f-153">JSON representation</span></span>

<span data-ttu-id="11c0f-154">Ниже приводится представление JSON **группового** ресурса.</span><span class="sxs-lookup"><span data-stu-id="11c0f-154">The following is a JSON representation of a **group** resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.group",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
```json
{
  "@odata.type": "#microsoft.graph.termStore.group",
  "id": "string",
  "createdDateTime": "string (timestamp)",
  "description": "string",
  "scope" : "microsoft.graph.termStore.groupScope",
  "displayName": "string",
  "parentSiteId" : "string"
}
```



[identitySet]: identitySet.md
[microsoft.graph.termStore.set]: termstore-set.md
[microsoft.graph.termStore.group]: termstore-group.md
[microsoft.graph.termStore.store]: termstore-store.md
[магазин]: ../resources/termstore-store.md
[store]: ../resources/termstore-store.md
[group]: ../resources/termstore-group.md
[set]: ../resources/termstore-set.md
<!--
{
  "type": "#page.annotation",
  "description": "TermGroup is the entity used for managing permissions for the termSets in termStore",
  "keywords": "termGroup,facet,resource",
  "section": "documentation",
  "tocPath": "TermGroup",
  "tocBookmarks": {
    "Resources/termStore.group&quot;: &quot;#"
  },
  "suppressions": []
}
-->


