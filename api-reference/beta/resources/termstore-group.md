---
author: mohitpcad
title: Тип ресурса Group
doc_type: resourcePageType
description: Представляет группу, используемую в банке терминов.
localization_priority: Normal
ms.prod: Sharepoint
ms.openlocfilehash: 121eba9bfdde52372ce4c03a3fe594eb931f620f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48057978"
---
# <a name="group-resource-type"></a><span data-ttu-id="6f2fe-103">Тип ресурса Group</span><span class="sxs-lookup"><span data-stu-id="6f2fe-103">Group resource type</span></span>

<span data-ttu-id="6f2fe-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="6f2fe-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


<span data-ttu-id="6f2fe-105">Представляет группу, используемую в [банке](../resources/termstore-store.md)терминов.</span><span class="sxs-lookup"><span data-stu-id="6f2fe-105">Represents a group used in a term [store](../resources/termstore-store.md).</span></span> <span data-ttu-id="6f2fe-106">Группа — это логическая иерархия, содержащая коллекцию наборов.</span><span class="sxs-lookup"><span data-stu-id="6f2fe-106">A group is a logical hierarchy that contains a collection of sets under it.</span></span> 

<span data-ttu-id="6f2fe-107">Наследуется от [объекта Entity](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="6f2fe-107">Inherits from [entity](../resources/entity.md).</span></span>


## <a name="methods"></a><span data-ttu-id="6f2fe-108">Методы</span><span class="sxs-lookup"><span data-stu-id="6f2fe-108">Methods</span></span>

| <span data-ttu-id="6f2fe-109">Метод</span><span class="sxs-lookup"><span data-stu-id="6f2fe-109">Method</span></span>                                                   | <span data-ttu-id="6f2fe-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="6f2fe-110">Return type</span></span>       |    <span data-ttu-id="6f2fe-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6f2fe-111">Description</span></span>
|:---------------------------------------------------------|:------------------|:---------------------
| [<span data-ttu-id="6f2fe-112">Создание группы</span><span class="sxs-lookup"><span data-stu-id="6f2fe-112">Create group</span></span>](../api/termstore-group-post.md)                     | <span data-ttu-id="6f2fe-113">[Microsoft. Graph. Банк.]</span><span class="sxs-lookup"><span data-stu-id="6f2fe-113">[microsoft.graph.termStore.group]</span></span> | <span data-ttu-id="6f2fe-114">Создайте группу в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="6f2fe-114">Create a group in a term [store].</span></span>
| [<span data-ttu-id="6f2fe-115">Получение группы</span><span class="sxs-lookup"><span data-stu-id="6f2fe-115">Get group</span></span>](../api/termstore-store-get-group.md)                           | <span data-ttu-id="6f2fe-116">[Microsoft. Graph. Банк.]</span><span class="sxs-lookup"><span data-stu-id="6f2fe-116">[microsoft.graph.termStore.group]</span></span> | <span data-ttu-id="6f2fe-117">Получение данных группы в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="6f2fe-117">Retrieve the data of a group in a term [store].</span></span>
| [<span data-ttu-id="6f2fe-118">Удаление группы</span><span class="sxs-lookup"><span data-stu-id="6f2fe-118">Delete group</span></span>](../api/termstore-group-delete.md)                     | <span data-ttu-id="6f2fe-119">Нет</span><span class="sxs-lookup"><span data-stu-id="6f2fe-119">None</span></span> |  <span data-ttu-id="6f2fe-120">Удаление группы в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="6f2fe-120">Delete a group in a term [store].</span></span>

## <a name="properties"></a><span data-ttu-id="6f2fe-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f2fe-121">Properties</span></span>

| <span data-ttu-id="6f2fe-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f2fe-122">Property</span></span>             | <span data-ttu-id="6f2fe-123">Тип</span><span class="sxs-lookup"><span data-stu-id="6f2fe-123">Type</span></span>               | <span data-ttu-id="6f2fe-124">Описание</span><span class="sxs-lookup"><span data-stu-id="6f2fe-124">Description</span></span>
|:---------------------|:-------------------|:------------------------------------
| <span data-ttu-id="6f2fe-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6f2fe-125">createdDateTime</span></span>      | <span data-ttu-id="6f2fe-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f2fe-126">DateTimeOffset</span></span>     | <span data-ttu-id="6f2fe-127">Дата и время создания группы.</span><span class="sxs-lookup"><span data-stu-id="6f2fe-127">Date and time of group creation.</span></span> <span data-ttu-id="6f2fe-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f2fe-128">Read-only.</span></span>
| <span data-ttu-id="6f2fe-129">description</span><span class="sxs-lookup"><span data-stu-id="6f2fe-129">description</span></span>          | <span data-ttu-id="6f2fe-130">string</span><span class="sxs-lookup"><span data-stu-id="6f2fe-130">string</span></span>             | <span data-ttu-id="6f2fe-131">Описание, содержащее сведения об использовании терминов.</span><span class="sxs-lookup"><span data-stu-id="6f2fe-131">Description giving details on the term usage.</span></span>
| <span data-ttu-id="6f2fe-132">id</span><span class="sxs-lookup"><span data-stu-id="6f2fe-132">id</span></span>                   | <span data-ttu-id="6f2fe-133">string</span><span class="sxs-lookup"><span data-stu-id="6f2fe-133">string</span></span>             | <span data-ttu-id="6f2fe-134">Уникальный идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="6f2fe-134">Unique identifier of group.</span></span> <span data-ttu-id="6f2fe-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="6f2fe-135">Read-Only.</span></span>
| <span data-ttu-id="6f2fe-136">displayName</span><span class="sxs-lookup"><span data-stu-id="6f2fe-136">displayName</span></span>          | <span data-ttu-id="6f2fe-137">string</span><span class="sxs-lookup"><span data-stu-id="6f2fe-137">string</span></span>             | <span data-ttu-id="6f2fe-138">Имя группы.</span><span class="sxs-lookup"><span data-stu-id="6f2fe-138">Name of group.</span></span>
| <span data-ttu-id="6f2fe-139">scope</span><span class="sxs-lookup"><span data-stu-id="6f2fe-139">scope</span></span>                | <span data-ttu-id="6f2fe-140">string</span><span class="sxs-lookup"><span data-stu-id="6f2fe-140">string</span></span>              | <span data-ttu-id="6f2fe-141">Возвращает тип группы.</span><span class="sxs-lookup"><span data-stu-id="6f2fe-141">Returns type of group.</span></span> <span data-ttu-id="6f2fe-142">Возможные значения: "Global", "System" и "siteCollection".</span><span class="sxs-lookup"><span data-stu-id="6f2fe-142">Possible values are 'global', 'system' and 'siteCollection'.</span></span>

## <a name="relationships"></a><span data-ttu-id="6f2fe-143">Связи</span><span class="sxs-lookup"><span data-stu-id="6f2fe-143">Relationships</span></span>
| <span data-ttu-id="6f2fe-144">Связь</span><span class="sxs-lookup"><span data-stu-id="6f2fe-144">Relationship</span></span>       | <span data-ttu-id="6f2fe-145">Тип</span><span class="sxs-lookup"><span data-stu-id="6f2fe-145">Type</span></span>                        | <span data-ttu-id="6f2fe-146">Описание</span><span class="sxs-lookup"><span data-stu-id="6f2fe-146">Description</span></span>
|:-------------------|:----------------------------|:--------------------------
| <span data-ttu-id="6f2fe-147">предваритель</span><span class="sxs-lookup"><span data-stu-id="6f2fe-147">sets</span></span>           | <span data-ttu-id="6f2fe-148">Коллекция [Microsoft. Graph. Банк. Set для Microsoft. Graph.][]</span><span class="sxs-lookup"><span data-stu-id="6f2fe-148">[microsoft.graph.termStore.set][] collection</span></span> | <span data-ttu-id="6f2fe-149">Все наборы в группе в [банке]терминов.</span><span class="sxs-lookup"><span data-stu-id="6f2fe-149">All sets under the group in a term [store].</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f2fe-150">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6f2fe-150">JSON representation</span></span>

<span data-ttu-id="6f2fe-151">Ниже представлено представление ресурса **Group** в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f2fe-151">The following is a JSON representation of a **group** resource.</span></span>
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
}
```



[identitySet]: identitySet.md
[Microsoft. Graph. банка. Set]: termstore-set.md
[microsoft.graph.termStore.set]: termstore-set.md
[Microsoft. Graph. Банк.]: termstore-group.md
[microsoft.graph.termStore.group]: termstore-group.md
[microsoft.graph.termStore.store]: termstore-store.md
[восстановлен]: ../resources/termstore-store.md
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


