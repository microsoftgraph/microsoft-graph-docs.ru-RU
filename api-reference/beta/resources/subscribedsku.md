---
title: Тип ресурса subscribedSku
description: Представляет тип SKU с подпиской.
localization_priority: Normal
author: SumitParikh
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ff7170a8058be986c7af6b7c2ebd53f47b7ffb82
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433119"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="287d7-103">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="287d7-103">subscribedSku resource type</span></span>

<span data-ttu-id="287d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="287d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="287d7-105">Только операция чтения поддерживается в поддерживаемых skUs; создание, обновление и удаление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="287d7-105">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="287d7-106">Выражения фильтра запросов не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="287d7-106">Query filter expressions are not supported.</span></span> <span data-ttu-id="287d7-107">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="287d7-107">Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="287d7-108">Методы</span><span class="sxs-lookup"><span data-stu-id="287d7-108">Methods</span></span>
| <span data-ttu-id="287d7-109">Метод</span><span class="sxs-lookup"><span data-stu-id="287d7-109">Method</span></span>           | <span data-ttu-id="287d7-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="287d7-110">Return Type</span></span>    |<span data-ttu-id="287d7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="287d7-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="287d7-112">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="287d7-112">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="287d7-113">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="287d7-113">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="287d7-114">Получение определенной коммерческой подписки, приобретенной организацией.</span><span class="sxs-lookup"><span data-stu-id="287d7-114">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="287d7-115">Список subscribedsku</span><span class="sxs-lookup"><span data-stu-id="287d7-115">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="287d7-116">Коллекция объектов [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="287d7-116">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="287d7-117">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="287d7-117">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="287d7-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="287d7-118">Properties</span></span>
| <span data-ttu-id="287d7-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="287d7-119">Property</span></span>     | <span data-ttu-id="287d7-120">Тип</span><span class="sxs-lookup"><span data-stu-id="287d7-120">Type</span></span>   |<span data-ttu-id="287d7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="287d7-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="287d7-122">appliesTo</span><span class="sxs-lookup"><span data-stu-id="287d7-122">appliesTo</span></span>|<span data-ttu-id="287d7-123">String</span><span class="sxs-lookup"><span data-stu-id="287d7-123">String</span></span>| <span data-ttu-id="287d7-124">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="287d7-124">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="287d7-125">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="287d7-125">capabilityStatus</span></span>|<span data-ttu-id="287d7-126">String</span><span class="sxs-lookup"><span data-stu-id="287d7-126">String</span></span>| <span data-ttu-id="287d7-127">Возможные значения: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span><span class="sxs-lookup"><span data-stu-id="287d7-127">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> |
|<span data-ttu-id="287d7-128">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="287d7-128">consumedUnits</span></span>|<span data-ttu-id="287d7-129">Int32</span><span class="sxs-lookup"><span data-stu-id="287d7-129">Int32</span></span>| <span data-ttu-id="287d7-130">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="287d7-130">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="287d7-131">id</span><span class="sxs-lookup"><span data-stu-id="287d7-131">id</span></span>|<span data-ttu-id="287d7-132">String</span><span class="sxs-lookup"><span data-stu-id="287d7-132">String</span></span>| <span data-ttu-id="287d7-133">Уникальный идентификатор объекта sku, подписка на который выполнена.</span><span class="sxs-lookup"><span data-stu-id="287d7-133">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="287d7-134">Key, not nullable.</span><span class="sxs-lookup"><span data-stu-id="287d7-134">Key, not nullable.</span></span> |
|<span data-ttu-id="287d7-135">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="287d7-135">prepaidUnits</span></span>|[<span data-ttu-id="287d7-136">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="287d7-136">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="287d7-137">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="287d7-137">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="287d7-138">servicePlans</span><span class="sxs-lookup"><span data-stu-id="287d7-138">servicePlans</span></span>|<span data-ttu-id="287d7-139">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="287d7-139">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="287d7-140">Сведения о планах обслуживания, доступных в отношении SKU.</span><span class="sxs-lookup"><span data-stu-id="287d7-140">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="287d7-141">Не является недействительным</span><span class="sxs-lookup"><span data-stu-id="287d7-141">Not nullable</span></span> |
|<span data-ttu-id="287d7-142">skuId</span><span class="sxs-lookup"><span data-stu-id="287d7-142">skuId</span></span>|<span data-ttu-id="287d7-143">Guid</span><span class="sxs-lookup"><span data-stu-id="287d7-143">Guid</span></span>| <span data-ttu-id="287d7-144">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="287d7-144">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="287d7-145">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="287d7-145">skuPartNumber</span></span>|<span data-ttu-id="287d7-146">String</span><span class="sxs-lookup"><span data-stu-id="287d7-146">String</span></span>| <span data-ttu-id="287d7-147">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="287d7-147">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="287d7-148">Чтобы получить список коммерческих подписок, приобретенных организацией, см. в [журнале List subscribedSkus.](../api/subscribedsku-list.md)</span><span class="sxs-lookup"><span data-stu-id="287d7-148">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="287d7-149">Связи</span><span class="sxs-lookup"><span data-stu-id="287d7-149">Relationships</span></span>
<span data-ttu-id="287d7-150">Нет</span><span class="sxs-lookup"><span data-stu-id="287d7-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="287d7-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="287d7-151">JSON representation</span></span>

<span data-ttu-id="287d7-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="287d7-152">Here is a JSON representation of the resource</span></span>

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


