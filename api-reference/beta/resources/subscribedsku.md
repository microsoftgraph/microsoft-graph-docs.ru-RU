---
title: Тип ресурса subscribedSku
description: Представляет тип подписанного SKU.
localization_priority: Normal
author: SumitParikh
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9d9ccb4bd30a3b14bdfd2527dedde0a0030cb2bd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997524"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="d03d3-103">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="d03d3-103">subscribedSku resource type</span></span>

<span data-ttu-id="d03d3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d03d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d03d3-105">На подписанных SKU поддерживаются только операции чтения; Создание, обновление и удаление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="d03d3-105">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="d03d3-106">Выражения фильтра запросов не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="d03d3-106">Query filter expressions are not supported.</span></span> <span data-ttu-id="d03d3-107">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="d03d3-107">Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="d03d3-108">Методы</span><span class="sxs-lookup"><span data-stu-id="d03d3-108">Methods</span></span>
| <span data-ttu-id="d03d3-109">Метод</span><span class="sxs-lookup"><span data-stu-id="d03d3-109">Method</span></span>           | <span data-ttu-id="d03d3-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d03d3-110">Return Type</span></span>    |<span data-ttu-id="d03d3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d03d3-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d03d3-112">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="d03d3-112">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="d03d3-113">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="d03d3-113">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="d03d3-114">Получение конкретной коммерческой подписки, приобретенной Организацией.</span><span class="sxs-lookup"><span data-stu-id="d03d3-114">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="d03d3-115">Список subscribedsku</span><span class="sxs-lookup"><span data-stu-id="d03d3-115">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="d03d3-116">Коллекция объектов [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="d03d3-116">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="d03d3-117">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="d03d3-117">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="d03d3-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="d03d3-118">Properties</span></span>
| <span data-ttu-id="d03d3-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="d03d3-119">Property</span></span>     | <span data-ttu-id="d03d3-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d03d3-120">Type</span></span>   |<span data-ttu-id="d03d3-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d03d3-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d03d3-122">Тег</span><span class="sxs-lookup"><span data-stu-id="d03d3-122">appliesTo</span></span>|<span data-ttu-id="d03d3-123">String</span><span class="sxs-lookup"><span data-stu-id="d03d3-123">String</span></span>| <span data-ttu-id="d03d3-124">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="d03d3-124">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="d03d3-125">капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="d03d3-125">capabilityStatus</span></span>|<span data-ttu-id="d03d3-126">String</span><span class="sxs-lookup"><span data-stu-id="d03d3-126">String</span></span>| <span data-ttu-id="d03d3-127">Возможные значения: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span><span class="sxs-lookup"><span data-stu-id="d03d3-127">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> |
|<span data-ttu-id="d03d3-128">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="d03d3-128">consumedUnits</span></span>|<span data-ttu-id="d03d3-129">Int32</span><span class="sxs-lookup"><span data-stu-id="d03d3-129">Int32</span></span>| <span data-ttu-id="d03d3-130">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="d03d3-130">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="d03d3-131">id</span><span class="sxs-lookup"><span data-stu-id="d03d3-131">id</span></span>|<span data-ttu-id="d03d3-132">String</span><span class="sxs-lookup"><span data-stu-id="d03d3-132">String</span></span>| <span data-ttu-id="d03d3-133">Уникальный идентификатор объекта sku, подписка на который выполнена.</span><span class="sxs-lookup"><span data-stu-id="d03d3-133">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="d03d3-134">Key, не допускающая значение null.</span><span class="sxs-lookup"><span data-stu-id="d03d3-134">Key, not nullable.</span></span> |
|<span data-ttu-id="d03d3-135">препаидунитс</span><span class="sxs-lookup"><span data-stu-id="d03d3-135">prepaidUnits</span></span>|[<span data-ttu-id="d03d3-136">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="d03d3-136">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="d03d3-137">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="d03d3-137">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="d03d3-138">сервицепланс</span><span class="sxs-lookup"><span data-stu-id="d03d3-138">servicePlans</span></span>|<span data-ttu-id="d03d3-139">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="d03d3-139">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="d03d3-140">Сведения о планах обслуживания, доступных в отношении SKU.</span><span class="sxs-lookup"><span data-stu-id="d03d3-140">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="d03d3-141">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="d03d3-141">Not nullable</span></span> |
|<span data-ttu-id="d03d3-142">skuId</span><span class="sxs-lookup"><span data-stu-id="d03d3-142">skuId</span></span>|<span data-ttu-id="d03d3-143">Guid</span><span class="sxs-lookup"><span data-stu-id="d03d3-143">Guid</span></span>| <span data-ttu-id="d03d3-144">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="d03d3-144">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="d03d3-145">скупартнумбер</span><span class="sxs-lookup"><span data-stu-id="d03d3-145">skuPartNumber</span></span>|<span data-ttu-id="d03d3-146">String</span><span class="sxs-lookup"><span data-stu-id="d03d3-146">String</span></span>| <span data-ttu-id="d03d3-147">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="d03d3-147">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="d03d3-148">Чтобы получить список коммерческих подписок, приобретенных в Организации, ознакомьтесь со статьей [List субскрибедскус](../api/subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="d03d3-148">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="d03d3-149">Связи</span><span class="sxs-lookup"><span data-stu-id="d03d3-149">Relationships</span></span>
<span data-ttu-id="d03d3-150">Нет</span><span class="sxs-lookup"><span data-stu-id="d03d3-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d03d3-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d03d3-151">JSON representation</span></span>

<span data-ttu-id="d03d3-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d03d3-152">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.subscribedSku"
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
<!--
{
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


