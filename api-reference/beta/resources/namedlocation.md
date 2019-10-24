---
title: Тип ресурса Намедлокатион
description: Это базовый класс, представляющий имя расположения Azure Active Directory. Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3f1e0b7c86a8b2c026c44b46fd833594aadad5a9
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653855"
---
# <a name="namedlocation-resource-type"></a><span data-ttu-id="9e6ce-104">Тип ресурса Намедлокатион</span><span class="sxs-lookup"><span data-stu-id="9e6ce-104">namedLocation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e6ce-105">Это базовый класс, представляющий имя расположения Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9e6ce-105">This is the base class that represents an Azure Active Directory named location.</span></span> <span data-ttu-id="9e6ce-106">Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.</span><span class="sxs-lookup"><span data-stu-id="9e6ce-106">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

## <a name="methods"></a><span data-ttu-id="9e6ce-107">Методы</span><span class="sxs-lookup"><span data-stu-id="9e6ce-107">Methods</span></span>

| <span data-ttu-id="9e6ce-108">Метод</span><span class="sxs-lookup"><span data-stu-id="9e6ce-108">Method</span></span>       | <span data-ttu-id="9e6ce-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9e6ce-109">Return Type</span></span> | <span data-ttu-id="9e6ce-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9e6ce-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9e6ce-111">Список Намедлокатионс</span><span class="sxs-lookup"><span data-stu-id="9e6ce-111">List namedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="9e6ce-112">Коллекция [намедлокатион](namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="9e6ce-112">[namedLocation](namedLocation.md) collection</span></span> | <span data-ttu-id="9e6ce-113">Получение всех объектов **намедлокатион** в Организации.</span><span class="sxs-lookup"><span data-stu-id="9e6ce-113">Get all the **namedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="9e6ce-114">Получение Намедлокатион</span><span class="sxs-lookup"><span data-stu-id="9e6ce-114">Get namedLocation</span></span>](../api/namedlocation-get.md) | [<span data-ttu-id="9e6ce-115">намедлокатион</span><span class="sxs-lookup"><span data-stu-id="9e6ce-115">namedLocation</span></span>](namedlocation.md) | <span data-ttu-id="9e6ce-116">Чтение свойств и связей объекта **намедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="9e6ce-116">Read the properties and relationships of a **namedLocation** object.</span></span> |
| [<span data-ttu-id="9e6ce-117">Удаление Намедлокатион</span><span class="sxs-lookup"><span data-stu-id="9e6ce-117">Delete namedLocation</span></span>](../api/namedlocation-delete.md) | <span data-ttu-id="9e6ce-118">Нет</span><span class="sxs-lookup"><span data-stu-id="9e6ce-118">None</span></span> | <span data-ttu-id="9e6ce-119">Удаление объекта **намедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="9e6ce-119">Delete a **namedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9e6ce-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e6ce-120">Properties</span></span>

| <span data-ttu-id="9e6ce-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e6ce-121">Property</span></span>     | <span data-ttu-id="9e6ce-122">Тип</span><span class="sxs-lookup"><span data-stu-id="9e6ce-122">Type</span></span>        | <span data-ttu-id="9e6ce-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9e6ce-123">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9e6ce-124">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e6ce-124">createdDateTime</span></span>|<span data-ttu-id="9e6ce-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e6ce-125">DateTimeOffset</span></span>|<span data-ttu-id="9e6ce-126">Тип timestamp представляет дату и время создания расположения с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="9e6ce-126">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9e6ce-127">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9e6ce-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="9e6ce-128">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9e6ce-128">Read-only.</span></span>|
|<span data-ttu-id="9e6ce-129">displayName</span><span class="sxs-lookup"><span data-stu-id="9e6ce-129">displayName</span></span>|<span data-ttu-id="9e6ce-130">Строка</span><span class="sxs-lookup"><span data-stu-id="9e6ce-130">String</span></span>|<span data-ttu-id="9e6ce-131">Удобное для человека имя расположения.</span><span class="sxs-lookup"><span data-stu-id="9e6ce-131">Human-readable name of the location.</span></span>|
|<span data-ttu-id="9e6ce-132">id</span><span class="sxs-lookup"><span data-stu-id="9e6ce-132">id</span></span>|<span data-ttu-id="9e6ce-133">String</span><span class="sxs-lookup"><span data-stu-id="9e6ce-133">String</span></span>|<span data-ttu-id="9e6ce-134">Идентификатор объекта Намедлокатион.</span><span class="sxs-lookup"><span data-stu-id="9e6ce-134">Identifier of a namedLocation object.</span></span> <span data-ttu-id="9e6ce-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9e6ce-135">Read-only.</span></span>|
|<span data-ttu-id="9e6ce-136">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e6ce-136">modifiedDateTime</span></span>|<span data-ttu-id="9e6ce-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e6ce-137">DateTimeOffset</span></span>|<span data-ttu-id="9e6ce-138">Тип timestamp представляет дату и время последнего изменения расположения с использованием формата ISO 8601, которое всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="9e6ce-138">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9e6ce-139">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="9e6ce-139">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="9e6ce-140">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9e6ce-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e6ce-141">Отношения</span><span class="sxs-lookup"><span data-stu-id="9e6ce-141">Relationships</span></span>

<span data-ttu-id="9e6ce-142">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9e6ce-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e6ce-143">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9e6ce-143">JSON representation</span></span>

<span data-ttu-id="9e6ce-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e6ce-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedLocation",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "namedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
