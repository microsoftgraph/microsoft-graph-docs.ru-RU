---
title: Тип ресурса subscribedSku
description: " Создание, обновление и удаление не поддерживается. Выражения фильтра запроса не поддерживается. Наследуется от directoryObject."
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 090e6912ce2f337a8e30322c9b45161af73175cc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522702"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="04b38-105">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="04b38-105">subscribedSku resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04b38-p102">В подписанных SKU поддерживается только операция чтения. Создание, обновление и удаление не поддерживаются. Выражения фильтра запроса не поддерживаются. Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="04b38-p102">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="04b38-109">Методы</span><span class="sxs-lookup"><span data-stu-id="04b38-109">Methods</span></span>
| <span data-ttu-id="04b38-110">Метод</span><span class="sxs-lookup"><span data-stu-id="04b38-110">Method</span></span>           | <span data-ttu-id="04b38-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="04b38-111">Return Type</span></span>    |<span data-ttu-id="04b38-112">Описание</span><span class="sxs-lookup"><span data-stu-id="04b38-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04b38-113">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="04b38-113">[Get subscribedSku](../api/subscribedsku-get.md)</span></span> | [<span data-ttu-id="04b38-114">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="04b38-114">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="04b38-115">Чтение свойств и связей объекта subscribedSku.</span><span class="sxs-lookup"><span data-stu-id="04b38-115">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="04b38-116">Список объектов subscribedSku</span><span class="sxs-lookup"><span data-stu-id="04b38-116">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="04b38-117">Коллекция объектов [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="04b38-117">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="04b38-118">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="04b38-118">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="04b38-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="04b38-119">Properties</span></span>
| <span data-ttu-id="04b38-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="04b38-120">Property</span></span>     | <span data-ttu-id="04b38-121">Тип</span><span class="sxs-lookup"><span data-stu-id="04b38-121">Type</span></span>   |<span data-ttu-id="04b38-122">Описание</span><span class="sxs-lookup"><span data-stu-id="04b38-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="04b38-123">appliesTo</span><span class="sxs-lookup"><span data-stu-id="04b38-123">appliesTo</span></span>|<span data-ttu-id="04b38-124">String</span><span class="sxs-lookup"><span data-stu-id="04b38-124">String</span></span>| <span data-ttu-id="04b38-125">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="04b38-125">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="04b38-126">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="04b38-126">capabilityStatus</span></span>|<span data-ttu-id="04b38-127">Строка</span><span class="sxs-lookup"><span data-stu-id="04b38-127">String</span></span>| <span data-ttu-id="04b38-128">Например, Enabled.</span><span class="sxs-lookup"><span data-stu-id="04b38-128">For example, "Enabled".</span></span> |
|<span data-ttu-id="04b38-129">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="04b38-129">consumedUnits</span></span>|<span data-ttu-id="04b38-130">Int32</span><span class="sxs-lookup"><span data-stu-id="04b38-130">Int32</span></span>| <span data-ttu-id="04b38-131">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="04b38-131">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="04b38-132">id</span><span class="sxs-lookup"><span data-stu-id="04b38-132">id</span></span>|<span data-ttu-id="04b38-133">String</span><span class="sxs-lookup"><span data-stu-id="04b38-133">String</span></span>| <span data-ttu-id="04b38-p103">Уникальный идентификатор объекта sku, подписка на который выполнена. Ключ, значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="04b38-p103">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="04b38-136">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="04b38-136">prepaidUnits</span></span>|[<span data-ttu-id="04b38-137">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="04b38-137">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="04b38-138">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="04b38-138">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="04b38-139">servicePlans</span><span class="sxs-lookup"><span data-stu-id="04b38-139">servicePlans</span></span>|<span data-ttu-id="04b38-140">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="04b38-140">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="04b38-p104">Сведения о планах обслуживания, доступных в отношении SKU. Значение NULL не допускается</span><span class="sxs-lookup"><span data-stu-id="04b38-p104">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="04b38-143">skuId</span><span class="sxs-lookup"><span data-stu-id="04b38-143">skuId</span></span>|<span data-ttu-id="04b38-144">Guid</span><span class="sxs-lookup"><span data-stu-id="04b38-144">Guid</span></span>| <span data-ttu-id="04b38-145">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="04b38-145">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="04b38-146">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="04b38-146">skuPartNumber</span></span>|<span data-ttu-id="04b38-147">String</span><span class="sxs-lookup"><span data-stu-id="04b38-147">String</span></span>| <span data-ttu-id="04b38-148">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="04b38-148">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="04b38-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="04b38-149">Relationships</span></span>
<span data-ttu-id="04b38-150">Нет</span><span class="sxs-lookup"><span data-stu-id="04b38-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04b38-151">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04b38-151">JSON representation</span></span>

<span data-ttu-id="04b38-152">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04b38-152">Here is a JSON representation of the resource</span></span>

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
