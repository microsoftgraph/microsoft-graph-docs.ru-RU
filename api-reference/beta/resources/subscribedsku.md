---
title: Тип ресурса subscribedSku
description: " Создание, обновление и удаление не поддерживается. Выражения фильтра запроса не поддерживается. Наследуется от directoryObject."
localization_priority: Normal
ms.openlocfilehash: 07f40c766d7f46974cf99b9954f63a61c2c0c621
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829605"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="e1b9a-105">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="e1b9a-105">subscribedSku resource type</span></span>

> <span data-ttu-id="e1b9a-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e1b9a-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1b9a-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1b9a-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e1b9a-p103">В подписанных SKU поддерживается только операция чтения. Создание, обновление и удаление не поддерживаются. Выражения фильтра запроса не поддерживаются. Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="e1b9a-p103">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="e1b9a-111">Методы</span><span class="sxs-lookup"><span data-stu-id="e1b9a-111">Methods</span></span>
| <span data-ttu-id="e1b9a-112">Метод</span><span class="sxs-lookup"><span data-stu-id="e1b9a-112">Method</span></span>           | <span data-ttu-id="e1b9a-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e1b9a-113">Return Type</span></span>    |<span data-ttu-id="e1b9a-114">Описание</span><span class="sxs-lookup"><span data-stu-id="e1b9a-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e1b9a-115">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="e1b9a-115">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="e1b9a-116">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="e1b9a-116">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="e1b9a-117">Чтение свойств и связей объекта subscribedSku.</span><span class="sxs-lookup"><span data-stu-id="e1b9a-117">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="e1b9a-118">Список subscribedsku</span><span class="sxs-lookup"><span data-stu-id="e1b9a-118">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="e1b9a-119">Коллекция объектов [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="e1b9a-119">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="e1b9a-120">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="e1b9a-120">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="e1b9a-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1b9a-121">Properties</span></span>
| <span data-ttu-id="e1b9a-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1b9a-122">Property</span></span>     | <span data-ttu-id="e1b9a-123">Тип</span><span class="sxs-lookup"><span data-stu-id="e1b9a-123">Type</span></span>   |<span data-ttu-id="e1b9a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e1b9a-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1b9a-125">appliesTo</span><span class="sxs-lookup"><span data-stu-id="e1b9a-125">appliesTo</span></span>|<span data-ttu-id="e1b9a-126">String</span><span class="sxs-lookup"><span data-stu-id="e1b9a-126">String</span></span>| <span data-ttu-id="e1b9a-127">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="e1b9a-127">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="e1b9a-128">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="e1b9a-128">capabilityStatus</span></span>|<span data-ttu-id="e1b9a-129">Строка</span><span class="sxs-lookup"><span data-stu-id="e1b9a-129">String</span></span>| <span data-ttu-id="e1b9a-130">Например, Enabled.</span><span class="sxs-lookup"><span data-stu-id="e1b9a-130">For example, "Enabled".</span></span> |
|<span data-ttu-id="e1b9a-131">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="e1b9a-131">consumedUnits</span></span>|<span data-ttu-id="e1b9a-132">Int32</span><span class="sxs-lookup"><span data-stu-id="e1b9a-132">Int32</span></span>| <span data-ttu-id="e1b9a-133">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="e1b9a-133">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="e1b9a-134">id</span><span class="sxs-lookup"><span data-stu-id="e1b9a-134">id</span></span>|<span data-ttu-id="e1b9a-135">String</span><span class="sxs-lookup"><span data-stu-id="e1b9a-135">String</span></span>| <span data-ttu-id="e1b9a-p104">Уникальный идентификатор объекта sku, подписка на который выполнена. Ключ, значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="e1b9a-p104">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="e1b9a-138">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="e1b9a-138">prepaidUnits</span></span>|[<span data-ttu-id="e1b9a-139">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="e1b9a-139">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="e1b9a-140">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="e1b9a-140">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="e1b9a-141">servicePlans</span><span class="sxs-lookup"><span data-stu-id="e1b9a-141">servicePlans</span></span>|<span data-ttu-id="e1b9a-142">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="e1b9a-142">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="e1b9a-p105">Сведения о планах обслуживания, доступных в отношении SKU. Значение NULL не допускается</span><span class="sxs-lookup"><span data-stu-id="e1b9a-p105">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="e1b9a-145">skuId</span><span class="sxs-lookup"><span data-stu-id="e1b9a-145">skuId</span></span>|<span data-ttu-id="e1b9a-146">Guid</span><span class="sxs-lookup"><span data-stu-id="e1b9a-146">Guid</span></span>| <span data-ttu-id="e1b9a-147">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="e1b9a-147">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="e1b9a-148">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="e1b9a-148">skuPartNumber</span></span>|<span data-ttu-id="e1b9a-149">String</span><span class="sxs-lookup"><span data-stu-id="e1b9a-149">String</span></span>| <span data-ttu-id="e1b9a-150">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="e1b9a-150">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="e1b9a-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="e1b9a-151">Relationships</span></span>
<span data-ttu-id="e1b9a-152">Нет</span><span class="sxs-lookup"><span data-stu-id="e1b9a-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1b9a-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1b9a-153">JSON representation</span></span>

<span data-ttu-id="e1b9a-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1b9a-154">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "subscribedSku resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
