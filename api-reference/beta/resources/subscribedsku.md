---
title: Тип ресурса subscribedSku
description: " Создание, обновление и удаление не поддерживаются. Выражения фильтра запросов не поддерживаются. Наследуется от directoryObject."
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 528ec916edf049ef48b057afabad943bbb2182cf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520298"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="94d1b-105">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="94d1b-105">subscribedSku resource type</span></span>

<span data-ttu-id="94d1b-106">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="94d1b-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94d1b-107">На подписанных SKU поддерживаются только операции чтения; Создание, обновление и удаление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="94d1b-107">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="94d1b-108">Выражения фильтра запросов не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="94d1b-108">Query filter expressions are not supported.</span></span> <span data-ttu-id="94d1b-109">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="94d1b-109">Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="94d1b-110">Методы</span><span class="sxs-lookup"><span data-stu-id="94d1b-110">Methods</span></span>
| <span data-ttu-id="94d1b-111">Метод</span><span class="sxs-lookup"><span data-stu-id="94d1b-111">Method</span></span>           | <span data-ttu-id="94d1b-112">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="94d1b-112">Return Type</span></span>    |<span data-ttu-id="94d1b-113">Описание</span><span class="sxs-lookup"><span data-stu-id="94d1b-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="94d1b-114">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="94d1b-114">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="94d1b-115">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="94d1b-115">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="94d1b-116">Получение конкретной коммерческой подписки, приобретенной Организацией.</span><span class="sxs-lookup"><span data-stu-id="94d1b-116">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="94d1b-117">Список subscribedsku</span><span class="sxs-lookup"><span data-stu-id="94d1b-117">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="94d1b-118">Коллекция объектов [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="94d1b-118">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="94d1b-119">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="94d1b-119">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="94d1b-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="94d1b-120">Properties</span></span>
| <span data-ttu-id="94d1b-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="94d1b-121">Property</span></span>     | <span data-ttu-id="94d1b-122">Тип</span><span class="sxs-lookup"><span data-stu-id="94d1b-122">Type</span></span>   |<span data-ttu-id="94d1b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="94d1b-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94d1b-124">Тег</span><span class="sxs-lookup"><span data-stu-id="94d1b-124">appliesTo</span></span>|<span data-ttu-id="94d1b-125">String</span><span class="sxs-lookup"><span data-stu-id="94d1b-125">String</span></span>| <span data-ttu-id="94d1b-126">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="94d1b-126">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="94d1b-127">капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="94d1b-127">capabilityStatus</span></span>|<span data-ttu-id="94d1b-128">String</span><span class="sxs-lookup"><span data-stu-id="94d1b-128">String</span></span>| <span data-ttu-id="94d1b-129">Возможные значения: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span><span class="sxs-lookup"><span data-stu-id="94d1b-129">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> |
|<span data-ttu-id="94d1b-130">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="94d1b-130">consumedUnits</span></span>|<span data-ttu-id="94d1b-131">Int32</span><span class="sxs-lookup"><span data-stu-id="94d1b-131">Int32</span></span>| <span data-ttu-id="94d1b-132">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="94d1b-132">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="94d1b-133">id</span><span class="sxs-lookup"><span data-stu-id="94d1b-133">id</span></span>|<span data-ttu-id="94d1b-134">String</span><span class="sxs-lookup"><span data-stu-id="94d1b-134">String</span></span>| <span data-ttu-id="94d1b-135">Уникальный идентификатор объекта sku, подписка на который выполнена.</span><span class="sxs-lookup"><span data-stu-id="94d1b-135">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="94d1b-136">Key, не допускающая значение null.</span><span class="sxs-lookup"><span data-stu-id="94d1b-136">Key, not nullable.</span></span> |
|<span data-ttu-id="94d1b-137">препаидунитс</span><span class="sxs-lookup"><span data-stu-id="94d1b-137">prepaidUnits</span></span>|[<span data-ttu-id="94d1b-138">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="94d1b-138">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="94d1b-139">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="94d1b-139">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="94d1b-140">сервицепланс</span><span class="sxs-lookup"><span data-stu-id="94d1b-140">servicePlans</span></span>|<span data-ttu-id="94d1b-141">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="94d1b-141">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="94d1b-142">Сведения о планах обслуживания, доступных в отношении SKU.</span><span class="sxs-lookup"><span data-stu-id="94d1b-142">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="94d1b-143">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="94d1b-143">Not nullable</span></span> |
|<span data-ttu-id="94d1b-144">skuId</span><span class="sxs-lookup"><span data-stu-id="94d1b-144">skuId</span></span>|<span data-ttu-id="94d1b-145">Guid</span><span class="sxs-lookup"><span data-stu-id="94d1b-145">Guid</span></span>| <span data-ttu-id="94d1b-146">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="94d1b-146">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="94d1b-147">скупартнумбер</span><span class="sxs-lookup"><span data-stu-id="94d1b-147">skuPartNumber</span></span>|<span data-ttu-id="94d1b-148">String</span><span class="sxs-lookup"><span data-stu-id="94d1b-148">String</span></span>| <span data-ttu-id="94d1b-149">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="94d1b-149">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="94d1b-150">Чтобы получить список коммерческих подписок, приобретенных в Организации, ознакомьтесь со статьей [List субскрибедскус](../api/subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="94d1b-150">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="94d1b-151">Связи</span><span class="sxs-lookup"><span data-stu-id="94d1b-151">Relationships</span></span>
<span data-ttu-id="94d1b-152">Нет</span><span class="sxs-lookup"><span data-stu-id="94d1b-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94d1b-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="94d1b-153">JSON representation</span></span>

<span data-ttu-id="94d1b-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="94d1b-154">Here is a JSON representation of the resource</span></span>

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
