---
title: Тип ресурса ipNamedLocation
description: Представляет именуемую позицию Azure Active Directory, определяемую диапазонами IP-адресов. Именуемые расположения — это настраиваемые правила, которые определяют сетевые расположения, которые затем можно использовать в политике условного доступа.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b63452ca6eefb9ad3a0d4b3f860fb1a8d41638fb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158403"
---
# <a name="ipnamedlocation-resource-type"></a><span data-ttu-id="021e0-104">Тип ресурса ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="021e0-104">ipNamedLocation resource type</span></span>

<span data-ttu-id="021e0-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="021e0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="021e0-106">Представляет именуемую позицию Azure Active Directory, определяемую диапазонами IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="021e0-106">Represents an Azure Active Directory named location defined by IP ranges.</span></span> <span data-ttu-id="021e0-107">Именуемые расположения — это настраиваемые правила, которые определяют сетевые расположения, которые затем можно использовать в политике условного доступа.</span><span class="sxs-lookup"><span data-stu-id="021e0-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="021e0-108">Наследуется от [namedLocation](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="021e0-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="021e0-109">Методы</span><span class="sxs-lookup"><span data-stu-id="021e0-109">Methods</span></span>

| <span data-ttu-id="021e0-110">Метод</span><span class="sxs-lookup"><span data-stu-id="021e0-110">Method</span></span>       | <span data-ttu-id="021e0-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="021e0-111">Return Type</span></span> | <span data-ttu-id="021e0-112">Описание</span><span class="sxs-lookup"><span data-stu-id="021e0-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="021e0-113">Список ipNamedLocations</span><span class="sxs-lookup"><span data-stu-id="021e0-113">List ipNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="021e0-114">[Коллекция ipNamedLocation](ipNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="021e0-114">[ipNamedLocation](ipNamedLocation.md) collection</span></span> | <span data-ttu-id="021e0-115">Получить все **объекты ipNamedLocation** в организации.</span><span class="sxs-lookup"><span data-stu-id="021e0-115">Get all the **ipNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="021e0-116">Создание ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="021e0-116">Create ipNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="021e0-117">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="021e0-117">ipNamedLocation</span></span>](ipNamedLocation.md) | <span data-ttu-id="021e0-118">Создание объекта **ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="021e0-118">Create a new **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="021e0-119">Get ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="021e0-119">Get ipNamedLocation</span></span>](../api/ipnamedlocation-get.md) | [<span data-ttu-id="021e0-120">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="021e0-120">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="021e0-121">Чтение свойств и связей объекта **ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="021e0-121">Read the properties and relationships of an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="021e0-122">Обновление ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="021e0-122">Update ipNamedLocation</span></span>](../api/ipnamedlocation-update.md) | [<span data-ttu-id="021e0-123">ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="021e0-123">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="021e0-124">Обновление объекта **ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="021e0-124">Update an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="021e0-125">Удаление ipNamedLocation</span><span class="sxs-lookup"><span data-stu-id="021e0-125">Delete ipNamedLocation</span></span>](../api/ipnamedlocation-delete.md) | <span data-ttu-id="021e0-126">Нет</span><span class="sxs-lookup"><span data-stu-id="021e0-126">None</span></span> | <span data-ttu-id="021e0-127">Удаление объекта **ipNamedLocation.**</span><span class="sxs-lookup"><span data-stu-id="021e0-127">Delete an **ipNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="021e0-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="021e0-128">Properties</span></span>

| <span data-ttu-id="021e0-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="021e0-129">Property</span></span>     | <span data-ttu-id="021e0-130">Тип</span><span class="sxs-lookup"><span data-stu-id="021e0-130">Type</span></span>        | <span data-ttu-id="021e0-131">Описание</span><span class="sxs-lookup"><span data-stu-id="021e0-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="021e0-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="021e0-132">createdDateTime</span></span>|<span data-ttu-id="021e0-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="021e0-133">DateTimeOffset</span></span>|<span data-ttu-id="021e0-134">Тип Timestamp представляет дату и время создания расположения в формате ISO 8601 и всегда используется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="021e0-134">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="021e0-135">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="021e0-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="021e0-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="021e0-136">Read-only.</span></span> <span data-ttu-id="021e0-137">Наследуется [от namedLocation.](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="021e0-137">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="021e0-138">displayName</span><span class="sxs-lookup"><span data-stu-id="021e0-138">displayName</span></span>|<span data-ttu-id="021e0-139">String</span><span class="sxs-lookup"><span data-stu-id="021e0-139">String</span></span>|<span data-ttu-id="021e0-140">Понятное человеку имя расположения.</span><span class="sxs-lookup"><span data-stu-id="021e0-140">Human-readable name of the location.</span></span>|
|<span data-ttu-id="021e0-141">id</span><span class="sxs-lookup"><span data-stu-id="021e0-141">id</span></span>|<span data-ttu-id="021e0-142">String</span><span class="sxs-lookup"><span data-stu-id="021e0-142">String</span></span>|<span data-ttu-id="021e0-143">Идентификатор объекта namedLocation.</span><span class="sxs-lookup"><span data-stu-id="021e0-143">Identifier of a namedLocation object.</span></span> <span data-ttu-id="021e0-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="021e0-144">Read-only.</span></span> <span data-ttu-id="021e0-145">Наследуется [от namedLocation.](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="021e0-145">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="021e0-146">ipRanges</span><span class="sxs-lookup"><span data-stu-id="021e0-146">ipRanges</span></span>|<span data-ttu-id="021e0-147">Коллекция объектов [ipRange](iprange.md)</span><span class="sxs-lookup"><span data-stu-id="021e0-147">[ipRange](iprange.md) collection</span></span>|<span data-ttu-id="021e0-148">Список диапазонов IP-адресов в формате IPv4 CIDR (например, 1.2.3.4/32) или любой допустимый формат IPv6 из IETF RFC596.</span><span class="sxs-lookup"><span data-stu-id="021e0-148">List of IP address ranges in IPv4 CIDR format (e.g. 1.2.3.4/32) or any allowable IPv6 format from IETF RFC596.</span></span>|
|<span data-ttu-id="021e0-149">isTrusted</span><span class="sxs-lookup"><span data-stu-id="021e0-149">isTrusted</span></span>|<span data-ttu-id="021e0-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="021e0-150">Boolean</span></span>|<span data-ttu-id="021e0-151">Имеет true, если это расположение является явным доверенным.</span><span class="sxs-lookup"><span data-stu-id="021e0-151">True if this location is explicitly trusted.</span></span>|
|<span data-ttu-id="021e0-152">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="021e0-152">modifiedDateTime</span></span>|<span data-ttu-id="021e0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="021e0-153">DateTimeOffset</span></span>|<span data-ttu-id="021e0-154">Тип Timestamp представляет дату и время последнего изменения расположения в формате ISO 8601 и всегда используется в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="021e0-154">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="021e0-155">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="021e0-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="021e0-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="021e0-156">Read-only.</span></span> <span data-ttu-id="021e0-157">Наследуется [от namedLocation.](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="021e0-157">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="021e0-158">Связи</span><span class="sxs-lookup"><span data-stu-id="021e0-158">Relationships</span></span>

<span data-ttu-id="021e0-159">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="021e0-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="021e0-160">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="021e0-160">JSON representation</span></span>

<span data-ttu-id="021e0-161">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="021e0-161">The following is a JSON representation of the resource.</span></span>

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


