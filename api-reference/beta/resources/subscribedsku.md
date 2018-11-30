---
title: Тип ресурса subscribedSku
description: " Создание, обновление и удаление не поддерживается. Выражения фильтра запроса не поддерживается. Наследуется от directoryObject."
ms.openlocfilehash: ab9b64d8de67379aa002ffeec78edd327b15b222
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081435"
---
# <a name="subscribedsku-resource-type"></a><span data-ttu-id="7b548-105">Тип ресурса subscribedSku</span><span class="sxs-lookup"><span data-stu-id="7b548-105">subscribedSku resource type</span></span>

> <span data-ttu-id="7b548-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="7b548-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7b548-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7b548-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7b548-p103">В подписанных SKU поддерживается только операция чтения. Создание, обновление и удаление не поддерживаются. Выражения фильтра запроса не поддерживаются. Наследуется от [directoryObject](directoryobject.md).</span><span class="sxs-lookup"><span data-stu-id="7b548-p103">Only the read operation is supported on subscribed SKUs; create, update, and delete are not supported. Query filter expressions are not supported. Inherits from [directoryObject](directoryobject.md).</span></span>


## <a name="methods"></a><span data-ttu-id="7b548-111">Методы</span><span class="sxs-lookup"><span data-stu-id="7b548-111">Methods</span></span>
| <span data-ttu-id="7b548-112">Метод</span><span class="sxs-lookup"><span data-stu-id="7b548-112">Method</span></span>           | <span data-ttu-id="7b548-113">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7b548-113">Return Type</span></span>    |<span data-ttu-id="7b548-114">Описание</span><span class="sxs-lookup"><span data-stu-id="7b548-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7b548-115">Получение объекта subscribedSku</span><span class="sxs-lookup"><span data-stu-id="7b548-115">Get subscribedSku</span></span>](../api/subscribedsku-get.md) | [<span data-ttu-id="7b548-116">subscribedSku</span><span class="sxs-lookup"><span data-stu-id="7b548-116">subscribedSku</span></span>](subscribedsku.md) |<span data-ttu-id="7b548-117">Чтение свойств и связей объекта subscribedSku.</span><span class="sxs-lookup"><span data-stu-id="7b548-117">Read properties and relationships of subscribedSku object.</span></span>|
|[<span data-ttu-id="7b548-118">Список subscribedsku</span><span class="sxs-lookup"><span data-stu-id="7b548-118">List subscribedsku</span></span>](../api/subscribedsku-list.md) | <span data-ttu-id="7b548-119">Коллекция объектов [subscribedSku](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="7b548-119">[subscribedSku](subscribedsku.md) collection</span></span> |<span data-ttu-id="7b548-120">Получение списка коммерческих подписок, приобретенных организацией.</span><span class="sxs-lookup"><span data-stu-id="7b548-120">Retrieve the list of commercial subscriptions that an organization has acquired.</span></span>|

## <a name="properties"></a><span data-ttu-id="7b548-121">Свойства</span><span class="sxs-lookup"><span data-stu-id="7b548-121">Properties</span></span>
| <span data-ttu-id="7b548-122">Свойство</span><span class="sxs-lookup"><span data-stu-id="7b548-122">Property</span></span>     | <span data-ttu-id="7b548-123">Тип</span><span class="sxs-lookup"><span data-stu-id="7b548-123">Type</span></span>   |<span data-ttu-id="7b548-124">Описание</span><span class="sxs-lookup"><span data-stu-id="7b548-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b548-125">appliesTo</span><span class="sxs-lookup"><span data-stu-id="7b548-125">appliesTo</span></span>|<span data-ttu-id="7b548-126">String</span><span class="sxs-lookup"><span data-stu-id="7b548-126">String</span></span>| <span data-ttu-id="7b548-127">Например, User или Company.</span><span class="sxs-lookup"><span data-stu-id="7b548-127">For example, "User" or "Company".</span></span> |
|<span data-ttu-id="7b548-128">capabilityStatus</span><span class="sxs-lookup"><span data-stu-id="7b548-128">capabilityStatus</span></span>|<span data-ttu-id="7b548-129">Строка</span><span class="sxs-lookup"><span data-stu-id="7b548-129">String</span></span>| <span data-ttu-id="7b548-130">Например, Enabled.</span><span class="sxs-lookup"><span data-stu-id="7b548-130">For example, "Enabled".</span></span> |
|<span data-ttu-id="7b548-131">consumedUnits</span><span class="sxs-lookup"><span data-stu-id="7b548-131">consumedUnits</span></span>|<span data-ttu-id="7b548-132">Int32</span><span class="sxs-lookup"><span data-stu-id="7b548-132">Int32</span></span>| <span data-ttu-id="7b548-133">Количество лицензий, которые были назначены.</span><span class="sxs-lookup"><span data-stu-id="7b548-133">The number of licenses that have been assigned.</span></span> |
|<span data-ttu-id="7b548-134">id</span><span class="sxs-lookup"><span data-stu-id="7b548-134">id</span></span>|<span data-ttu-id="7b548-135">String</span><span class="sxs-lookup"><span data-stu-id="7b548-135">String</span></span>| <span data-ttu-id="7b548-p104">Уникальный идентификатор объекта sku, подписка на который выполнена. Ключ, значение NULL не допускается.</span><span class="sxs-lookup"><span data-stu-id="7b548-p104">The unique identifier for the subscribed sku object. Key, not nullable.</span></span> |
|<span data-ttu-id="7b548-138">prepaidUnits</span><span class="sxs-lookup"><span data-stu-id="7b548-138">prepaidUnits</span></span>|[<span data-ttu-id="7b548-139">licenseUnitsDetail</span><span class="sxs-lookup"><span data-stu-id="7b548-139">licenseUnitsDetail</span></span>](licenseunitsdetail.md)| <span data-ttu-id="7b548-140">Сведения о количестве и состоянии предварительно оплаченных лицензий.</span><span class="sxs-lookup"><span data-stu-id="7b548-140">Information about the number and status of prepaid licenses.</span></span> |
|<span data-ttu-id="7b548-141">servicePlans</span><span class="sxs-lookup"><span data-stu-id="7b548-141">servicePlans</span></span>|<span data-ttu-id="7b548-142">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="7b548-142">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="7b548-p105">Сведения о планах обслуживания, доступных в отношении SKU. Значение NULL не допускается</span><span class="sxs-lookup"><span data-stu-id="7b548-p105">Information about the service plans that are available with the SKU. Not nullable</span></span> |
|<span data-ttu-id="7b548-145">skuId</span><span class="sxs-lookup"><span data-stu-id="7b548-145">skuId</span></span>|<span data-ttu-id="7b548-146">Guid</span><span class="sxs-lookup"><span data-stu-id="7b548-146">Guid</span></span>| <span data-ttu-id="7b548-147">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="7b548-147">The unique identifier (GUID) for the service SKU.</span></span> |
|<span data-ttu-id="7b548-148">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="7b548-148">skuPartNumber</span></span>|<span data-ttu-id="7b548-149">String</span><span class="sxs-lookup"><span data-stu-id="7b548-149">String</span></span>| <span data-ttu-id="7b548-150">Артикул SKU, например: AAD_PREMIUM или RMSBASIC.</span><span class="sxs-lookup"><span data-stu-id="7b548-150">The SKU part number; for example: "AAD_PREMIUM" or "RMSBASIC".</span></span> |

## <a name="relationships"></a><span data-ttu-id="7b548-151">Отношения</span><span class="sxs-lookup"><span data-stu-id="7b548-151">Relationships</span></span>
<span data-ttu-id="7b548-152">Нет</span><span class="sxs-lookup"><span data-stu-id="7b548-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7b548-153">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7b548-153">JSON representation</span></span>

<span data-ttu-id="7b548-154">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7b548-154">Here is a JSON representation of the resource</span></span>

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
