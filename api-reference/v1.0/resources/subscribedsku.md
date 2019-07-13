---
title: Тип ресурса subscribedSku
description: Содержит сведения о SKU службы, на которую компания подписана.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c3343661f6c72a057c73b70f91a284f3168a9c72
ms.sourcegitcommit: 6720736406f21e40914b27ba28387adedf97fa56
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2019
ms.locfileid: "35639068"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="a45e4-103">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="a45e4-103">subscribedSku resource type</span></span>

<span data-ttu-id="a45e4-104">Содержит сведения о SKU службы, на которую компания подписана.</span><span class="sxs-lookup"><span data-stu-id="a45e4-104">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="a45e4-105">На подписанных SKU поддерживаются только операции чтения; Создание, обновление и удаление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="a45e4-105">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="a45e4-106">Выражения фильтра запросов не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="a45e4-106">Query filter expressions are not supported.</span></span> <span data-ttu-id="a45e4-107">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="a45e4-107">Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a45e4-108">Методы</span><span class="sxs-lookup"><span data-stu-id="a45e4-108">Methods</span></span>
| <span data-ttu-id="a45e4-109">Метод</span><span class="sxs-lookup"><span data-stu-id="a45e4-109">Method</span></span>           | <span data-ttu-id="a45e4-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a45e4-110">Return Type</span></span>    |<span data-ttu-id="a45e4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a45e4-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a45e4-112">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="a45e4-112">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="a45e4-113">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="a45e4-113">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="a45e4-114">Получение конкретной коммерческой подписки, приобретенной Организацией.</span><span class="sxs-lookup"><span data-stu-id="a45e4-114">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="a45e4-115">Список subscribedsku</span><span class="sxs-lookup"><span data-stu-id="a45e4-115">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="a45e4-116">Коллекция объектов [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="a45e4-116">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="a45e4-117">Получение списка коммерческих подписок, приобретенных Организацией.</span><span class="sxs-lookup"><span data-stu-id="a45e4-117">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="a45e4-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="a45e4-118">Properties</span></span>
| <span data-ttu-id="a45e4-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="a45e4-119">Property</span></span>     | <span data-ttu-id="a45e4-120">Тип</span><span class="sxs-lookup"><span data-stu-id="a45e4-120">Type</span></span>   |<span data-ttu-id="a45e4-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a45e4-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a45e4-122">Тег</span><span class="sxs-lookup"><span data-stu-id="a45e4-122">appliesTo</span></span>|<span data-ttu-id="a45e4-123">String</span><span class="sxs-lookup"><span data-stu-id="a45e4-123">String</span></span>| <span data-ttu-id="a45e4-124">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="a45e4-124">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="a45e4-125">Капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="a45e4-125">capabilityStatus</span></span>|<span data-ttu-id="a45e4-126">String</span><span class="sxs-lookup"><span data-stu-id="a45e4-126">String</span></span>| <span data-ttu-id="a45e4-127">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="a45e4-127">For example, "Enabled".</span></span> |
|<span data-ttu-id="a45e4-128">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="a45e4-128">consumedUnits</span></span>|<span data-ttu-id="a45e4-129">Int32</span><span class="sxs-lookup"><span data-stu-id="a45e4-129">Int32</span></span>| <span data-ttu-id="a45e4-130">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="a45e4-130">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="a45e4-131">id</span><span class="sxs-lookup"><span data-stu-id="a45e4-131">id</span></span>|<span data-ttu-id="a45e4-132">String</span><span class="sxs-lookup"><span data-stu-id="a45e4-132">String</span></span>| <span data-ttu-id="a45e4-133">Уникальный идентификатор объекта sku, подписка на который выполнена.</span><span class="sxs-lookup"><span data-stu-id="a45e4-133">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="a45e4-134">Key, не допускающая значение null.</span><span class="sxs-lookup"><span data-stu-id="a45e4-134">Key, not nullable.</span></span> |
|<span data-ttu-id="a45e4-135">Препаидунитс</span><span class="sxs-lookup"><span data-stu-id="a45e4-135">prepaidUnits</span></span>|[<span data-ttu-id="a45e4-136">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="a45e4-136">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="a45e4-137">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="a45e4-137">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="a45e4-138">Сервицепланс</span><span class="sxs-lookup"><span data-stu-id="a45e4-138">servicePlans</span></span>|<span data-ttu-id="a45e4-139">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="a45e4-139">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="a45e4-140">Сведения о планах обслуживания, доступных в отношении SKU.</span><span class="sxs-lookup"><span data-stu-id="a45e4-140">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="a45e4-141">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="a45e4-141">Not nullable</span></span> |
|<span data-ttu-id="a45e4-142">skuId</span><span class="sxs-lookup"><span data-stu-id="a45e4-142">skuId</span></span>|<span data-ttu-id="a45e4-143">Guid</span><span class="sxs-lookup"><span data-stu-id="a45e4-143">Guid</span></span>| <span data-ttu-id="a45e4-144">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="a45e4-144">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="a45e4-145">Скупартнумбер</span><span class="sxs-lookup"><span data-stu-id="a45e4-145">skuPartNumber</span></span>|<span data-ttu-id="a45e4-146">String</span><span class="sxs-lookup"><span data-stu-id="a45e4-146">String</span></span>| <span data-ttu-id="a45e4-147">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="a45e4-147">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="a45e4-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="a45e4-148">Relationships</span></span>
<span data-ttu-id="a45e4-149">Нет</span><span class="sxs-lookup"><span data-stu-id="a45e4-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a45e4-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a45e4-150">JSON representation</span></span>

<span data-ttu-id="a45e4-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a45e4-151">Here is a JSON representation of the resource</span></span>

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
