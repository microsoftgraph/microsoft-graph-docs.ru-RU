---
title: Тип ресурса subscribedSku
description: Представляет тип подписанного SKU.
localization_priority: Normal
author: SumitParikh
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 63aafb107a9c95c3dd4fa0c5b3aad33bccdc0174
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "43411750"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="6f994-103">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="6f994-103">subscribedSku resource type</span></span>

<span data-ttu-id="6f994-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f994-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f994-105">На подписанных SKU поддерживаются только операции чтения; Создание, обновление и удаление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="6f994-105">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="6f994-106">Выражения фильтра запросов не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="6f994-106">Query filter expressions are not supported.</span></span> <span data-ttu-id="6f994-107">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="6f994-107">Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="6f994-108">Методы</span><span class="sxs-lookup"><span data-stu-id="6f994-108">Methods</span></span>
| <span data-ttu-id="6f994-109">Метод</span><span class="sxs-lookup"><span data-stu-id="6f994-109">Method</span></span>           | <span data-ttu-id="6f994-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="6f994-110">Return Type</span></span>    |<span data-ttu-id="6f994-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6f994-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6f994-112">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="6f994-112">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="6f994-113">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="6f994-113">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="6f994-114">Получение конкретной коммерческой подписки, приобретенной Организацией.</span><span class="sxs-lookup"><span data-stu-id="6f994-114">Get a specific commercial subscription that an organization has acquired.</span></span>|
|[<span data-ttu-id="6f994-115">Список subscribedsku</span><span class="sxs-lookup"><span data-stu-id="6f994-115">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="6f994-116">Коллекция объектов [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="6f994-116">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="6f994-117">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="6f994-117">Get the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="6f994-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f994-118">Properties</span></span>
| <span data-ttu-id="6f994-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f994-119">Property</span></span>     | <span data-ttu-id="6f994-120">Тип</span><span class="sxs-lookup"><span data-stu-id="6f994-120">Type</span></span>   |<span data-ttu-id="6f994-121">Описание</span><span class="sxs-lookup"><span data-stu-id="6f994-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f994-122">Тег</span><span class="sxs-lookup"><span data-stu-id="6f994-122">appliesTo</span></span>|<span data-ttu-id="6f994-123">String</span><span class="sxs-lookup"><span data-stu-id="6f994-123">String</span></span>| <span data-ttu-id="6f994-124">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="6f994-124">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="6f994-125">капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="6f994-125">capabilityStatus</span></span>|<span data-ttu-id="6f994-126">String</span><span class="sxs-lookup"><span data-stu-id="6f994-126">String</span></span>| <span data-ttu-id="6f994-127">Возможные значения: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span><span class="sxs-lookup"><span data-stu-id="6f994-127">Possible values are: `Enabled`, `Warning`, `Suspended`, `Deleted`, `LockedOut`.</span></span> |
|<span data-ttu-id="6f994-128">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="6f994-128">consumedUnits</span></span>|<span data-ttu-id="6f994-129">Int32</span><span class="sxs-lookup"><span data-stu-id="6f994-129">Int32</span></span>| <span data-ttu-id="6f994-130">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="6f994-130">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="6f994-131">id</span><span class="sxs-lookup"><span data-stu-id="6f994-131">id</span></span>|<span data-ttu-id="6f994-132">String</span><span class="sxs-lookup"><span data-stu-id="6f994-132">String</span></span>| <span data-ttu-id="6f994-133">Уникальный идентификатор объекта sku, подписка на который выполнена.</span><span class="sxs-lookup"><span data-stu-id="6f994-133">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="6f994-134">Key, не допускающая значение null.</span><span class="sxs-lookup"><span data-stu-id="6f994-134">Key, not nullable.</span></span> |
|<span data-ttu-id="6f994-135">препаидунитс</span><span class="sxs-lookup"><span data-stu-id="6f994-135">prepaidUnits</span></span>|[<span data-ttu-id="6f994-136">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="6f994-136">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="6f994-137">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="6f994-137">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="6f994-138">сервицепланс</span><span class="sxs-lookup"><span data-stu-id="6f994-138">servicePlans</span></span>|<span data-ttu-id="6f994-139">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="6f994-139">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="6f994-140">Сведения о планах обслуживания, доступных в отношении SKU.</span><span class="sxs-lookup"><span data-stu-id="6f994-140">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="6f994-141">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="6f994-141">Not nullable</span></span> |
|<span data-ttu-id="6f994-142">skuId</span><span class="sxs-lookup"><span data-stu-id="6f994-142">skuId</span></span>|<span data-ttu-id="6f994-143">Guid</span><span class="sxs-lookup"><span data-stu-id="6f994-143">Guid</span></span>| <span data-ttu-id="6f994-144">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="6f994-144">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="6f994-145">скупартнумбер</span><span class="sxs-lookup"><span data-stu-id="6f994-145">skuPartNumber</span></span>|<span data-ttu-id="6f994-146">String</span><span class="sxs-lookup"><span data-stu-id="6f994-146">String</span></span>| <span data-ttu-id="6f994-147">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="6f994-147">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> <span data-ttu-id="6f994-148">Чтобы получить список коммерческих подписок, приобретенных в Организации, ознакомьтесь со статьей [List субскрибедскус](../api/subscribedsku-list.md).</span><span class="sxs-lookup"><span data-stu-id="6f994-148">To get a list of commercial subscriptions that an organization has acquired, see [List subscribedSkus](../api/subscribedsku-list.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="6f994-149">Связи</span><span class="sxs-lookup"><span data-stu-id="6f994-149">Relationships</span></span>
<span data-ttu-id="6f994-150">Нет</span><span class="sxs-lookup"><span data-stu-id="6f994-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f994-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f994-151">JSON representation</span></span>

<span data-ttu-id="6f994-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f994-152">Here is a JSON representation of the resource</span></span>

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
