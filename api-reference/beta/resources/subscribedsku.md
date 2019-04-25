---
title: Тип ресурса subscribedSku
description: " Создание, обновление и удаление не поддерживаются. Выражения фильтра запросов не поддерживаются. Наследуется от directoryObject."
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 090e6912ce2f337a8e30322c9b45161af73175cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582092"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="bba7d-105">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="bba7d-105">subscribedSku resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bba7d-106">На подписанных SKU поддерживаются только операции чтения; Создание, обновление и удаление не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="bba7d-106">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported.</span></span> <span data-ttu-id="bba7d-107">Выражения фильтра запросов не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="bba7d-107">Query filter expressions are not supported.</span></span> <span data-ttu-id="bba7d-108">Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="bba7d-108">Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="bba7d-109">Методы</span><span class="sxs-lookup"><span data-stu-id="bba7d-109">Methods</span></span>
| <span data-ttu-id="bba7d-110">Метод</span><span class="sxs-lookup"><span data-stu-id="bba7d-110">Method</span></span>           | <span data-ttu-id="bba7d-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bba7d-111">Return Type</span></span>    |<span data-ttu-id="bba7d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bba7d-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bba7d-113">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="bba7d-113">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="bba7d-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="bba7d-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="bba7d-115">Чтение свойств и связей объекта subscribedSku.</span><span class="sxs-lookup"><span data-stu-id="bba7d-115">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="bba7d-116">Список subscribedsku</span><span class="sxs-lookup"><span data-stu-id="bba7d-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="bba7d-117">Коллекция объектов [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="bba7d-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="bba7d-118">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="bba7d-118">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="bba7d-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="bba7d-119">Properties</span></span>
| <span data-ttu-id="bba7d-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="bba7d-120">Property</span></span>     | <span data-ttu-id="bba7d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="bba7d-121">Type</span></span>   |<span data-ttu-id="bba7d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bba7d-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bba7d-123">Тег</span><span class="sxs-lookup"><span data-stu-id="bba7d-123">appliesTo</span></span>|<span data-ttu-id="bba7d-124">String</span><span class="sxs-lookup"><span data-stu-id="bba7d-124">String</span></span>| <span data-ttu-id="bba7d-125">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="bba7d-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="bba7d-126">Капабилитистатус</span><span class="sxs-lookup"><span data-stu-id="bba7d-126">capabilityStatus</span></span>|<span data-ttu-id="bba7d-127">String</span><span class="sxs-lookup"><span data-stu-id="bba7d-127">String</span></span>| <span data-ttu-id="bba7d-128">Пример: "Enabled".</span><span class="sxs-lookup"><span data-stu-id="bba7d-128">For example, "Enabled".</span></span> |
|<span data-ttu-id="bba7d-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="bba7d-129">consumedUnits</span></span>|<span data-ttu-id="bba7d-130">Int32</span><span class="sxs-lookup"><span data-stu-id="bba7d-130">Int32</span></span>| <span data-ttu-id="bba7d-131">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="bba7d-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="bba7d-132">id</span><span class="sxs-lookup"><span data-stu-id="bba7d-132">id</span></span>|<span data-ttu-id="bba7d-133">String</span><span class="sxs-lookup"><span data-stu-id="bba7d-133">String</span></span>| <span data-ttu-id="bba7d-134">Уникальный идентификатор объекта sku, подписка на который выполнена.</span><span class="sxs-lookup"><span data-stu-id="bba7d-134">The unique identifier for the subscribed sku object.</span></span> <span data-ttu-id="bba7d-135">Key, не допускающая значение null.</span><span class="sxs-lookup"><span data-stu-id="bba7d-135">Key, not nullable.</span></span> |
|<span data-ttu-id="bba7d-136">Препаидунитс</span><span class="sxs-lookup"><span data-stu-id="bba7d-136">prepaidUnits</span></span>|[<span data-ttu-id="bba7d-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="bba7d-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="bba7d-138">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="bba7d-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="bba7d-139">Сервицепланс</span><span class="sxs-lookup"><span data-stu-id="bba7d-139">servicePlans</span></span>|<span data-ttu-id="bba7d-140">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="bba7d-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="bba7d-141">Сведения о планах обслуживания, доступных в отношении SKU.</span><span class="sxs-lookup"><span data-stu-id="bba7d-141">Information about the service plans that are available with the SKU.</span></span> <span data-ttu-id="bba7d-142">Не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="bba7d-142">Not nullable</span></span> |
|<span data-ttu-id="bba7d-143">skuId</span><span class="sxs-lookup"><span data-stu-id="bba7d-143">skuId</span></span>|<span data-ttu-id="bba7d-144">Guid</span><span class="sxs-lookup"><span data-stu-id="bba7d-144">Guid</span></span>| <span data-ttu-id="bba7d-145">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="bba7d-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="bba7d-146">Скупартнумбер</span><span class="sxs-lookup"><span data-stu-id="bba7d-146">skuPartNumber</span></span>|<span data-ttu-id="bba7d-147">String</span><span class="sxs-lookup"><span data-stu-id="bba7d-147">String</span></span>| <span data-ttu-id="bba7d-148">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="bba7d-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="bba7d-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="bba7d-149">Relationships</span></span>
<span data-ttu-id="bba7d-150">Нет</span><span class="sxs-lookup"><span data-stu-id="bba7d-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bba7d-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bba7d-151">JSON representation</span></span>

<span data-ttu-id="bba7d-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bba7d-152">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/subscribedsku.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
