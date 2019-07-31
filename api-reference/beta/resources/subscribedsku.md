---
title: Тип ресурса subscribedSku
description: " Создание, обновление и удаление не поддерживаются. Выражения фильтра запросов не поддерживаются. Наследуется от directoryObject."
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9e57ff1e59c7caf5b29e582b7381492a7eee5b4c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964833"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="1313c-105">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="1313c-105">subscribedSku resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1313c-106">На подписанных SKU поддерживаются только операции чтения; Создание, обновление и удаление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="1313c-106">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="1313c-107">Выражения фильтра запросов не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="1313c-107">Query filter expressions are not supported.</span></span> <span data-ttu-id="1313c-108">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="1313c-108">Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="1313c-109">Методы</span><span class="sxs-lookup"><span data-stu-id="1313c-109">Methods</span></span>
| <span data-ttu-id="1313c-110">Метод</span><span class="sxs-lookup"><span data-stu-id="1313c-110">Method</span></span>           | <span data-ttu-id="1313c-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1313c-111">Return Type</span></span>    |<span data-ttu-id="1313c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1313c-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1313c-113">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="1313c-113">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="1313c-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="1313c-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="1313c-115">Получение конкретной коммерческой подписки, приобретенной Организацией.</span><span class="sxs-lookup"><span data-stu-id="1313c-115">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="1313c-116">Список subscribedsku</span><span class="sxs-lookup"><span data-stu-id="1313c-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="1313c-117">Коллекция объектов [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="1313c-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="1313c-118">Получение списка коммерческих подписок, приобретенных Организацией.</span><span class="sxs-lookup"><span data-stu-id="1313c-118">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="1313c-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="1313c-119">Properties</span></span>
| <span data-ttu-id="1313c-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="1313c-120">Property</span></span>     | <span data-ttu-id="1313c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="1313c-121">Type</span></span>   |<span data-ttu-id="1313c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="1313c-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1313c-123">Тег</span><span class="sxs-lookup"><span data-stu-id="1313c-123">appliesTo</span></span>|<span data-ttu-id="1313c-124">String</span><span class="sxs-lookup"><span data-stu-id="1313c-124">String</span></span>| <span data-ttu-id="1313c-125">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="1313c-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="1313c-126">Капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="1313c-126">capabilityStatus</span></span>|<span data-ttu-id="1313c-127">String</span><span class="sxs-lookup"><span data-stu-id="1313c-127">String</span></span>| <span data-ttu-id="1313c-128">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="1313c-128">For example, "Enabled".</span></span> |
|<span data-ttu-id="1313c-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="1313c-129">consumedUnits</span></span>|<span data-ttu-id="1313c-130">Int32</span><span class="sxs-lookup"><span data-stu-id="1313c-130">Int32</span></span>| <span data-ttu-id="1313c-131">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="1313c-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="1313c-132">id</span><span class="sxs-lookup"><span data-stu-id="1313c-132">id</span></span>|<span data-ttu-id="1313c-133">String</span><span class="sxs-lookup"><span data-stu-id="1313c-133">String</span></span>| <span data-ttu-id="1313c-134">Уникальный идентификатор объекта sku, подписка на который выполнена.</span><span class="sxs-lookup"><span data-stu-id="1313c-134">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="1313c-135">Key, не допускающая значение null.</span><span class="sxs-lookup"><span data-stu-id="1313c-135">Key, not nullable.</span></span> |
|<span data-ttu-id="1313c-136">Препаидунитс</span><span class="sxs-lookup"><span data-stu-id="1313c-136">prepaidUnits</span></span>|[<span data-ttu-id="1313c-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="1313c-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="1313c-138">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="1313c-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="1313c-139">Сервицепланс</span><span class="sxs-lookup"><span data-stu-id="1313c-139">servicePlans</span></span>|<span data-ttu-id="1313c-140">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="1313c-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="1313c-141">Сведения о планах обслуживания, доступных в отношении SKU.</span><span class="sxs-lookup"><span data-stu-id="1313c-141">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="1313c-142">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="1313c-142">Not nullable</span></span> |
|<span data-ttu-id="1313c-143">skuId</span><span class="sxs-lookup"><span data-stu-id="1313c-143">skuId</span></span>|<span data-ttu-id="1313c-144">Guid</span><span class="sxs-lookup"><span data-stu-id="1313c-144">Guid</span></span>| <span data-ttu-id="1313c-145">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="1313c-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="1313c-146">Скупартнумбер</span><span class="sxs-lookup"><span data-stu-id="1313c-146">skuPartNumber</span></span>|<span data-ttu-id="1313c-147">String</span><span class="sxs-lookup"><span data-stu-id="1313c-147">String</span></span>| <span data-ttu-id="1313c-148">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="1313c-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="1313c-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="1313c-149">Relationships</span></span>
<span data-ttu-id="1313c-150">Нет</span><span class="sxs-lookup"><span data-stu-id="1313c-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1313c-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1313c-151">JSON representation</span></span>

<span data-ttu-id="1313c-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1313c-152">Here is a JSON representation of the resource</span></span>

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
