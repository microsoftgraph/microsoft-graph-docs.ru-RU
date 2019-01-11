---
title: Тип ресурса subscribedSku
description: Содержит сведения о SKU службы, на которую компания подписана.
localization_priority: Normal
ms.openlocfilehash: 17290890ff27fded1aaf5d7fdb2c0cdacee09b0c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873719"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="372c0-103">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="372c0-103">subscribedSku resource type</span></span>

<span data-ttu-id="372c0-104">Содержит сведения о SKU службы, на которую компания подписана.</span><span class="sxs-lookup"><span data-stu-id="372c0-104">Contains information about a service SKU that a company is subscribed to.</span></span>

<span data-ttu-id="372c0-p101">В подписанных SKU поддерживается только операция чтения. Создание, обновление и удаление не поддерживаются. Выражения фильтра запроса не поддерживаются. Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="372c0-p101">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>

## <a name="methods"></a><span data-ttu-id="372c0-108">Методы</span><span class="sxs-lookup"><span data-stu-id="372c0-108">Methods</span></span>
| <span data-ttu-id="372c0-109">Метод</span><span class="sxs-lookup"><span data-stu-id="372c0-109">Method</span></span>           | <span data-ttu-id="372c0-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="372c0-110">Return Type</span></span>    |<span data-ttu-id="372c0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="372c0-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="372c0-112">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="372c0-112">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="372c0-113">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="372c0-113">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="372c0-114">Чтение свойств и связей объекта subscribedSku.</span><span class="sxs-lookup"><span data-stu-id="372c0-114">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="372c0-115">Список subscribedsku</span><span class="sxs-lookup"><span data-stu-id="372c0-115">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="372c0-116">Коллекция объектов [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="372c0-116">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="372c0-117">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="372c0-117">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="372c0-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="372c0-118">Properties</span></span>
| <span data-ttu-id="372c0-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="372c0-119">Property</span></span>     | <span data-ttu-id="372c0-120">Тип</span><span class="sxs-lookup"><span data-stu-id="372c0-120">Type</span></span>   |<span data-ttu-id="372c0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="372c0-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="372c0-122">appliesTo</span><span class="sxs-lookup"><span data-stu-id="372c0-122">appliesTo</span></span>|<span data-ttu-id="372c0-123">String</span><span class="sxs-lookup"><span data-stu-id="372c0-123">String</span></span>| <span data-ttu-id="372c0-124">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="372c0-124">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="372c0-125">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="372c0-125">capabilityStatus</span></span>|<span data-ttu-id="372c0-126">Строка</span><span class="sxs-lookup"><span data-stu-id="372c0-126">String</span></span>| <span data-ttu-id="372c0-127">Например, Enabled.</span><span class="sxs-lookup"><span data-stu-id="372c0-127">For example, "Enabled".</span></span> |
|<span data-ttu-id="372c0-128">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="372c0-128">consumedUnits</span></span>|<span data-ttu-id="372c0-129">Int32</span><span class="sxs-lookup"><span data-stu-id="372c0-129">Int32</span></span>| <span data-ttu-id="372c0-130">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="372c0-130">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="372c0-131">id</span><span class="sxs-lookup"><span data-stu-id="372c0-131">id</span></span>|<span data-ttu-id="372c0-132">String</span><span class="sxs-lookup"><span data-stu-id="372c0-132">String</span></span>| <span data-ttu-id="372c0-p102">Уникальный идентификатор объекта sku, подписка на который выполнена. Ключ, значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="372c0-p102">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="372c0-135">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="372c0-135">prepaidUnits</span></span>|[<span data-ttu-id="372c0-136">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="372c0-136">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="372c0-137">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="372c0-137">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="372c0-138">servicePlans</span><span class="sxs-lookup"><span data-stu-id="372c0-138">servicePlans</span></span>|<span data-ttu-id="372c0-139">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="372c0-139">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="372c0-p103">Сведения о планах обслуживания, доступных в отношении SKU. Значение NULL не допускается</span><span class="sxs-lookup"><span data-stu-id="372c0-p103">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="372c0-142">skuId</span><span class="sxs-lookup"><span data-stu-id="372c0-142">skuId</span></span>|<span data-ttu-id="372c0-143">Guid</span><span class="sxs-lookup"><span data-stu-id="372c0-143">Guid</span></span>| <span data-ttu-id="372c0-144">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="372c0-144">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="372c0-145">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="372c0-145">skuPartNumber</span></span>|<span data-ttu-id="372c0-146">String</span><span class="sxs-lookup"><span data-stu-id="372c0-146">String</span></span>| <span data-ttu-id="372c0-147">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="372c0-147">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="372c0-148">Отношения</span><span class="sxs-lookup"><span data-stu-id="372c0-148">Relationships</span></span>
<span data-ttu-id="372c0-149">Нет</span><span class="sxs-lookup"><span data-stu-id="372c0-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="372c0-150">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="372c0-150">JSON representation</span></span>

<span data-ttu-id="372c0-151">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="372c0-151">Here is a JSON representation of the resource</span></span>

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
