---
title: Тип ресурса subscribedSku
description: " Создание, обновление и удаление не поддерживаются. Выражения фильтра запросов не поддерживаются. Наследуется от directoryObject."
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4096860b3c45f525a57d208c6f70f1f1087d552d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345737"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="64edd-105">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="64edd-105">subscribedSku resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64edd-106">На подписанных SKU поддерживаются только операции чтения; Создание, обновление и удаление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="64edd-106">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="64edd-107">Выражения фильтра запросов не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="64edd-107">Query filter expressions are not supported.</span></span> <span data-ttu-id="64edd-108">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="64edd-108">Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="64edd-109">Методы</span><span class="sxs-lookup"><span data-stu-id="64edd-109">Methods</span></span>
| <span data-ttu-id="64edd-110">Метод</span><span class="sxs-lookup"><span data-stu-id="64edd-110">Method</span></span>           | <span data-ttu-id="64edd-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="64edd-111">Return Type</span></span>    |<span data-ttu-id="64edd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="64edd-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="64edd-113">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="64edd-113">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="64edd-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="64edd-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="64edd-115">Чтение свойств и связей объекта subscribedSku.</span><span class="sxs-lookup"><span data-stu-id="64edd-115">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="64edd-116">Список subscribedsku</span><span class="sxs-lookup"><span data-stu-id="64edd-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="64edd-117">Коллекция объектов [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="64edd-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="64edd-118">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="64edd-118">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="64edd-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="64edd-119">Properties</span></span>
| <span data-ttu-id="64edd-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="64edd-120">Property</span></span>     | <span data-ttu-id="64edd-121">Тип</span><span class="sxs-lookup"><span data-stu-id="64edd-121">Type</span></span>   |<span data-ttu-id="64edd-122">Описание</span><span class="sxs-lookup"><span data-stu-id="64edd-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64edd-123">Тег</span><span class="sxs-lookup"><span data-stu-id="64edd-123">appliesTo</span></span>|<span data-ttu-id="64edd-124">String</span><span class="sxs-lookup"><span data-stu-id="64edd-124">String</span></span>| <span data-ttu-id="64edd-125">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="64edd-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="64edd-126">Капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="64edd-126">capabilityStatus</span></span>|<span data-ttu-id="64edd-127">String</span><span class="sxs-lookup"><span data-stu-id="64edd-127">String</span></span>| <span data-ttu-id="64edd-128">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="64edd-128">For example, "Enabled".</span></span> |
|<span data-ttu-id="64edd-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="64edd-129">consumedUnits</span></span>|<span data-ttu-id="64edd-130">Int32</span><span class="sxs-lookup"><span data-stu-id="64edd-130">Int32</span></span>| <span data-ttu-id="64edd-131">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="64edd-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="64edd-132">id</span><span class="sxs-lookup"><span data-stu-id="64edd-132">id</span></span>|<span data-ttu-id="64edd-133">String</span><span class="sxs-lookup"><span data-stu-id="64edd-133">String</span></span>| <span data-ttu-id="64edd-134">Уникальный идентификатор объекта sku, подписка на который выполнена.</span><span class="sxs-lookup"><span data-stu-id="64edd-134">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="64edd-135">Key, не допускающая значение null.</span><span class="sxs-lookup"><span data-stu-id="64edd-135">Key, not nullable.</span></span> |
|<span data-ttu-id="64edd-136">Препаидунитс</span><span class="sxs-lookup"><span data-stu-id="64edd-136">prepaidUnits</span></span>|[<span data-ttu-id="64edd-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="64edd-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="64edd-138">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="64edd-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="64edd-139">Сервицепланс</span><span class="sxs-lookup"><span data-stu-id="64edd-139">servicePlans</span></span>|<span data-ttu-id="64edd-140">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="64edd-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="64edd-141">Сведения о планах обслуживания, доступных в отношении SKU.</span><span class="sxs-lookup"><span data-stu-id="64edd-141">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="64edd-142">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="64edd-142">Not nullable</span></span> |
|<span data-ttu-id="64edd-143">skuId</span><span class="sxs-lookup"><span data-stu-id="64edd-143">skuId</span></span>|<span data-ttu-id="64edd-144">Guid</span><span class="sxs-lookup"><span data-stu-id="64edd-144">Guid</span></span>| <span data-ttu-id="64edd-145">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="64edd-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="64edd-146">Скупартнумбер</span><span class="sxs-lookup"><span data-stu-id="64edd-146">skuPartNumber</span></span>|<span data-ttu-id="64edd-147">String</span><span class="sxs-lookup"><span data-stu-id="64edd-147">String</span></span>| <span data-ttu-id="64edd-148">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="64edd-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="64edd-149">Связи</span><span class="sxs-lookup"><span data-stu-id="64edd-149">Relationships</span></span>
<span data-ttu-id="64edd-150">Нет</span><span class="sxs-lookup"><span data-stu-id="64edd-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64edd-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="64edd-151">JSON representation</span></span>

<span data-ttu-id="64edd-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="64edd-152">Here is a JSON representation of the resource</span></span>

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
