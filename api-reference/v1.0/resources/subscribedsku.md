---
title: Тип ресурса subscribedSku
description: Содержит сведения о SKU службы, на которую компания подписана.
localization_priority: Normal
author: SumitParikh
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cb9933ddc93ca647bca1427d3401cb912662ab2c
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "43384942"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="8d330-103">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="8d330-103">subscribedSku resource type</span></span>

<span data-ttu-id="8d330-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d330-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8d330-105">Содержит сведения о SKU службы, на которую компания подписана.</span><span class="sxs-lookup"><span data-stu-id="8d330-105">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="8d330-106">На подписанных SKU поддерживаются только операции чтения; Создание, обновление и удаление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="8d330-106">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="8d330-107">Выражения фильтра запросов не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="8d330-107">Query filter expressions are not supported.</span></span> <span data-ttu-id="8d330-108">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="8d330-108">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="8d330-109">Методы</span><span class="sxs-lookup"><span data-stu-id="8d330-109">Methods</span></span>
| <span data-ttu-id="8d330-110">Метод</span><span class="sxs-lookup"><span data-stu-id="8d330-110">Method</span></span>           | <span data-ttu-id="8d330-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8d330-111">Return Type</span></span>    |<span data-ttu-id="8d330-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8d330-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8d330-113">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="8d330-113">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="8d330-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="8d330-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="8d330-115">Получение конкретной коммерческой подписки, приобретенной Организацией.</span><span class="sxs-lookup"><span data-stu-id="8d330-115">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="8d330-116">Список subscribedsku</span><span class="sxs-lookup"><span data-stu-id="8d330-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="8d330-117">Коллекция объектов [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="8d330-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="8d330-118">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="8d330-118">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="8d330-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d330-119">Properties</span></span>
| <span data-ttu-id="8d330-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d330-120">Property</span></span>     | <span data-ttu-id="8d330-121">Тип</span><span class="sxs-lookup"><span data-stu-id="8d330-121">Type</span></span>   |<span data-ttu-id="8d330-122">Описание</span><span class="sxs-lookup"><span data-stu-id="8d330-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8d330-123">Тег</span><span class="sxs-lookup"><span data-stu-id="8d330-123">appliesTo</span></span>|<span data-ttu-id="8d330-124">String</span><span class="sxs-lookup"><span data-stu-id="8d330-124">String</span></span>| <span data-ttu-id="8d330-125">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="8d330-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="8d330-126">капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="8d330-126">capabilityStatus</span></span>|<span data-ttu-id="8d330-127">String</span><span class="sxs-lookup"><span data-stu-id="8d330-127">String</span></span>|  <span data-ttu-id="8d330-128">Возможные значения: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span><span class="sxs-lookup"><span data-stu-id="8d330-128">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> |
|<span data-ttu-id="8d330-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="8d330-129">consumedUnits</span></span>|<span data-ttu-id="8d330-130">Int32</span><span class="sxs-lookup"><span data-stu-id="8d330-130">Int32</span></span>| <span data-ttu-id="8d330-131">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="8d330-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="8d330-132">id</span><span class="sxs-lookup"><span data-stu-id="8d330-132">id</span></span>|<span data-ttu-id="8d330-133">String</span><span class="sxs-lookup"><span data-stu-id="8d330-133">String</span></span>| <span data-ttu-id="8d330-134">Уникальный идентификатор объекта sku, подписка на который выполнена.</span><span class="sxs-lookup"><span data-stu-id="8d330-134">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="8d330-135">Key, не допускающая значение null.</span><span class="sxs-lookup"><span data-stu-id="8d330-135">Key, not nullable.</span></span> |
|<span data-ttu-id="8d330-136">препаидунитс</span><span class="sxs-lookup"><span data-stu-id="8d330-136">prepaidUnits</span></span>|[<span data-ttu-id="8d330-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="8d330-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="8d330-138">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="8d330-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="8d330-139">сервицепланс</span><span class="sxs-lookup"><span data-stu-id="8d330-139">servicePlans</span></span>|<span data-ttu-id="8d330-140">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="8d330-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="8d330-141">Сведения о планах обслуживания, доступных в отношении SKU.</span><span class="sxs-lookup"><span data-stu-id="8d330-141">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="8d330-142">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="8d330-142">Not nullable</span></span> |
|<span data-ttu-id="8d330-143">skuId</span><span class="sxs-lookup"><span data-stu-id="8d330-143">skuId</span></span>|<span data-ttu-id="8d330-144">Guid</span><span class="sxs-lookup"><span data-stu-id="8d330-144">Guid</span></span>| <span data-ttu-id="8d330-145">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="8d330-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="8d330-146">скупартнумбер</span><span class="sxs-lookup"><span data-stu-id="8d330-146">skuPartNumber</span></span>|<span data-ttu-id="8d330-147">String</span><span class="sxs-lookup"><span data-stu-id="8d330-147">String</span></span>| <span data-ttu-id="8d330-148">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="8d330-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="8d330-149">Чтобы получить список коммерческих подписок, приобретенных в Организации, ознакомьтесь со статьей [List субскрибедскус](../api/subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="8d330-149">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d330-150">Отношения</span><span class="sxs-lookup"><span data-stu-id="8d330-150">Relationships</span></span>
<span data-ttu-id="8d330-151">Нет</span><span class="sxs-lookup"><span data-stu-id="8d330-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d330-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d330-152">JSON representation</span></span>

<span data-ttu-id="8d330-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d330-153">Here is a JSON representation of the resource</span></span>

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
