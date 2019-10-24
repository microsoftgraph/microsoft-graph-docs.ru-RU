---
title: Тип ресурса Ипнамедлокатион
description: Представляет Azure Active Directory с именем Location, заданным диапазонами IP-адресов. Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 10bdafb9894d822f345bb6fb23174fa7f7deee4c
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653820"
---
# <a name="ipnamedlocation-resource-type"></a><span data-ttu-id="172a4-104">Тип ресурса Ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="172a4-104">ipNamedLocation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="172a4-105">Представляет Azure Active Directory с именем Location, заданным диапазонами IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="172a4-105">Represents an Azure Active Directory named location defined by IP ranges.</span></span> <span data-ttu-id="172a4-106">Именованные расположения — это настраиваемые правила, определяющие сетевые расположения, которые можно использовать в политике условного доступа.</span><span class="sxs-lookup"><span data-stu-id="172a4-106">Named locations are custom rules that define network locations which can then be used in a Conditional Access policy.</span></span>

<span data-ttu-id="172a4-107">Наследуется от [намедлокатион](../resources/namedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="172a4-107">Inherits from [namedLocation](../resources/namedLocation.md)</span></span>

## <a name="methods"></a><span data-ttu-id="172a4-108">Методы</span><span class="sxs-lookup"><span data-stu-id="172a4-108">Methods</span></span>

| <span data-ttu-id="172a4-109">Метод</span><span class="sxs-lookup"><span data-stu-id="172a4-109">Method</span></span>       | <span data-ttu-id="172a4-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="172a4-110">Return Type</span></span> | <span data-ttu-id="172a4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="172a4-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="172a4-112">Список Ипнамедлокатионс</span><span class="sxs-lookup"><span data-stu-id="172a4-112">List ipNamedLocations</span></span>](../api/conditionalaccessroot-list-namedlocations.md) | <span data-ttu-id="172a4-113">Коллекция [ипнамедлокатион](ipNamedLocation.md)</span><span class="sxs-lookup"><span data-stu-id="172a4-113">[ipNamedLocation](ipNamedLocation.md) collection</span></span> | <span data-ttu-id="172a4-114">Получение всех объектов **ипнамедлокатион** в Организации.</span><span class="sxs-lookup"><span data-stu-id="172a4-114">Get all the **ipNamedLocation** objects in the organization.</span></span> |
| [<span data-ttu-id="172a4-115">Создание Ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="172a4-115">Create ipNamedLocation</span></span>](../api/conditionalaccessroot-post-namedlocations.md) | [<span data-ttu-id="172a4-116">ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="172a4-116">ipNamedLocation</span></span>](ipNamedLocation.md) | <span data-ttu-id="172a4-117">Создание нового объекта **ипнамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="172a4-117">Create a new **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="172a4-118">Получение Ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="172a4-118">Get ipNamedLocation</span></span>](../api/ipnamedlocation-get.md) | [<span data-ttu-id="172a4-119">ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="172a4-119">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="172a4-120">Чтение свойств и связей объекта **ипнамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="172a4-120">Read the properties and relationships of an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="172a4-121">Обновление Ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="172a4-121">Update ipNamedLocation</span></span>](../api/ipnamedlocation-update.md) | [<span data-ttu-id="172a4-122">ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="172a4-122">ipNamedLocation</span></span>](ipnamedlocation.md) | <span data-ttu-id="172a4-123">Обновление объекта **ипнамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="172a4-123">Update an **ipNamedLocation** object.</span></span> |
| [<span data-ttu-id="172a4-124">Удаление Ипнамедлокатион</span><span class="sxs-lookup"><span data-stu-id="172a4-124">Delete ipNamedLocation</span></span>](../api/ipnamedlocation-delete.md) | <span data-ttu-id="172a4-125">Нет</span><span class="sxs-lookup"><span data-stu-id="172a4-125">None</span></span> | <span data-ttu-id="172a4-126">Удаление объекта **ипнамедлокатион** .</span><span class="sxs-lookup"><span data-stu-id="172a4-126">Delete an **ipNamedLocation** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="172a4-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="172a4-127">Properties</span></span>

