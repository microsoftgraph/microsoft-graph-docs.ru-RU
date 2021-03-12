---
title: тип ресурса ipNamedLocation
description: Представляет расположение Azure Active Directory с именем, определенное диапазонами IP. Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1781c10e28e2d3efc28154cd15a8c36c9b43ac21
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719341"
---
# <a name="ipnamedlocation-resource-type"></a><span data-ttu-id="fe403-104">тип ресурса ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="fe403-104">ipNamedLocation resource type</span></span>

<span data-ttu-id="fe403-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe403-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe403-106">Представляет расположение Azure Active Directory с именем, определенное диапазонами IP.</span><span class="sxs-lookup"><span data-stu-id="fe403-106">Represents an Azure Active Directory named location defined by IP ranges.</span></span> <span data-ttu-id="fe403-107">Именуемые расположения — это настраиваемые правила, определяемые расположениями сети, которые затем можно использовать в политике условного доступа.</span><span class="sxs-lookup"><span data-stu-id="fe403-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="fe403-108">Наследует от [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="fe403-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="fe403-109">Методы</span><span class="sxs-lookup"><span data-stu-id="fe403-109">Methods</span></span>

| <span data-ttu-id="fe403-110">Метод</span><span class="sxs-lookup"><span data-stu-id="fe403-110">Method</span></span>       | <span data-ttu-id="fe403-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="fe403-111">Return Type</span></span> | <span data-ttu-id="fe403-112">Описание</span><span class="sxs-lookup"><span data-stu-id="fe403-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="fe403-113">Список ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="fe403-113">List ipNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="fe403-114">[коллекция ipNamedLocation](ipNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="fe403-114">[ipNamedLocation](ipNamedLocation.md) collection</span></span> | <span data-ttu-id="fe403-115">Получите все **объекты ipNamedLocation** в организации.</span><span class="sxs-lookup"><span data-stu-id="fe403-115">Get all the **ipNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="fe403-116">Создание ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="fe403-116">Create ipNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="fe403-117">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="fe403-117">ipNamedLocation</span></span>](ipNamedLocation.md) | <span data-ttu-id="fe403-118">Создание нового **объекта ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="fe403-118">Create a new **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="fe403-119">Get ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="fe403-119">Get ipNamedLocation</span></span>](../api/ipnamedlocation-get.md) | [<span data-ttu-id="fe403-120">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="fe403-120">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="fe403-121">Ознакомьтесь с свойствами и отношениями **объекта ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="fe403-121">Read the properties and relationships of an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="fe403-122">Обновление ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="fe403-122">Update ipNamedLocation</span></span>](../api/ipnamedlocation-update.md) | [<span data-ttu-id="fe403-123">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="fe403-123">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="fe403-124">Обновление **объекта ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="fe403-124">Update an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="fe403-125">Удаление ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="fe403-125">Delete ipNamedLocation</span></span>](../api/ipnamedlocation-delete.md) | <span data-ttu-id="fe403-126">Нет</span><span class="sxs-lookup"><span data-stu-id="fe403-126">None</span></span> | <span data-ttu-id="fe403-127">Удаление **объекта ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="fe403-127">Delete an **ipNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="fe403-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe403-128">Properties</span></span>

| <span data-ttu-id="fe403-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe403-129">Property</span></span>     | <span data-ttu-id="fe403-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fe403-130">Type</span></span>        | <span data-ttu-id="fe403-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fe403-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fe403-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe403-132">createdDateTime</span></span>|<span data-ttu-id="fe403-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe403-133">DateTimeOffset</span></span>|<span data-ttu-id="fe403-134">Тип Timestamp представляет дату создания и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="fe403-134">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fe403-135">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="fe403-135">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="fe403-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe403-136">Read-only.</span></span> <span data-ttu-id="fe403-137">Наследуется [от namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="fe403-137">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="fe403-138">displayName</span><span class="sxs-lookup"><span data-stu-id="fe403-138">displayName</span></span>|<span data-ttu-id="fe403-139">String</span><span class="sxs-lookup"><span data-stu-id="fe403-139">String</span></span>|<span data-ttu-id="fe403-140">Понятное человеку имя расположения.</span><span class="sxs-lookup"><span data-stu-id="fe403-140">Human-readable name of the location.</span></span>|
|<span data-ttu-id="fe403-141">id</span><span class="sxs-lookup"><span data-stu-id="fe403-141">id</span></span>|<span data-ttu-id="fe403-142">String</span><span class="sxs-lookup"><span data-stu-id="fe403-142">String</span></span>|<span data-ttu-id="fe403-143">Идентификатор объекта namedLocation.</span><span class="sxs-lookup"><span data-stu-id="fe403-143">Identifier of a namedLocation object.</span></span> <span data-ttu-id="fe403-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe403-144">Read-only.</span></span> <span data-ttu-id="fe403-145">Наследуется [от namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="fe403-145">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="fe403-146">ipRanges</span><span class="sxs-lookup"><span data-stu-id="fe403-146">ipRanges</span></span>|<span data-ttu-id="fe403-147">Коллекция объектов [ipRange](iprange.md)</span><span class="sxs-lookup"><span data-stu-id="fe403-147">[ipRange](iprange.md) collection</span></span>|<span data-ttu-id="fe403-148">Список диапазонов IP-адресов в формате CIDR IPv4 (например, 1.2.3.4/32) или любого допустимого формата IPv6 от IETF RFC596.</span><span class="sxs-lookup"><span data-stu-id="fe403-148">List of IP address ranges in IPv4 CIDR format (e.g. 1.2.3.4/32) or any allowable IPv6 format from IETF RFC596.</span></span>|
|<span data-ttu-id="fe403-149">isTrusted</span><span class="sxs-lookup"><span data-stu-id="fe403-149">isTrusted</span></span>|<span data-ttu-id="fe403-150">Логический</span><span class="sxs-lookup"><span data-stu-id="fe403-150">Boolean</span></span>|<span data-ttu-id="fe403-151">True, если это расположение явно доверяется.</span><span class="sxs-lookup"><span data-stu-id="fe403-151">True if this location is explicitly trusted.</span></span>|
|<span data-ttu-id="fe403-152">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe403-152">modifiedDateTime</span></span>|<span data-ttu-id="fe403-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe403-153">DateTimeOffset</span></span>|<span data-ttu-id="fe403-154">Тип Timestamp представляет последнюю измененную дату и время расположения с помощью формата ISO 8601 и всегда находится во времени UTC.</span><span class="sxs-lookup"><span data-stu-id="fe403-154">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fe403-155">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="fe403-155">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="fe403-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fe403-156">Read-only.</span></span> <span data-ttu-id="fe403-157">Наследуется [от namedLocation](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="fe403-157">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe403-158">Связи</span><span class="sxs-lookup"><span data-stu-id="fe403-158">Relationships</span></span>

<span data-ttu-id="fe403-159">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fe403-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe403-160">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fe403-160">JSON representation</span></span>

<span data-ttu-id="fe403-161">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe403-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ipNamedLocation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "ipRanges": [{"@odata.type": "microsoft.graph.ipRange"}],
  "isTrusted": true,
  "modifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "ipNamedLocation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

