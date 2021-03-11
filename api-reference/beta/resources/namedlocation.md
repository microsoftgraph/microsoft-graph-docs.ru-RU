---
title: тип ресурса namedLocation
description: Это базовый класс, который представляет расположение Azure Active Directory с именем. Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ae3ec6235259001a453bac50e45d2b142cdbaa8f
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722120"
---
# <a name="namedlocation-resource-type"></a><span data-ttu-id="55697-104">тип ресурса namedLocation</span><span class="sxs-lookup"><span data-stu-id="55697-104">namedLocation resource type</span></span>

<span data-ttu-id="55697-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55697-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55697-106">Это базовый класс, который представляет расположение Azure Active Directory с именем.</span><span class="sxs-lookup"><span data-stu-id="55697-106">This is the base class that represents an Azure Active Directory named location.</span></span> <span data-ttu-id="55697-107">Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.</span><span class="sxs-lookup"><span data-stu-id="55697-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

## <a name="methods"></a><span data-ttu-id="55697-108">Методы</span><span class="sxs-lookup"><span data-stu-id="55697-108">Methods</span></span>

| <span data-ttu-id="55697-109">Метод</span><span class="sxs-lookup"><span data-stu-id="55697-109">Method</span></span>       | <span data-ttu-id="55697-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="55697-110">Return Type</span></span> | <span data-ttu-id="55697-111">Описание</span><span class="sxs-lookup"><span data-stu-id="55697-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="55697-112">Список namedLocations</span><span class="sxs-lookup"><span data-stu-id="55697-112">List namedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="55697-113">[коллекция namedLocation](namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="55697-113">[namedLocation](namedLocation.md) collection</span></span> | <span data-ttu-id="55697-114">Получите все **объекты namedLocation** в организации.</span><span class="sxs-lookup"><span data-stu-id="55697-114">Get all the **namedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="55697-115">Get namedLocation</span><span class="sxs-lookup"><span data-stu-id="55697-115">Get namedLocation</span></span>](../api/namedlocation-get.md) | [<span data-ttu-id="55697-116">namedLocation</span><span class="sxs-lookup"><span data-stu-id="55697-116">namedLocation</span></span>](namedlocation.md) | <span data-ttu-id="55697-117">Ознакомьтесь с свойствами и отношениями объекта **с именемLocation.**</span><span class="sxs-lookup"><span data-stu-id="55697-117">Read the properties and relationships of a **namedLocation** object.</span></span> |
| [<span data-ttu-id="55697-118">Удаление namedLocation</span><span class="sxs-lookup"><span data-stu-id="55697-118">Delete namedLocation</span></span>](../api/namedlocation-delete.md) | <span data-ttu-id="55697-119">Нет</span><span class="sxs-lookup"><span data-stu-id="55697-119">None</span></span> | <span data-ttu-id="55697-120">Удаление **объекта namedLocation.**</span><span class="sxs-lookup"><span data-stu-id="55697-120">Delete a **namedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="55697-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="55697-121">Properties</span></span>

| <span data-ttu-id="55697-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="55697-122">Property</span></span>     | <span data-ttu-id="55697-123">Тип</span><span class="sxs-lookup"><span data-stu-id="55697-123">Type</span></span>        | <span data-ttu-id="55697-124">Описание</span><span class="sxs-lookup"><span data-stu-id="55697-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="55697-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="55697-125">createdDateTime</span></span>|<span data-ttu-id="55697-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55697-126">DateTimeOffset</span></span>|<span data-ttu-id="55697-127">Тип Timestamp представляет дату создания и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="55697-127">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="55697-128">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="55697-128">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="55697-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55697-129">Read-only.</span></span>|
|<span data-ttu-id="55697-130">displayName</span><span class="sxs-lookup"><span data-stu-id="55697-130">displayName</span></span>|<span data-ttu-id="55697-131">String</span><span class="sxs-lookup"><span data-stu-id="55697-131">String</span></span>|<span data-ttu-id="55697-132">Понятное человеку имя расположения.</span><span class="sxs-lookup"><span data-stu-id="55697-132">Human-readable name of the location.</span></span>|
|<span data-ttu-id="55697-133">id</span><span class="sxs-lookup"><span data-stu-id="55697-133">id</span></span>|<span data-ttu-id="55697-134">String</span><span class="sxs-lookup"><span data-stu-id="55697-134">String</span></span>|<span data-ttu-id="55697-135">Идентификатор объекта namedLocation.</span><span class="sxs-lookup"><span data-stu-id="55697-135">Identifier of a namedLocation object.</span></span> <span data-ttu-id="55697-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55697-136">Read-only.</span></span>|
|<span data-ttu-id="55697-137">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55697-137">modifiedDateTime</span></span>|<span data-ttu-id="55697-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55697-138">DateTimeOffset</span></span>|<span data-ttu-id="55697-139">Тип Timestamp представляет последнюю измененную дату и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="55697-139">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="55697-140">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="55697-140">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="55697-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="55697-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55697-142">Связи</span><span class="sxs-lookup"><span data-stu-id="55697-142">Relationships</span></span>

<span data-ttu-id="55697-143">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="55697-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="55697-144">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="55697-144">JSON representation</span></span>

<span data-ttu-id="55697-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="55697-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedLocation",
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