| <span data-ttu-id="172a4-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="172a4-128">Property</span></span>     | <span data-ttu-id="172a4-129">Тип</span><span class="sxs-lookup"><span data-stu-id="172a4-129">Type</span></span>        | <span data-ttu-id="172a4-130">Описание</span><span class="sxs-lookup"><span data-stu-id="172a4-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="172a4-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="172a4-131">createdDateTime</span></span>|<span data-ttu-id="172a4-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="172a4-132">DateTimeOffset</span></span>|<span data-ttu-id="172a4-133">Тип timestamp представляет дату и время создания расположения с использованием формата ISO 8601 и всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="172a4-133">The Timestamp type represents creation date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="172a4-134">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="172a4-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="172a4-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="172a4-135">Read-only.</span></span> <span data-ttu-id="172a4-136">Наследуется от [намедлокатион](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="172a4-136">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="172a4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="172a4-137">displayName</span></span>|<span data-ttu-id="172a4-138">Строка</span><span class="sxs-lookup"><span data-stu-id="172a4-138">String</span></span>|<span data-ttu-id="172a4-139">Удобное для человека имя расположения.</span><span class="sxs-lookup"><span data-stu-id="172a4-139">Human-readable name of the location.</span></span>|
|<span data-ttu-id="172a4-140">id</span><span class="sxs-lookup"><span data-stu-id="172a4-140">id</span></span>|<span data-ttu-id="172a4-141">String</span><span class="sxs-lookup"><span data-stu-id="172a4-141">String</span></span>|<span data-ttu-id="172a4-142">Идентификатор объекта Намедлокатион.</span><span class="sxs-lookup"><span data-stu-id="172a4-142">Identifier of a namedLocation object.</span></span> <span data-ttu-id="172a4-143">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="172a4-143">Read-only.</span></span> <span data-ttu-id="172a4-144">Наследуется от [намедлокатион](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="172a4-144">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|
|<span data-ttu-id="172a4-145">ипранжес</span><span class="sxs-lookup"><span data-stu-id="172a4-145">ipRanges</span></span>|<span data-ttu-id="172a4-146">Коллекция объектов [ipRange](iprange.md)</span><span class="sxs-lookup"><span data-stu-id="172a4-146">[ipRange](iprange.md) collection</span></span>|<span data-ttu-id="172a4-147">Список диапазонов IP-адресов в формате CIDR IPv4 (например, 1.2.3.4/32) или любом допустимом формате IPv6 из IETF RFC596.</span><span class="sxs-lookup"><span data-stu-id="172a4-147">List of IP address ranges in IPv4 CIDR format (e.g. 1.2.3.4/32) or any allowable IPv6 format from IETF RFC596.</span></span>|
|<span data-ttu-id="172a4-148">Доверять</span><span class="sxs-lookup"><span data-stu-id="172a4-148">isTrusted</span></span>|<span data-ttu-id="172a4-149">Логический</span><span class="sxs-lookup"><span data-stu-id="172a4-149">Boolean</span></span>|<span data-ttu-id="172a4-150">Значение true, если данное расположение явно является доверенным.</span><span class="sxs-lookup"><span data-stu-id="172a4-150">True if this location is explicitly trusted.</span></span>|
|<span data-ttu-id="172a4-151">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="172a4-151">modifiedDateTime</span></span>|<span data-ttu-id="172a4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="172a4-152">DateTimeOffset</span></span>|<span data-ttu-id="172a4-153">Тип timestamp представляет дату и время последнего изменения расположения с использованием формата ISO 8601, которое всегда задается в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="172a4-153">The Timestamp type represents last modified date and time of the location using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="172a4-154">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="172a4-154">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="172a4-155">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="172a4-155">Read-only.</span></span> <span data-ttu-id="172a4-156">Наследуется от [намедлокатион](../resources/namedLocation.md).</span><span class="sxs-lookup"><span data-stu-id="172a4-156">Inherited from [namedLocation](../resources/namedLocation.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="172a4-157">Связи</span><span class="sxs-lookup"><span data-stu-id="172a4-157">Relationships</span></span>

<span data-ttu-id="172a4-158">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="172a4-158">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="172a4-159">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="172a4-159">JSON representation</span></span>

<span data-ttu-id="172a4-160">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="172a4-160">The following is a JSON representation of the resource.</span></span>

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
