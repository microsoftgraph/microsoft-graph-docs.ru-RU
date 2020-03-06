---
title: Тип ресурса subscribedSku
description: Содержит сведения о SKU службы, на которую компания подписана.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b7f1d532c88b3b289e0d337236843fada7c0dd2e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533613"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="dd2e3-103">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="dd2e3-103">subscribedSku resource type</span></span>

<span data-ttu-id="dd2e3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd2e3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dd2e3-105">Содержит сведения о SKU службы, на которую компания подписана.</span><span class="sxs-lookup"><span data-stu-id="dd2e3-105">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="dd2e3-106">На подписанных SKU поддерживаются только операции чтения; Создание, обновление и удаление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="dd2e3-106">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="dd2e3-107">Выражения фильтра запросов не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="dd2e3-107">Query filter expressions are not supported.</span></span> <span data-ttu-id="dd2e3-108">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="dd2e3-108">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="dd2e3-109">Методы</span><span class="sxs-lookup"><span data-stu-id="dd2e3-109">Methods</span></span>
| <span data-ttu-id="dd2e3-110">Метод</span><span class="sxs-lookup"><span data-stu-id="dd2e3-110">Method</span></span>           | <span data-ttu-id="dd2e3-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="dd2e3-111">Return Type</span></span>    |<span data-ttu-id="dd2e3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="dd2e3-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dd2e3-113">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="dd2e3-113">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="dd2e3-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="dd2e3-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="dd2e3-115">Получение конкретной коммерческой подписки, приобретенной Организацией.</span><span class="sxs-lookup"><span data-stu-id="dd2e3-115">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="dd2e3-116">Список subscribedsku</span><span class="sxs-lookup"><span data-stu-id="dd2e3-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="dd2e3-117">Коллекция объектов [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="dd2e3-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="dd2e3-118">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="dd2e3-118">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="dd2e3-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="dd2e3-119">Properties</span></span>
| <span data-ttu-id="dd2e3-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="dd2e3-120">Property</span></span>     | <span data-ttu-id="dd2e3-121">Тип</span><span class="sxs-lookup"><span data-stu-id="dd2e3-121">Type</span></span>   |<span data-ttu-id="dd2e3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="dd2e3-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd2e3-123">Тег</span><span class="sxs-lookup"><span data-stu-id="dd2e3-123">appliesTo</span></span>|<span data-ttu-id="dd2e3-124">String</span><span class="sxs-lookup"><span data-stu-id="dd2e3-124">String</span></span>| <span data-ttu-id="dd2e3-125">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="dd2e3-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="dd2e3-126">капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="dd2e3-126">capabilityStatus</span></span>|<span data-ttu-id="dd2e3-127">Строка</span><span class="sxs-lookup"><span data-stu-id="dd2e3-127">String</span></span>|  <span data-ttu-id="dd2e3-128">Возможные значения: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span><span class="sxs-lookup"><span data-stu-id="dd2e3-128">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> |
|<span data-ttu-id="dd2e3-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="dd2e3-129">consumedUnits</span></span>|<span data-ttu-id="dd2e3-130">Int32</span><span class="sxs-lookup"><span data-stu-id="dd2e3-130">Int32</span></span>| <span data-ttu-id="dd2e3-131">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="dd2e3-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="dd2e3-132">id</span><span class="sxs-lookup"><span data-stu-id="dd2e3-132">id</span></span>|<span data-ttu-id="dd2e3-133">Строка</span><span class="sxs-lookup"><span data-stu-id="dd2e3-133">String</span></span>| <span data-ttu-id="dd2e3-134">Уникальный идентификатор объекта sku, подписка на который выполнена.</span><span class="sxs-lookup"><span data-stu-id="dd2e3-134">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="dd2e3-135">Key, не допускающая значение null.</span><span class="sxs-lookup"><span data-stu-id="dd2e3-135">Key, not nullable.</span></span> |
|<span data-ttu-id="dd2e3-136">препаидунитс</span><span class="sxs-lookup"><span data-stu-id="dd2e3-136">prepaidUnits</span></span>|[<span data-ttu-id="dd2e3-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="dd2e3-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="dd2e3-138">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="dd2e3-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="dd2e3-139">сервицепланс</span><span class="sxs-lookup"><span data-stu-id="dd2e3-139">servicePlans</span></span>|<span data-ttu-id="dd2e3-140">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="dd2e3-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="dd2e3-141">Сведения о планах обслуживания, доступных в отношении SKU.</span><span class="sxs-lookup"><span data-stu-id="dd2e3-141">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="dd2e3-142">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="dd2e3-142">Not nullable</span></span> |
|<span data-ttu-id="dd2e3-143">skuId</span><span class="sxs-lookup"><span data-stu-id="dd2e3-143">skuId</span></span>|<span data-ttu-id="dd2e3-144">Guid</span><span class="sxs-lookup"><span data-stu-id="dd2e3-144">Guid</span></span>| <span data-ttu-id="dd2e3-145">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="dd2e3-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="dd2e3-146">скупартнумбер</span><span class="sxs-lookup"><span data-stu-id="dd2e3-146">skuPartNumber</span></span>|<span data-ttu-id="dd2e3-147">String</span><span class="sxs-lookup"><span data-stu-id="dd2e3-147">String</span></span>| <span data-ttu-id="dd2e3-148">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="dd2e3-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="dd2e3-149">Чтобы получить список коммерческих подписок, приобретенных в Организации, ознакомьтесь со статьей [List субскрибедскус](../api/subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="dd2e3-149">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd2e3-150">Связи</span><span class="sxs-lookup"><span data-stu-id="dd2e3-150">Relationships</span></span>
<span data-ttu-id="dd2e3-151">Нет</span><span class="sxs-lookup"><span data-stu-id="dd2e3-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd2e3-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dd2e3-152">JSON representation</span></span>

<span data-ttu-id="dd2e3-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dd2e3-153">Here is a JSON representation of the resource</span></span>

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
