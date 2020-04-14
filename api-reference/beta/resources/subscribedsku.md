---
title: Тип ресурса subscribedSku
description: Представляет тип подписанного SKU.
localization_priority: Normal
author: SumitParikh
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 63aafb107a9c95c3dd4fa0c5b3aad33bccdc0174
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43411750"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="c054e-103">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="c054e-103">subscribedSku resource type</span></span>

<span data-ttu-id="c054e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c054e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c054e-105">На подписанных SKU поддерживаются только операции чтения; Создание, обновление и удаление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="c054e-105">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="c054e-106">Выражения фильтра запросов не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="c054e-106">Query filter expressions are not supported.</span></span> <span data-ttu-id="c054e-107">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="c054e-107">Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="c054e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="c054e-108">Methods</span></span>
| <span data-ttu-id="c054e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="c054e-109">Method</span></span>           | <span data-ttu-id="c054e-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c054e-110">Return Type</span></span>    |<span data-ttu-id="c054e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c054e-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c054e-112">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="c054e-112">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="c054e-113">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="c054e-113">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="c054e-114">Получение конкретной коммерческой подписки, приобретенной Организацией.</span><span class="sxs-lookup"><span data-stu-id="c054e-114">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="c054e-115">Список subscribedsku</span><span class="sxs-lookup"><span data-stu-id="c054e-115">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="c054e-116">Коллекция объектов [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="c054e-116">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="c054e-117">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="c054e-117">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="c054e-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="c054e-118">Properties</span></span>
| <span data-ttu-id="c054e-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="c054e-119">Property</span></span>     | <span data-ttu-id="c054e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="c054e-120">Type</span></span>   |<span data-ttu-id="c054e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="c054e-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c054e-122">Тег</span><span class="sxs-lookup"><span data-stu-id="c054e-122">appliesTo</span></span>|<span data-ttu-id="c054e-123">String</span><span class="sxs-lookup"><span data-stu-id="c054e-123">String</span></span>| <span data-ttu-id="c054e-124">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="c054e-124">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="c054e-125">капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="c054e-125">capabilityStatus</span></span>|<span data-ttu-id="c054e-126">String</span><span class="sxs-lookup"><span data-stu-id="c054e-126">String</span></span>| <span data-ttu-id="c054e-127">Возможные значения: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span><span class="sxs-lookup"><span data-stu-id="c054e-127">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> |
|<span data-ttu-id="c054e-128">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="c054e-128">consumedUnits</span></span>|<span data-ttu-id="c054e-129">Int32</span><span class="sxs-lookup"><span data-stu-id="c054e-129">Int32</span></span>| <span data-ttu-id="c054e-130">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="c054e-130">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="c054e-131">id</span><span class="sxs-lookup"><span data-stu-id="c054e-131">id</span></span>|<span data-ttu-id="c054e-132">String</span><span class="sxs-lookup"><span data-stu-id="c054e-132">String</span></span>| <span data-ttu-id="c054e-133">Уникальный идентификатор объекта sku, подписка на который выполнена.</span><span class="sxs-lookup"><span data-stu-id="c054e-133">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="c054e-134">Key, не допускающая значение null.</span><span class="sxs-lookup"><span data-stu-id="c054e-134">Key, not nullable.</span></span> |
|<span data-ttu-id="c054e-135">препаидунитс</span><span class="sxs-lookup"><span data-stu-id="c054e-135">prepaidUnits</span></span>|[<span data-ttu-id="c054e-136">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="c054e-136">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="c054e-137">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="c054e-137">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="c054e-138">сервицепланс</span><span class="sxs-lookup"><span data-stu-id="c054e-138">servicePlans</span></span>|<span data-ttu-id="c054e-139">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="c054e-139">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="c054e-140">Сведения о планах обслуживания, доступных в отношении SKU.</span><span class="sxs-lookup"><span data-stu-id="c054e-140">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="c054e-141">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="c054e-141">Not nullable</span></span> |
|<span data-ttu-id="c054e-142">skuId</span><span class="sxs-lookup"><span data-stu-id="c054e-142">skuId</span></span>|<span data-ttu-id="c054e-143">Guid</span><span class="sxs-lookup"><span data-stu-id="c054e-143">Guid</span></span>| <span data-ttu-id="c054e-144">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="c054e-144">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="c054e-145">скупартнумбер</span><span class="sxs-lookup"><span data-stu-id="c054e-145">skuPartNumber</span></span>|<span data-ttu-id="c054e-146">String</span><span class="sxs-lookup"><span data-stu-id="c054e-146">String</span></span>| <span data-ttu-id="c054e-147">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="c054e-147">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="c054e-148">Чтобы получить список коммерческих подписок, приобретенных в Организации, ознакомьтесь со статьей [List субскрибедскус](../api/subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="c054e-148">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="c054e-149">Связи</span><span class="sxs-lookup"><span data-stu-id="c054e-149">Relationships</span></span>
<span data-ttu-id="c054e-150">Нет</span><span class="sxs-lookup"><span data-stu-id="c054e-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c054e-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c054e-151">JSON representation</span></span>

<span data-ttu-id="c054e-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c054e-152">Here is a JSON representation of the resource</span></span>

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
