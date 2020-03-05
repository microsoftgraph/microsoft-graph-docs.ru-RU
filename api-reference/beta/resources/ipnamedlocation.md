---
title: Тип ресурса Ипнамедлокатион
description: Представляет Azure Active Directory с именем Location, заданным диапазонами IP-адресов. Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e32d6c51ae09601bc752ed2a352dc50a4285f7c2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523165"
---
# <a name="ipnamedlocation-resource-type"></a><span data-ttu-id="3581a-104">Тип ресурса Ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="3581a-104">ipNamedLocation resource type</span></span>

<span data-ttu-id="3581a-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3581a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3581a-106">Представляет Azure Active Directory с именем Location, заданным диапазонами IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="3581a-106">Represents an Azure Active Directory named location defined by IP ranges.</span></span> <span data-ttu-id="3581a-107">Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.</span><span class="sxs-lookup"><span data-stu-id="3581a-107">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="3581a-108">Наследуется от [намедлокатион](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="3581a-108">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="3581a-109">Методы</span><span class="sxs-lookup"><span data-stu-id="3581a-109">Methods</span></span>

| <span data-ttu-id="3581a-110">Метод</span><span class="sxs-lookup"><span data-stu-id="3581a-110">Method</span></span>       | <span data-ttu-id="3581a-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3581a-111">Return Type</span></span> | <span data-ttu-id="3581a-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3581a-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3581a-113">Список Ипнамедлокатионс</span><span class="sxs-lookup"><span data-stu-id="3581a-113">List ipNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="3581a-114">Коллекция [ипнамедлокатион](ipNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="3581a-114">[ipNamedLocation](ipNamedLocation.md) collection</span></span> | <span data-ttu-id="3581a-115">Получение всех объектов **ипнамедлокатион** в Организации.</span><span class="sxs-lookup"><span data-stu-id="3581a-115">Get all the **ipNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="3581a-116">Создание Ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="3581a-116">Create ipNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="3581a-117">ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="3581a-117">ipNamedLocation</span></span>](ipNamedLocation.md) | <span data-ttu-id="3581a-118">Создание нового объекта **ипнамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="3581a-118">Create a new **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="3581a-119">Получение Ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="3581a-119">Get ipNamedLocation</span></span>](../api/ipnamedlocation-get.md) | [<span data-ttu-id="3581a-120">ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="3581a-120">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="3581a-121">Чтение свойств и связей объекта **ипнамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="3581a-121">Read the properties and relationships of an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="3581a-122">Обновление Ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="3581a-122">Update ipNamedLocation</span></span>](../api/ipnamedlocation-update.md) | [<span data-ttu-id="3581a-123">ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="3581a-123">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="3581a-124">Обновление объекта **ипнамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="3581a-124">Update an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="3581a-125">Удаление Ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="3581a-125">Delete ipNamedLocation</span></span>](../api/ipnamedlocation-delete.md) | <span data-ttu-id="3581a-126">Нет</span><span class="sxs-lookup"><span data-stu-id="3581a-126">None</span></span> | <span data-ttu-id="3581a-127">Удаление объекта **ипнамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="3581a-127">Delete an **ipNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="3581a-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="3581a-128">Properties</span></span>

| <span data-ttu-id="3581a-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="3581a-129">Property</span></span>     | <span data-ttu-id="3581a-130">Тип</span><span class="sxs-lookup"><span data-stu-id="3581a-130">Type</span></span>        | <span data-ttu-id="3581a-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3581a-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3581a-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3581a-132">createdDateTime</span></span>|<span data-ttu-id="3581a-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3581a-133">DateTimeOffset</span></span>|<span data-ttu-id="3581a-134">Тип timestamp представляет дату и время создания расположения с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3581a-134">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3581a-135">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3581a-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="3581a-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3581a-136">Read-only.</span></span> <span data-ttu-id="3581a-137">Наследуется от [намедлокатион](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="3581a-137">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="3581a-138">displayName</span><span class="sxs-lookup"><span data-stu-id="3581a-138">displayName</span></span>|<span data-ttu-id="3581a-139">Строка</span><span class="sxs-lookup"><span data-stu-id="3581a-139">String</span></span>|<span data-ttu-id="3581a-140">Удобное для человека имя расположения.</span><span class="sxs-lookup"><span data-stu-id="3581a-140">Human-readable name of the location.</span></span>|
|<span data-ttu-id="3581a-141">id</span><span class="sxs-lookup"><span data-stu-id="3581a-141">id</span></span>|<span data-ttu-id="3581a-142">String</span><span class="sxs-lookup"><span data-stu-id="3581a-142">String</span></span>|<span data-ttu-id="3581a-143">Идентификатор объекта Намедлокатион.</span><span class="sxs-lookup"><span data-stu-id="3581a-143">Identifier of a namedLocation object.</span></span> <span data-ttu-id="3581a-144">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3581a-144">Read-only.</span></span> <span data-ttu-id="3581a-145">Наследуется от [намедлокатион](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="3581a-145">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="3581a-146">ипранжес</span><span class="sxs-lookup"><span data-stu-id="3581a-146">ipRanges</span></span>|<span data-ttu-id="3581a-147">Коллекция объектов [ipRange](iprange.md)</span><span class="sxs-lookup"><span data-stu-id="3581a-147">[ipRange](iprange.md) collection</span></span>|<span data-ttu-id="3581a-148">Список диапазонов IP-адресов в формате CIDR IPv4 (например, 1.2.3.4/32) или любом допустимом формате IPv6 из IETF RFC596.</span><span class="sxs-lookup"><span data-stu-id="3581a-148">List of IP address ranges in IPv4 CIDR format (e.g. 1.2.3.4/32) or any allowable IPv6 format from IETF RFC596.</span></span>|
|<span data-ttu-id="3581a-149">Доверять</span><span class="sxs-lookup"><span data-stu-id="3581a-149">isTrusted</span></span>|<span data-ttu-id="3581a-150">Логический</span><span class="sxs-lookup"><span data-stu-id="3581a-150">Boolean</span></span>|<span data-ttu-id="3581a-151">Значение true, если данное расположение явно является доверенным.</span><span class="sxs-lookup"><span data-stu-id="3581a-151">True if this location is explicitly trusted.</span></span>|
|<span data-ttu-id="3581a-152">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3581a-152">modifiedDateTime</span></span>|<span data-ttu-id="3581a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3581a-153">DateTimeOffset</span></span>|<span data-ttu-id="3581a-154">Тип timestamp представляет дату и время последнего изменения расположения с использованием формата ISO 8601, которое всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3581a-154">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3581a-155">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="3581a-155">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="3581a-156">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3581a-156">Read-only.</span></span> <span data-ttu-id="3581a-157">Наследуется от [намедлокатион](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="3581a-157">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="3581a-158">Связи</span><span class="sxs-lookup"><span data-stu-id="3581a-158">Relationships</span></span>

<span data-ttu-id="3581a-159">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3581a-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3581a-160">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="3581a-160">JSON representation</span></span>

<span data-ttu-id="3581a-161">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3581a-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.ipNamedLocation",
  "baseType": ""
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
