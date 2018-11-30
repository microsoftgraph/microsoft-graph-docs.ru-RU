---
title: Тип ресурса licenseDetails
description: Содержит сведения о лицензии, назначенной пользователю.
ms.openlocfilehash: 8c357617eea04151851a0e3a27c41937abd07b28
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025965"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="3c8c0-103">Тип ресурса licenseDetails</span><span class="sxs-lookup"><span data-stu-id="3c8c0-103">licenseDetails resource type</span></span>

<span data-ttu-id="3c8c0-104">Содержит сведения о лицензии, назначенной пользователю.</span><span class="sxs-lookup"><span data-stu-id="3c8c0-104">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="3c8c0-105">Методы</span><span class="sxs-lookup"><span data-stu-id="3c8c0-105">Methods</span></span>

| <span data-ttu-id="3c8c0-106">Метод</span><span class="sxs-lookup"><span data-stu-id="3c8c0-106">Method</span></span>           | <span data-ttu-id="3c8c0-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3c8c0-107">Return Type</span></span>    |<span data-ttu-id="3c8c0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="3c8c0-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3c8c0-109">Перечисление licenseDetails</span><span class="sxs-lookup"><span data-stu-id="3c8c0-109">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="3c8c0-110">Коллекция licenseDetails</span><span class="sxs-lookup"><span data-stu-id="3c8c0-110">licenseDetails collection</span></span> |<span data-ttu-id="3c8c0-111">Получение списка объектов licenseDetails для пользователя.</span><span class="sxs-lookup"><span data-stu-id="3c8c0-111">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="3c8c0-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c8c0-112">Properties</span></span>
| <span data-ttu-id="3c8c0-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c8c0-113">Property</span></span>     | <span data-ttu-id="3c8c0-114">Тип</span><span class="sxs-lookup"><span data-stu-id="3c8c0-114">Type</span></span>   |<span data-ttu-id="3c8c0-115">Описание</span><span class="sxs-lookup"><span data-stu-id="3c8c0-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c8c0-116">id</span><span class="sxs-lookup"><span data-stu-id="3c8c0-116">id</span></span>|<span data-ttu-id="3c8c0-117">String</span><span class="sxs-lookup"><span data-stu-id="3c8c0-117">String</span></span>| <span data-ttu-id="3c8c0-p101">Уникальный идентификатор объекта сведений о лицензии. Только для чтения, ключевое, не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="3c8c0-p101">The unique identifier for the license detail object. Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="3c8c0-120">servicePlans</span><span class="sxs-lookup"><span data-stu-id="3c8c0-120">servicePlans</span></span>|<span data-ttu-id="3c8c0-121">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="3c8c0-121">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="3c8c0-p102">Сведения о планах обслуживания, назначенных вместе с лицензией. Только для чтения, не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="3c8c0-p102">Information about the service plans assigned with the license. Read-only, Not nullable</span></span> |
|<span data-ttu-id="3c8c0-124">skuId</span><span class="sxs-lookup"><span data-stu-id="3c8c0-124">skuId</span></span>|<span data-ttu-id="3c8c0-125">Guid</span><span class="sxs-lookup"><span data-stu-id="3c8c0-125">Guid</span></span>| <span data-ttu-id="3c8c0-p103">Уникальный идентификатор (GUID) для SKU службы. Имеет то же значение, что и свойство skuId в связанном объекте [SubscribedSku](subscribedsku.md). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c8c0-p103">Unique identifier (GUID) for the service SKU. Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object. Read-only</span></span> |
|<span data-ttu-id="3c8c0-129">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="3c8c0-129">skuPartNumber</span></span>|<span data-ttu-id="3c8c0-130">String</span><span class="sxs-lookup"><span data-stu-id="3c8c0-130">String</span></span>| <span data-ttu-id="3c8c0-p104">Уникальное отображаемое имя SKU. Имеет то же значение, что и свойство skuPartNumber в связанном объекте [SubscribedSku](subscribedsku.md). Пример: AAD_Premium. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3c8c0-p104">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="3c8c0-134">Связи</span><span class="sxs-lookup"><span data-stu-id="3c8c0-134">Relationships</span></span>
<span data-ttu-id="3c8c0-135">Нет</span><span class="sxs-lookup"><span data-stu-id="3c8c0-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c8c0-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c8c0-136">JSON representation</span></span>
<span data-ttu-id="3c8c0-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c8c0-137">Here is a JSON representation of the resource.</span></span>

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