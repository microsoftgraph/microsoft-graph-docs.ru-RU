---
title: Тип ресурса subscribedSku
description: " Создание, обновление и удаление не поддерживаются. Выражения фильтра запросов не поддерживаются. Наследуется от directoryObject."
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c2bca99fed2b8c5328c2f2cf1ac3bf938ddcfcaa
ms.sourcegitcommit: 6720736406f21e40914b27ba28387adedf97fa56
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2019
ms.locfileid: "35639026"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="90300-105">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="90300-105">subscribedSku resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90300-106">На подписанных SKU поддерживаются только операции чтения; Создание, обновление и удаление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="90300-106">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="90300-107">Выражения фильтра запросов не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="90300-107">Query filter expressions are not supported.</span></span> <span data-ttu-id="90300-108">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="90300-108">Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="90300-109">Методы</span><span class="sxs-lookup"><span data-stu-id="90300-109">Methods</span></span>
| <span data-ttu-id="90300-110">Метод</span><span class="sxs-lookup"><span data-stu-id="90300-110">Method</span></span>           | <span data-ttu-id="90300-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="90300-111">Return Type</span></span>    |<span data-ttu-id="90300-112">Описание</span><span class="sxs-lookup"><span data-stu-id="90300-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="90300-113">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="90300-113">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="90300-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="90300-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="90300-115">Получение конкретной коммерческой подписки, приобретенной Организацией.</span><span class="sxs-lookup"><span data-stu-id="90300-115">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="90300-116">Список subscribedsku</span><span class="sxs-lookup"><span data-stu-id="90300-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="90300-117">Коллекция объектов [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="90300-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="90300-118">Получение списка коммерческих подписок, приобретенных Организацией.</span><span class="sxs-lookup"><span data-stu-id="90300-118">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="90300-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="90300-119">Properties</span></span>
| <span data-ttu-id="90300-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="90300-120">Property</span></span>     | <span data-ttu-id="90300-121">Тип</span><span class="sxs-lookup"><span data-stu-id="90300-121">Type</span></span>   |<span data-ttu-id="90300-122">Описание</span><span class="sxs-lookup"><span data-stu-id="90300-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90300-123">Тег</span><span class="sxs-lookup"><span data-stu-id="90300-123">appliesTo</span></span>|<span data-ttu-id="90300-124">String</span><span class="sxs-lookup"><span data-stu-id="90300-124">String</span></span>| <span data-ttu-id="90300-125">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="90300-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="90300-126">Капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="90300-126">capabilityStatus</span></span>|<span data-ttu-id="90300-127">String</span><span class="sxs-lookup"><span data-stu-id="90300-127">String</span></span>| <span data-ttu-id="90300-128">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="90300-128">For example, "Enabled".</span></span> |
|<span data-ttu-id="90300-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="90300-129">consumedUnits</span></span>|<span data-ttu-id="90300-130">Int32</span><span class="sxs-lookup"><span data-stu-id="90300-130">Int32</span></span>| <span data-ttu-id="90300-131">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="90300-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="90300-132">id</span><span class="sxs-lookup"><span data-stu-id="90300-132">id</span></span>|<span data-ttu-id="90300-133">String</span><span class="sxs-lookup"><span data-stu-id="90300-133">String</span></span>| <span data-ttu-id="90300-134">Уникальный идентификатор объекта sku, подписка на который выполнена.</span><span class="sxs-lookup"><span data-stu-id="90300-134">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="90300-135">Key, не допускающая значение null.</span><span class="sxs-lookup"><span data-stu-id="90300-135">Key, not nullable.</span></span> |
|<span data-ttu-id="90300-136">Препаидунитс</span><span class="sxs-lookup"><span data-stu-id="90300-136">prepaidUnits</span></span>|[<span data-ttu-id="90300-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="90300-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="90300-138">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="90300-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="90300-139">Сервицепланс</span><span class="sxs-lookup"><span data-stu-id="90300-139">servicePlans</span></span>|<span data-ttu-id="90300-140">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="90300-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="90300-141">Сведения о планах обслуживания, доступных в отношении SKU.</span><span class="sxs-lookup"><span data-stu-id="90300-141">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="90300-142">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="90300-142">Not nullable</span></span> |
|<span data-ttu-id="90300-143">skuId</span><span class="sxs-lookup"><span data-stu-id="90300-143">skuId</span></span>|<span data-ttu-id="90300-144">Guid</span><span class="sxs-lookup"><span data-stu-id="90300-144">Guid</span></span>| <span data-ttu-id="90300-145">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="90300-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="90300-146">Скупартнумбер</span><span class="sxs-lookup"><span data-stu-id="90300-146">skuPartNumber</span></span>|<span data-ttu-id="90300-147">String</span><span class="sxs-lookup"><span data-stu-id="90300-147">String</span></span>| <span data-ttu-id="90300-148">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="90300-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="90300-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="90300-149">Relationships</span></span>
<span data-ttu-id="90300-150">Нет</span><span class="sxs-lookup"><span data-stu-id="90300-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90300-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="90300-151">JSON representation</span></span>

<span data-ttu-id="90300-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90300-152">Here is a JSON representation of the resource</span></span>

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
