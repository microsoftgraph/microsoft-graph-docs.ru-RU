---
author: mohitpcad
title: Тип группового ресурса
doc_type: resourcePageType
description: Представляет группу, используемую в магазине терминов.
localization_priority: Normal
ms.prod: Sharepoint
ms.openlocfilehash: 1249f94b96e0c6ff7251a2a97f4885a21258aaeb
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473467"
---
# <a name="group-resource-type"></a><span data-ttu-id="cb5b8-103">Тип группового ресурса</span><span class="sxs-lookup"><span data-stu-id="cb5b8-103">Group resource type</span></span>

<span data-ttu-id="cb5b8-104">Пространство имен: microsoft.graph.termStore</span><span class="sxs-lookup"><span data-stu-id="cb5b8-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="cb5b8-105">Представляет группу, используемую в магазине [терминов.](../resources/termstore-store.md)</span><span class="sxs-lookup"><span data-stu-id="cb5b8-105">Represents a group used in a term [store](../resources/termstore-store.md).</span></span> <span data-ttu-id="cb5b8-106">Группа — это логическая иерархия, которая содержит коллекцию наборов под ней.</span><span class="sxs-lookup"><span data-stu-id="cb5b8-106">A group is a logical hierarchy that contains a collection of sets under it.</span></span> 

