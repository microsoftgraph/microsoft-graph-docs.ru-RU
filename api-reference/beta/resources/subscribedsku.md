---
title: Тип ресурса subscribedSku
description: Представляет тип SKU с подпиской.
localization_priority: Normal
author: SumitParikh
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 3d41247ebb88e4941556408fe6fbebbabc54ff8d
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030903"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="05e46-103">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="05e46-103">subscribedSku resource type</span></span>

<span data-ttu-id="05e46-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05e46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05e46-105">Только операция чтения поддерживается в поддерживаемых skUs; создание, обновление и удаление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="05e46-105">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="05e46-106">Выражения фильтра запросов не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="05e46-106">Query filter expressions are not supported.</span></span> <span data-ttu-id="05e46-107">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="05e46-107">Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="05e46-108">Методы</span><span class="sxs-lookup"><span data-stu-id="05e46-108">Methods</span></span>
| <span data-ttu-id="05e46-109">Метод</span><span class="sxs-lookup"><span data-stu-id="05e46-109">Method</span></span>           | <span data-ttu-id="05e46-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="05e46-110">Return Type</span></span>    |<span data-ttu-id="05e46-111">Описание</span><span class="sxs-lookup"><span data-stu-id="05e46-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="05e46-112">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="05e46-112">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="05e46-113">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="05e46-113">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="05e46-114">Получение определенной коммерческой подписки, приобретенной организацией.</span><span class="sxs-lookup"><span data-stu-id="05e46-114">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="05e46-115">Список subscribedsku</span><span class="sxs-lookup"><span data-stu-id="05e46-115">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="05e46-116">Коллекция объектов [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="05e46-116">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="05e46-117">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="05e46-117">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="05e46-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="05e46-118">Properties</span></span>
| <span data-ttu-id="05e46-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="05e46-119">Property</span></span>     | <span data-ttu-id="05e46-120">Тип</span><span class="sxs-lookup"><span data-stu-id="05e46-120">Type</span></span>   |<span data-ttu-id="05e46-121">Описание</span><span class="sxs-lookup"><span data-stu-id="05e46-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05e46-122">appliesTo</span><span class="sxs-lookup"><span data-stu-id="05e46-122">appliesTo</span></span>|<span data-ttu-id="05e46-123">String</span><span class="sxs-lookup"><span data-stu-id="05e46-123">String</span></span>| <span data-ttu-id="05e46-124">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="05e46-124">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="05e46-125">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="05e46-125">capabilityStatus</span></span>|<span data-ttu-id="05e46-126">String</span><span class="sxs-lookup"><span data-stu-id="05e46-126">String</span></span>| <span data-ttu-id="05e46-127">Возможные значения: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span><span class="sxs-lookup"><span data-stu-id="05e46-127">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> <span data-ttu-id="05e46-128">The capabilityStatus is `Enabled` if the **prepaidUnits** property has at least 1 unit that is **enabled,** and `LockedOut` if the customer cancelled their subscription.</span><span class="sxs-lookup"><span data-stu-id="05e46-128">The capabilityStatus is `Enabled` if the **prepaidUnits** property has at least 1 unit that is **enabled**, and `LockedOut` if the customer cancelled their subscription.</span></span> |
|<span data-ttu-id="05e46-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="05e46-129">consumedUnits</span></span>|<span data-ttu-id="05e46-130">Int32</span><span class="sxs-lookup"><span data-stu-id="05e46-130">Int32</span></span>| <span data-ttu-id="05e46-131">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="05e46-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="05e46-132">id</span><span class="sxs-lookup"><span data-stu-id="05e46-132">id</span></span>|<span data-ttu-id="05e46-133">String</span><span class="sxs-lookup"><span data-stu-id="05e46-133">String</span></span>| <span data-ttu-id="05e46-134">Уникальный идентификатор объекта sku, подписка на который выполнена.</span><span class="sxs-lookup"><span data-stu-id="05e46-134">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="05e46-135">Key, not nullable.</span><span class="sxs-lookup"><span data-stu-id="05e46-135">Key, not nullable.</span></span> |
|<span data-ttu-id="05e46-136">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="05e46-136">prepaidUnits</span></span>|[<span data-ttu-id="05e46-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="05e46-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="05e46-138">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="05e46-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="05e46-139">servicePlans</span><span class="sxs-lookup"><span data-stu-id="05e46-139">servicePlans</span></span>|<span data-ttu-id="05e46-140">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="05e46-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="05e46-141">Сведения о планах обслуживания, доступных в отношении SKU.</span><span class="sxs-lookup"><span data-stu-id="05e46-141">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="05e46-142">Не является недействительным</span><span class="sxs-lookup"><span data-stu-id="05e46-142">Not nullable</span></span> |
|<span data-ttu-id="05e46-143">skuId</span><span class="sxs-lookup"><span data-stu-id="05e46-143">skuId</span></span>|<span data-ttu-id="05e46-144">Guid</span><span class="sxs-lookup"><span data-stu-id="05e46-144">Guid</span></span>| <span data-ttu-id="05e46-145">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="05e46-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="05e46-146">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="05e46-146">skuPartNumber</span></span>|<span data-ttu-id="05e46-147">String</span><span class="sxs-lookup"><span data-stu-id="05e46-147">String</span></span>| <span data-ttu-id="05e46-148">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="05e46-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="05e46-149">Чтобы получить список коммерческих подписок, приобретенных организацией, см. в [журнале List subscribedSkus.](../api/subscribedsku-list.md)</span><span class="sxs-lookup"><span data-stu-id="05e46-149">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="05e46-150">Связи</span><span class="sxs-lookup"><span data-stu-id="05e46-150">Relationships</span></span>
<span data-ttu-id="05e46-151">Нет</span><span class="sxs-lookup"><span data-stu-id="05e46-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="05e46-152">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="05e46-152">JSON representation</span></span>

<span data-ttu-id="05e46-153">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="05e46-153">Here is a JSON representation of the resource</span></span>

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


