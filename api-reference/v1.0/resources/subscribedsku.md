---
title: Тип ресурса subscribedSku
description: Содержит сведения о SKU службы, на которую компания подписана.
localization_priority: Normal
author: SumitParikh
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 291a30b0d8d4aa9181114cf392b5c466fc395925
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030798"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="c1c2e-103">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="c1c2e-103">subscribedSku resource type</span></span>

<span data-ttu-id="c1c2e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1c2e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c1c2e-105">Содержит сведения о SKU службы, на которую компания подписана.</span><span class="sxs-lookup"><span data-stu-id="c1c2e-105">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="c1c2e-106">Только операция чтения поддерживается в поддерживаемых skUs; создание, обновление и удаление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="c1c2e-106">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="c1c2e-107">Выражения фильтра запросов не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="c1c2e-107">Query filter expressions are not supported.</span></span> <span data-ttu-id="c1c2e-108">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="c1c2e-108">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c1c2e-109">Методы</span><span class="sxs-lookup"><span data-stu-id="c1c2e-109">Methods</span></span>
| <span data-ttu-id="c1c2e-110">Метод</span><span class="sxs-lookup"><span data-stu-id="c1c2e-110">Method</span></span>           | <span data-ttu-id="c1c2e-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c1c2e-111">Return Type</span></span>    |<span data-ttu-id="c1c2e-112">Описание</span><span class="sxs-lookup"><span data-stu-id="c1c2e-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c1c2e-113">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="c1c2e-113">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="c1c2e-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="c1c2e-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="c1c2e-115">Получение определенной коммерческой подписки, приобретенной организацией.</span><span class="sxs-lookup"><span data-stu-id="c1c2e-115">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="c1c2e-116">Список subscribedsku</span><span class="sxs-lookup"><span data-stu-id="c1c2e-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="c1c2e-117">Коллекция объектов [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="c1c2e-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="c1c2e-118">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="c1c2e-118">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="c1c2e-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1c2e-119">Properties</span></span>
| <span data-ttu-id="c1c2e-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1c2e-120">Property</span></span>     | <span data-ttu-id="c1c2e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="c1c2e-121">Type</span></span>   |<span data-ttu-id="c1c2e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="c1c2e-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1c2e-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="c1c2e-123">appliesTo</span></span>|<span data-ttu-id="c1c2e-124">String</span><span class="sxs-lookup"><span data-stu-id="c1c2e-124">String</span></span>| <span data-ttu-id="c1c2e-125">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="c1c2e-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="c1c2e-126">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="c1c2e-126">capabilityStatus</span></span>|<span data-ttu-id="c1c2e-127">String</span><span class="sxs-lookup"><span data-stu-id="c1c2e-127">String</span></span>|  <span data-ttu-id="c1c2e-128">Возможные значения: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span><span class="sxs-lookup"><span data-stu-id="c1c2e-128">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> <span data-ttu-id="c1c2e-129">The capabilityStatus is `Enabled` if the **prepaidUnits** property has at least 1 unit that is **enabled,** and `LockedOut` if the customer cancelled their subscription.</span><span class="sxs-lookup"><span data-stu-id="c1c2e-129">The capabilityStatus is `Enabled` if the **prepaidUnits** property has at least 1 unit that is **enabled**, and `LockedOut` if the customer cancelled their subscription.</span></span> |
|<span data-ttu-id="c1c2e-130">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="c1c2e-130">consumedUnits</span></span>|<span data-ttu-id="c1c2e-131">Int32</span><span class="sxs-lookup"><span data-stu-id="c1c2e-131">Int32</span></span>| <span data-ttu-id="c1c2e-132">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="c1c2e-132">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="c1c2e-133">id</span><span class="sxs-lookup"><span data-stu-id="c1c2e-133">id</span></span>|<span data-ttu-id="c1c2e-134">String</span><span class="sxs-lookup"><span data-stu-id="c1c2e-134">String</span></span>| <span data-ttu-id="c1c2e-135">Уникальный идентификатор объекта sku, подписка на который выполнена.</span><span class="sxs-lookup"><span data-stu-id="c1c2e-135">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="c1c2e-136">Key, not nullable.</span><span class="sxs-lookup"><span data-stu-id="c1c2e-136">Key, not nullable.</span></span> |
|<span data-ttu-id="c1c2e-137">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="c1c2e-137">prepaidUnits</span></span>|[<span data-ttu-id="c1c2e-138">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="c1c2e-138">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="c1c2e-139">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="c1c2e-139">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="c1c2e-140">servicePlans</span><span class="sxs-lookup"><span data-stu-id="c1c2e-140">servicePlans</span></span>|<span data-ttu-id="c1c2e-141">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="c1c2e-141">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="c1c2e-142">Сведения о планах обслуживания, доступных в отношении SKU.</span><span class="sxs-lookup"><span data-stu-id="c1c2e-142">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="c1c2e-143">Не является недействительным</span><span class="sxs-lookup"><span data-stu-id="c1c2e-143">Not nullable</span></span> |
|<span data-ttu-id="c1c2e-144">skuId</span><span class="sxs-lookup"><span data-stu-id="c1c2e-144">skuId</span></span>|<span data-ttu-id="c1c2e-145">Guid</span><span class="sxs-lookup"><span data-stu-id="c1c2e-145">Guid</span></span>| <span data-ttu-id="c1c2e-146">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="c1c2e-146">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="c1c2e-147">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="c1c2e-147">skuPartNumber</span></span>|<span data-ttu-id="c1c2e-148">String</span><span class="sxs-lookup"><span data-stu-id="c1c2e-148">String</span></span>| <span data-ttu-id="c1c2e-149">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="c1c2e-149">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="c1c2e-150">Чтобы получить список коммерческих подписок, приобретенных организацией, см. в [журнале List subscribedSkus.](../api/subscribedsku-list.md)</span><span class="sxs-lookup"><span data-stu-id="c1c2e-150">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1c2e-151">Связи</span><span class="sxs-lookup"><span data-stu-id="c1c2e-151">Relationships</span></span>
<span data-ttu-id="c1c2e-152">Нет</span><span class="sxs-lookup"><span data-stu-id="c1c2e-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1c2e-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1c2e-153">JSON representation</span></span>

<span data-ttu-id="c1c2e-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1c2e-154">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscribedSku",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "appliesTo": "string",
  "capabilityStatus": "string",
  "consumedUnits": 1024,
  "id": "string (identifier)",
  "prepaidUnits": {"@odata.type": "microsoft.graph.licenseUnitsDetail"},
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "guid",
  "skuPartNumber": "string"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