<span data-ttu-id="cb5b8-107">Наследует от [объекта](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="cb5b8-107">Inherits from [entity](../resources/entity.md).</span></span>


## <a name="methods"></a><span data-ttu-id="cb5b8-108">Методы</span><span class="sxs-lookup"><span data-stu-id="cb5b8-108">Methods</span></span>

| <span data-ttu-id="cb5b8-109">Метод</span><span class="sxs-lookup"><span data-stu-id="cb5b8-109">Method</span></span>                                                   | <span data-ttu-id="cb5b8-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="cb5b8-110">Return type</span></span>       |    <span data-ttu-id="cb5b8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cb5b8-111">Description</span></span>
|:---------------------------------------------------------|:------------------|:---------------------
| [<span data-ttu-id="cb5b8-112">Создание группы</span><span class="sxs-lookup"><span data-stu-id="cb5b8-112">Create group</span></span>](../api/termstore-group-post.md)                     | <span data-ttu-id="cb5b8-113">[microsoft.graph.termStore.group]</span><span class="sxs-lookup"><span data-stu-id="cb5b8-113">[microsoft.graph.termStore.group]</span></span> | <span data-ttu-id="cb5b8-114">Создание группы в магазине [терминов.]</span><span class="sxs-lookup"><span data-stu-id="cb5b8-114">Create a group in a term [store].</span></span>
| [<span data-ttu-id="cb5b8-115">Получение группы</span><span class="sxs-lookup"><span data-stu-id="cb5b8-115">Get group</span></span>](../api/termstore-store-get-group.md)                           | <span data-ttu-id="cb5b8-116">[microsoft.graph.termStore.group]</span><span class="sxs-lookup"><span data-stu-id="cb5b8-116">[microsoft.graph.termStore.group]</span></span> | <span data-ttu-id="cb5b8-117">Извлечение данных группы в магазине [терминов.]</span><span class="sxs-lookup"><span data-stu-id="cb5b8-117">Retrieve the data of a group in a term [store].</span></span>
| [<span data-ttu-id="cb5b8-118">Удаление группы</span><span class="sxs-lookup"><span data-stu-id="cb5b8-118">Delete group</span></span>](../api/termstore-group-delete.md)                     | <span data-ttu-id="cb5b8-119">Нет</span><span class="sxs-lookup"><span data-stu-id="cb5b8-119">None</span></span> |  <span data-ttu-id="cb5b8-120">Удаление группы в магазине [терминов].</span><span class="sxs-lookup"><span data-stu-id="cb5b8-120">Delete a group in a term [store].</span></span>

## <a name="properties"></a><span data-ttu-id="cb5b8-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="cb5b8-121">Properties</span></span>

| <span data-ttu-id="cb5b8-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="cb5b8-122">Property</span></span>             | <span data-ttu-id="cb5b8-123">Тип</span><span class="sxs-lookup"><span data-stu-id="cb5b8-123">Type</span></span>               | <span data-ttu-id="cb5b8-124">Описание</span><span class="sxs-lookup"><span data-stu-id="cb5b8-124">Description</span></span>
|:---------------------|:-------------------|:------------------------------------
| <span data-ttu-id="cb5b8-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb5b8-125">createdDateTime</span></span>      | <span data-ttu-id="cb5b8-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb5b8-126">DateTimeOffset</span></span>     | <span data-ttu-id="cb5b8-127">Дата и время создания группы.</span><span class="sxs-lookup"><span data-stu-id="cb5b8-127">Date and time of group creation.</span></span> <span data-ttu-id="cb5b8-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb5b8-128">Read-only.</span></span>
| <span data-ttu-id="cb5b8-129">description</span><span class="sxs-lookup"><span data-stu-id="cb5b8-129">description</span></span>          | <span data-ttu-id="cb5b8-130">string</span><span class="sxs-lookup"><span data-stu-id="cb5b8-130">string</span></span>             | <span data-ttu-id="cb5b8-131">Описание с подробными сведениями об использовании термина.</span><span class="sxs-lookup"><span data-stu-id="cb5b8-131">Description giving details on the term usage.</span></span>
| <span data-ttu-id="cb5b8-132">id</span><span class="sxs-lookup"><span data-stu-id="cb5b8-132">id</span></span>                   | <span data-ttu-id="cb5b8-133">string</span><span class="sxs-lookup"><span data-stu-id="cb5b8-133">string</span></span>             | <span data-ttu-id="cb5b8-134">Уникальный идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="cb5b8-134">Unique identifier of group.</span></span> <span data-ttu-id="cb5b8-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="cb5b8-135">Read-Only.</span></span>
| <span data-ttu-id="cb5b8-136">displayName</span><span class="sxs-lookup"><span data-stu-id="cb5b8-136">displayName</span></span>          | <span data-ttu-id="cb5b8-137">string</span><span class="sxs-lookup"><span data-stu-id="cb5b8-137">string</span></span>             | <span data-ttu-id="cb5b8-138">Имя группы.</span><span class="sxs-lookup"><span data-stu-id="cb5b8-138">Name of group.</span></span>
| <span data-ttu-id="cb5b8-139">scope</span><span class="sxs-lookup"><span data-stu-id="cb5b8-139">scope</span></span>                | <span data-ttu-id="cb5b8-140">string</span><span class="sxs-lookup"><span data-stu-id="cb5b8-140">string</span></span>              | <span data-ttu-id="cb5b8-141">Возвращает тип группы.</span><span class="sxs-lookup"><span data-stu-id="cb5b8-141">Returns type of group.</span></span> <span data-ttu-id="cb5b8-142">Возможные значения : "глобальный", "системный" и "siteCollection".</span><span class="sxs-lookup"><span data-stu-id="cb5b8-142">Possible values are 'global', 'system' and 'siteCollection'.</span></span>
| <span data-ttu-id="cb5b8-143">parentSiteId</span><span class="sxs-lookup"><span data-stu-id="cb5b8-143">parentSiteId</span></span>         | <span data-ttu-id="cb5b8-144">Строка</span><span class="sxs-lookup"><span data-stu-id="cb5b8-144">string</span></span>             | <span data-ttu-id="cb5b8-145">Id родительского сайта этой группы.</span><span class="sxs-lookup"><span data-stu-id="cb5b8-145">Id of the parent site of this group.</span></span>

## <a name="relationships"></a><span data-ttu-id="cb5b8-146">Связи</span><span class="sxs-lookup"><span data-stu-id="cb5b8-146">Relationships</span></span>
| <span data-ttu-id="cb5b8-147">Связь</span><span class="sxs-lookup"><span data-stu-id="cb5b8-147">Relationship</span></span>       | <span data-ttu-id="cb5b8-148">Тип</span><span class="sxs-lookup"><span data-stu-id="cb5b8-148">Type</span></span>                        | <span data-ttu-id="cb5b8-149">Описание</span><span class="sxs-lookup"><span data-stu-id="cb5b8-149">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="cb5b8-150">наборы</span><span class="sxs-lookup"><span data-stu-id="cb5b8-150">sets</span></span>           | <span data-ttu-id="cb5b8-151">[коллекция microsoft.graph.termStore.set][]</span><span class="sxs-lookup"><span data-stu-id="cb5b8-151">[microsoft.graph.termStore.set][] collection</span></span> | <span data-ttu-id="cb5b8-152">Все наборы в группе в магазине [терминов].</span><span class="sxs-lookup"><span data-stu-id="cb5b8-152">All sets under the group in a term [store].</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb5b8-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cb5b8-153">JSON representation</span></span>

<span data-ttu-id="cb5b8-154">Ниже приводится представление JSON **группового** ресурса.</span><span class="sxs-lookup"><span data-stu-id="cb5b8-154">The following is a JSON representation of a **group** resource.</span></span>
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
    "Resources/termStore.group": "#"
  },
  "suppressions": []
}
-->


