---
title: Тип ресурса licenseDetails
description: Содержит сведения о лицензии, назначенной пользователю.
localization_priority: Normal
ms.openlocfilehash: 4495e85b45f6fcfda4f37e467e9cdc5393787dc1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843024"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="8a6a2-103">Тип ресурса licenseDetails</span><span class="sxs-lookup"><span data-stu-id="8a6a2-103">licenseDetails resource type</span></span>

<span data-ttu-id="8a6a2-104">Содержит сведения о лицензии, назначенной пользователю.</span><span class="sxs-lookup"><span data-stu-id="8a6a2-104">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="8a6a2-105">Методы</span><span class="sxs-lookup"><span data-stu-id="8a6a2-105">Methods</span></span>

| <span data-ttu-id="8a6a2-106">Метод</span><span class="sxs-lookup"><span data-stu-id="8a6a2-106">Method</span></span>           | <span data-ttu-id="8a6a2-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8a6a2-107">Return Type</span></span>    |<span data-ttu-id="8a6a2-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8a6a2-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8a6a2-109">Перечисление licenseDetails</span><span class="sxs-lookup"><span data-stu-id="8a6a2-109">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="8a6a2-110">Коллекция licenseDetails</span><span class="sxs-lookup"><span data-stu-id="8a6a2-110">licenseDetails collection</span></span> |<span data-ttu-id="8a6a2-111">Получение списка объектов licenseDetails для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8a6a2-111">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="8a6a2-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="8a6a2-112">Properties</span></span>
| <span data-ttu-id="8a6a2-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="8a6a2-113">Property</span></span>     | <span data-ttu-id="8a6a2-114">Тип</span><span class="sxs-lookup"><span data-stu-id="8a6a2-114">Type</span></span>   |<span data-ttu-id="8a6a2-115">Описание</span><span class="sxs-lookup"><span data-stu-id="8a6a2-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a6a2-116">id</span><span class="sxs-lookup"><span data-stu-id="8a6a2-116">id</span></span>|<span data-ttu-id="8a6a2-117">String</span><span class="sxs-lookup"><span data-stu-id="8a6a2-117">String</span></span>| <span data-ttu-id="8a6a2-p101">Уникальный идентификатор объекта сведений о лицензии. Только для чтения, ключевое, не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="8a6a2-p101">The unique identifier for the license detail object. Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="8a6a2-120">servicePlans</span><span class="sxs-lookup"><span data-stu-id="8a6a2-120">servicePlans</span></span>|<span data-ttu-id="8a6a2-121">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="8a6a2-121">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="8a6a2-p102">Сведения о планах обслуживания, назначенных вместе с лицензией. Только для чтения, не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="8a6a2-p102">Information about the service plans assigned with the license. Read-only, Not nullable</span></span> |
|<span data-ttu-id="8a6a2-124">skuId</span><span class="sxs-lookup"><span data-stu-id="8a6a2-124">skuId</span></span>|<span data-ttu-id="8a6a2-125">Guid</span><span class="sxs-lookup"><span data-stu-id="8a6a2-125">Guid</span></span>| <span data-ttu-id="8a6a2-p103">Уникальный идентификатор (GUID) для SKU службы. Имеет то же значение, что и свойство skuId в связанном объекте [SubscribedSku](subscribedsku.md). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a6a2-p103">Unique identifier (GUID) for the service SKU. Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object. Read-only</span></span> |
|<span data-ttu-id="8a6a2-129">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="8a6a2-129">skuPartNumber</span></span>|<span data-ttu-id="8a6a2-130">String</span><span class="sxs-lookup"><span data-stu-id="8a6a2-130">String</span></span>| <span data-ttu-id="8a6a2-p104">Уникальное отображаемое имя SKU. Имеет то же значение, что и свойство skuPartNumber в связанном объекте [SubscribedSku](subscribedsku.md). Пример: AAD_Premium. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8a6a2-p104">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="8a6a2-134">Связи</span><span class="sxs-lookup"><span data-stu-id="8a6a2-134">Relationships</span></span>
<span data-ttu-id="8a6a2-135">Нет</span><span class="sxs-lookup"><span data-stu-id="8a6a2-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a6a2-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8a6a2-136">JSON representation</span></span>
<span data-ttu-id="8a6a2-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8a6a2-137">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.licenseDetails"
}-->

```json
{
  "id": "String (identifier)",
  "servicePlans": [{"@odata.type": "microsoft.graph.servicePlanInfo"}],
  "skuId": "Guid",
  "skuPartNumber": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
