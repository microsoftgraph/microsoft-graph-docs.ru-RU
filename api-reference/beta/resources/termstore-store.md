---
title: Тип ресурса хранилища
description: Представляет банк терминов таксономии.
author: mohitpcad
localization_priority: Normal
ms.prod: Sharepoint
doc_type: resourcePageType
ms.openlocfilehash: de8b0c004da804a4d9a617eec20de22c51e98108
ms.sourcegitcommit: b7e82d0d64f640a09f5da76b38d8ed9f13684f95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2020
ms.locfileid: "48258438"
---
# <a name="store-resource-type"></a><span data-ttu-id="2c64c-103">Тип ресурса хранилища</span><span class="sxs-lookup"><span data-stu-id="2c64c-103">store resource type</span></span>

<span data-ttu-id="2c64c-104">Пространство имен: Microsoft. Graph. банка</span><span class="sxs-lookup"><span data-stu-id="2c64c-104">Namespace: microsoft.graph.termStore</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2c64c-105">Представляет банк терминов таксономии.</span><span class="sxs-lookup"><span data-stu-id="2c64c-105">Represents a taxonomy term store.</span></span>

<span data-ttu-id="2c64c-106">Наследуется от [объекта Entity](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="2c64c-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="2c64c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="2c64c-107">Methods</span></span>
|<span data-ttu-id="2c64c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="2c64c-108">Method</span></span>|<span data-ttu-id="2c64c-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="2c64c-109">Return type</span></span>|<span data-ttu-id="2c64c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2c64c-110">Description</span></span>
|:---|:---|:---
|[<span data-ttu-id="2c64c-111">Перечисление групп</span><span class="sxs-lookup"><span data-stu-id="2c64c-111">List groups</span></span>](../api/termstore-list-groups.md)|<span data-ttu-id="2c64c-112">Коллекция [Microsoft. Graph. банка терминов Microsoft. Graph.](../resources/termstore-group.md)</span><span class="sxs-lookup"><span data-stu-id="2c64c-112">[microsoft.graph.termStore.group](../resources/termstore-group.md) collection</span></span>| <span data-ttu-id="2c64c-113">Получение групп из доступных в объекте банка терминов.</span><span class="sxs-lookup"><span data-stu-id="2c64c-113">Get the groups from available in the term store object.</span></span>|
|[<span data-ttu-id="2c64c-114">Получение хранилища</span><span class="sxs-lookup"><span data-stu-id="2c64c-114">Get store</span></span>](../api/termstore-store-get.md) | [<span data-ttu-id="2c64c-115">Microsoft. Graph. Банк. Банк.</span><span class="sxs-lookup"><span data-stu-id="2c64c-115">microsoft.graph.termStore.store</span></span>](../resources/termstore-store.md) | <span data-ttu-id="2c64c-116">Чтение свойств и связей объекта банка терминов.</span><span class="sxs-lookup"><span data-stu-id="2c64c-116">Read the properties and relationships of a term store object.</span></span>
|[<span data-ttu-id="2c64c-117">Обновление хранилища</span><span class="sxs-lookup"><span data-stu-id="2c64c-117">Update store</span></span>](../api/termstore-store-update.md) | [<span data-ttu-id="2c64c-118">Microsoft. Graph. Банк. Банк.</span><span class="sxs-lookup"><span data-stu-id="2c64c-118">microsoft.graph.termStore.store</span></span>](../resources/termstore-store.md) | <span data-ttu-id="2c64c-119">Обновление свойств объекта банка терминов.</span><span class="sxs-lookup"><span data-stu-id="2c64c-119">Update the properties of a term store object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2c64c-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="2c64c-120">Properties</span></span>
|<span data-ttu-id="2c64c-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="2c64c-121">Property</span></span>|<span data-ttu-id="2c64c-122">Тип</span><span class="sxs-lookup"><span data-stu-id="2c64c-122">Type</span></span>|<span data-ttu-id="2c64c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2c64c-123">Description</span></span>
|:---|:---|:---
|<span data-ttu-id="2c64c-124">дефаултлангуажетаг</span><span class="sxs-lookup"><span data-stu-id="2c64c-124">defaultLanguageTag</span></span> | <span data-ttu-id="2c64c-125">Строка</span><span class="sxs-lookup"><span data-stu-id="2c64c-125">String</span></span> | <span data-ttu-id="2c64c-126">Язык банка терминов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2c64c-126">Default language of the term store.</span></span>
|<span data-ttu-id="2c64c-127">id</span><span class="sxs-lookup"><span data-stu-id="2c64c-127">id</span></span>|<span data-ttu-id="2c64c-128">Строка</span><span class="sxs-lookup"><span data-stu-id="2c64c-128">String</span></span> | <span data-ttu-id="2c64c-129">Уникальный идентификатор банка терминов.</span><span class="sxs-lookup"><span data-stu-id="2c64c-129">Unique identifier of the term store.</span></span> <span data-ttu-id="2c64c-130">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="2c64c-130">Read-only.</span></span>
|<span data-ttu-id="2c64c-131">лангуажетагс</span><span class="sxs-lookup"><span data-stu-id="2c64c-131">languageTags</span></span> | <span data-ttu-id="2c64c-132">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="2c64c-132">String collection</span></span> | <span data-ttu-id="2c64c-133">Список языков для банка терминов.</span><span class="sxs-lookup"><span data-stu-id="2c64c-133">List of languages for the term store.</span></span>

## <a name="relationships"></a><span data-ttu-id="2c64c-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="2c64c-134">Relationships</span></span>
|<span data-ttu-id="2c64c-135">Связь</span><span class="sxs-lookup"><span data-stu-id="2c64c-135">Relationship</span></span>|<span data-ttu-id="2c64c-136">Тип</span><span class="sxs-lookup"><span data-stu-id="2c64c-136">Type</span></span>|<span data-ttu-id="2c64c-137">Описание</span><span class="sxs-lookup"><span data-stu-id="2c64c-137">Description</span></span>
|:---|:---|:---
|<span data-ttu-id="2c64c-138">groups</span><span class="sxs-lookup"><span data-stu-id="2c64c-138">groups</span></span> |<span data-ttu-id="2c64c-139">Коллекция [Microsoft. Graph. банка терминов Microsoft. Graph.](../resources/termstore-group.md)</span><span class="sxs-lookup"><span data-stu-id="2c64c-139">[microsoft.graph.termStore.group](../resources/termstore-group.md) collection</span></span> | <span data-ttu-id="2c64c-140">Коллекция всех групп, доступных в банке терминов.</span><span class="sxs-lookup"><span data-stu-id="2c64c-140">Collection of all groups available in the term store.</span></span>
|<span data-ttu-id="2c64c-141">предваритель</span><span class="sxs-lookup"><span data-stu-id="2c64c-141">sets</span></span> | <span data-ttu-id="2c64c-142">Коллекция [Microsoft. Graph. Банк. Set для Microsoft. Graph.](../resources/termstore-set.md)</span><span class="sxs-lookup"><span data-stu-id="2c64c-142">[microsoft.graph.termStore.set](../resources/termstore-set.md) collection</span></span> | <span data-ttu-id="2c64c-143">Коллекция всех наборов, доступных в банке терминов.</span><span class="sxs-lookup"><span data-stu-id="2c64c-143">Collection of all sets available in the term store.</span></span>


## <a name="json-representation"></a><span data-ttu-id="2c64c-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2c64c-144">JSON representation</span></span>
<span data-ttu-id="2c64c-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2c64c-145">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.store",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.store",
  "id": "String (identifier)",
  "defaultLanguageTag": "String",
  "languageTags": [
    "String"
  ]  
}
```

<!--
{
  "type": "#page.annotation",
  "description": "TermStore is the top-level entity used for managing taxonomy for a client",
  "keywords": "termStore,facet,resource",
  "section": "documentation",
  "tocPath": "TermStore",
  "tocBookmarks": {
    "Resources/termStore.store": "#"
  },
  "suppressions": []
}
-->



