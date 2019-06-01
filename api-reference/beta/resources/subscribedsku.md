---
title: Тип ресурса subscribedSku
description: " Создание, обновление и удаление не поддерживаются. Выражения фильтра запросов не поддерживаются. Наследуется от directoryObject."
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9763592ee444cbf0ae73ffbad81288bb5fdd76c2
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655119"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="a5b53-105">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="a5b53-105">subscribedSku resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5b53-106">На подписанных SKU поддерживаются только операции чтения; Создание, обновление и удаление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="a5b53-106">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="a5b53-107">Выражения фильтра запросов не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="a5b53-107">Query filter expressions are not supported.</span></span> <span data-ttu-id="a5b53-108">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="a5b53-108">Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="a5b53-109">Методы</span><span class="sxs-lookup"><span data-stu-id="a5b53-109">Methods</span></span>
| <span data-ttu-id="a5b53-110">Метод</span><span class="sxs-lookup"><span data-stu-id="a5b53-110">Method</span></span>           | <span data-ttu-id="a5b53-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a5b53-111">Return Type</span></span>    |<span data-ttu-id="a5b53-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a5b53-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a5b53-113">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="a5b53-113">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="a5b53-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="a5b53-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="a5b53-115">Чтение свойств и связей объекта subscribedSku.</span><span class="sxs-lookup"><span data-stu-id="a5b53-115">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="a5b53-116">Список subscribedsku</span><span class="sxs-lookup"><span data-stu-id="a5b53-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="a5b53-117">Коллекция объектов [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="a5b53-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="a5b53-118">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="a5b53-118">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="a5b53-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="a5b53-119">Properties</span></span>
| <span data-ttu-id="a5b53-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="a5b53-120">Property</span></span>     | <span data-ttu-id="a5b53-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a5b53-121">Type</span></span>   |<span data-ttu-id="a5b53-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a5b53-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5b53-123">Тег</span><span class="sxs-lookup"><span data-stu-id="a5b53-123">appliesTo</span></span>|<span data-ttu-id="a5b53-124">String</span><span class="sxs-lookup"><span data-stu-id="a5b53-124">String</span></span>| <span data-ttu-id="a5b53-125">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="a5b53-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="a5b53-126">Капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="a5b53-126">capabilityStatus</span></span>|<span data-ttu-id="a5b53-127">String</span><span class="sxs-lookup"><span data-stu-id="a5b53-127">String</span></span>| <span data-ttu-id="a5b53-128">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="a5b53-128">For example, "Enabled".</span></span> |
|<span data-ttu-id="a5b53-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="a5b53-129">consumedUnits</span></span>|<span data-ttu-id="a5b53-130">Int32</span><span class="sxs-lookup"><span data-stu-id="a5b53-130">Int32</span></span>| <span data-ttu-id="a5b53-131">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="a5b53-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="a5b53-132">id</span><span class="sxs-lookup"><span data-stu-id="a5b53-132">id</span></span>|<span data-ttu-id="a5b53-133">String</span><span class="sxs-lookup"><span data-stu-id="a5b53-133">String</span></span>| <span data-ttu-id="a5b53-134">Уникальный идентификатор объекта sku, подписка на который выполнена.</span><span class="sxs-lookup"><span data-stu-id="a5b53-134">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="a5b53-135">Key, не допускающая значение null.</span><span class="sxs-lookup"><span data-stu-id="a5b53-135">Key, not nullable.</span></span> |
|<span data-ttu-id="a5b53-136">Препаидунитс</span><span class="sxs-lookup"><span data-stu-id="a5b53-136">prepaidUnits</span></span>|[<span data-ttu-id="a5b53-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="a5b53-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="a5b53-138">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="a5b53-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="a5b53-139">Сервицепланс</span><span class="sxs-lookup"><span data-stu-id="a5b53-139">servicePlans</span></span>|<span data-ttu-id="a5b53-140">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="a5b53-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="a5b53-141">Сведения о планах обслуживания, доступных в отношении SKU.</span><span class="sxs-lookup"><span data-stu-id="a5b53-141">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="a5b53-142">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="a5b53-142">Not nullable</span></span> |
|<span data-ttu-id="a5b53-143">skuId</span><span class="sxs-lookup"><span data-stu-id="a5b53-143">skuId</span></span>|<span data-ttu-id="a5b53-144">Guid</span><span class="sxs-lookup"><span data-stu-id="a5b53-144">Guid</span></span>| <span data-ttu-id="a5b53-145">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="a5b53-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="a5b53-146">Скупартнумбер</span><span class="sxs-lookup"><span data-stu-id="a5b53-146">skuPartNumber</span></span>|<span data-ttu-id="a5b53-147">String</span><span class="sxs-lookup"><span data-stu-id="a5b53-147">String</span></span>| <span data-ttu-id="a5b53-148">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="a5b53-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="a5b53-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="a5b53-149">Relationships</span></span>
<span data-ttu-id="a5b53-150">Нет</span><span class="sxs-lookup"><span data-stu-id="a5b53-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5b53-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a5b53-151">JSON representation</span></span>

<span data-ttu-id="a5b53-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a5b53-152">Here is a JSON representation of the resource</span></span>

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
