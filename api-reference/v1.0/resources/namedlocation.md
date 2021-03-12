---
title: тип ресурса namedLocation
description: Это базовый класс, который представляет расположение Azure Active Directory с именем. Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9a454855a5f1048ddfeab89c85be25e02a26f82b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721910"
---
# <a name="namedlocation-resource-type"></a><span data-ttu-id="0035b-104">тип ресурса namedLocation</span><span class="sxs-lookup"><span data-stu-id="0035b-104">namedLocation resource type</span></span>

<span data-ttu-id="0035b-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0035b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0035b-106">Это базовый класс, который представляет расположение Azure Active Directory с именем.</span><span class="sxs-lookup"><span data-stu-id="0035b-106">This is the base class that represents an Azure Active Directory named location.</span></span> <span data-ttu-id="0035b-107">Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.</span><span class="sxs-lookup"><span data-stu-id="0035b-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

## <a name="methods"></a><span data-ttu-id="0035b-108">Методы</span><span class="sxs-lookup"><span data-stu-id="0035b-108">Methods</span></span>

| <span data-ttu-id="0035b-109">Метод</span><span class="sxs-lookup"><span data-stu-id="0035b-109">Method</span></span>       | <span data-ttu-id="0035b-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0035b-110">Return Type</span></span> | <span data-ttu-id="0035b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0035b-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0035b-112">Список namedLocations</span><span class="sxs-lookup"><span data-stu-id="0035b-112">List namedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="0035b-113">[коллекция namedLocation](namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="0035b-113">[namedLocation](namedLocation.md) collection</span></span> | <span data-ttu-id="0035b-114">Получите все **объекты namedLocation** в организации.</span><span class="sxs-lookup"><span data-stu-id="0035b-114">Get all the **namedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="0035b-115">Get namedLocation</span><span class="sxs-lookup"><span data-stu-id="0035b-115">Get namedLocation</span></span>](../api/namedlocation-get.md) | [<span data-ttu-id="0035b-116">namedLocation</span><span class="sxs-lookup"><span data-stu-id="0035b-116">namedLocation</span></span>](namedlocation.md) | <span data-ttu-id="0035b-117">Ознакомьтесь с свойствами и отношениями объекта **с именемLocation.**</span><span class="sxs-lookup"><span data-stu-id="0035b-117">Read the properties and relationships of a **namedLocation** object.</span></span> |
| [<span data-ttu-id="0035b-118">Удаление namedLocation</span><span class="sxs-lookup"><span data-stu-id="0035b-118">Delete namedLocation</span></span>](../api/namedlocation-delete.md) | <span data-ttu-id="0035b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="0035b-119">None</span></span> | <span data-ttu-id="0035b-120">Удаление **объекта namedLocation.**</span><span class="sxs-lookup"><span data-stu-id="0035b-120">Delete a **namedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0035b-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="0035b-121">Properties</span></span>

| <span data-ttu-id="0035b-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="0035b-122">Property</span></span>     | <span data-ttu-id="0035b-123">Тип</span><span class="sxs-lookup"><span data-stu-id="0035b-123">Type</span></span>        | <span data-ttu-id="0035b-124">Описание</span><span class="sxs-lookup"><span data-stu-id="0035b-124">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0035b-125">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0035b-125">createdDateTime</span></span>|<span data-ttu-id="0035b-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0035b-126">DateTimeOffset</span></span>|<span data-ttu-id="0035b-127">Тип Timestamp представляет дату создания и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="0035b-127">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0035b-128">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="0035b-128">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="0035b-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0035b-129">Read-only.</span></span>|
|<span data-ttu-id="0035b-130">displayName</span><span class="sxs-lookup"><span data-stu-id="0035b-130">displayName</span></span>|<span data-ttu-id="0035b-131">String</span><span class="sxs-lookup"><span data-stu-id="0035b-131">String</span></span>|<span data-ttu-id="0035b-132">Понятное человеку имя расположения.</span><span class="sxs-lookup"><span data-stu-id="0035b-132">Human-readable name of the location.</span></span>|
|<span data-ttu-id="0035b-133">id</span><span class="sxs-lookup"><span data-stu-id="0035b-133">id</span></span>|<span data-ttu-id="0035b-134">String</span><span class="sxs-lookup"><span data-stu-id="0035b-134">String</span></span>|<span data-ttu-id="0035b-135">Идентификатор объекта namedLocation.</span><span class="sxs-lookup"><span data-stu-id="0035b-135">Identifier of a namedLocation object.</span></span> <span data-ttu-id="0035b-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0035b-136">Read-only.</span></span>|
|<span data-ttu-id="0035b-137">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0035b-137">modifiedDateTime</span></span>|<span data-ttu-id="0035b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0035b-138">DateTimeOffset</span></span>|<span data-ttu-id="0035b-139">Тип Timestamp представляет последнюю измененную дату и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="0035b-139">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0035b-140">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="0035b-140">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="0035b-141">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0035b-141">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0035b-142">Связи</span><span class="sxs-lookup"><span data-stu-id="0035b-142">Relationships</span></span>

<span data-ttu-id="0035b-143">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0035b-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0035b-144">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="0035b-144">JSON representation</span></span>

<span data-ttu-id="0035b-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0035b-145">The following is a JSON representation of the resource.</span></span>

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

