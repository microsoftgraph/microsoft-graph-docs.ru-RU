---
title: Тип ресурса licenseDetails
description: Содержит сведения о лицензии, назначенной пользователю.
ms.openlocfilehash: dd56026d2c1d230fe6bb25b78ff8ababa01f577b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082395"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="202d0-103">Тип ресурса licenseDetails</span><span class="sxs-lookup"><span data-stu-id="202d0-103">licenseDetails resource type</span></span>

> <span data-ttu-id="202d0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="202d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="202d0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="202d0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="202d0-106">Содержит сведения о лицензии, назначенной пользователю.</span><span class="sxs-lookup"><span data-stu-id="202d0-106">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="202d0-107">Методы</span><span class="sxs-lookup"><span data-stu-id="202d0-107">Methods</span></span>

| <span data-ttu-id="202d0-108">Метод</span><span class="sxs-lookup"><span data-stu-id="202d0-108">Method</span></span>           | <span data-ttu-id="202d0-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="202d0-109">Return Type</span></span>    |<span data-ttu-id="202d0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="202d0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="202d0-111">Перечисление licenseDetails</span><span class="sxs-lookup"><span data-stu-id="202d0-111">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="202d0-112">Коллекция licenseDetails</span><span class="sxs-lookup"><span data-stu-id="202d0-112">licenseDetails collection</span></span> |<span data-ttu-id="202d0-113">Получение списка объектов licenseDetails для пользователя.</span><span class="sxs-lookup"><span data-stu-id="202d0-113">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="202d0-114">Свойства</span><span class="sxs-lookup"><span data-stu-id="202d0-114">Properties</span></span>
| <span data-ttu-id="202d0-115">Свойство</span><span class="sxs-lookup"><span data-stu-id="202d0-115">Property</span></span>     | <span data-ttu-id="202d0-116">Тип</span><span class="sxs-lookup"><span data-stu-id="202d0-116">Type</span></span>   |<span data-ttu-id="202d0-117">Описание</span><span class="sxs-lookup"><span data-stu-id="202d0-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="202d0-118">id</span><span class="sxs-lookup"><span data-stu-id="202d0-118">id</span></span>|<span data-ttu-id="202d0-119">String</span><span class="sxs-lookup"><span data-stu-id="202d0-119">String</span></span>| <span data-ttu-id="202d0-p102">Уникальный идентификатор объекта сведений о лицензии. Только для чтения, ключевое, не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="202d0-p102">The unique identifier for the license detail object. Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="202d0-122">servicePlans</span><span class="sxs-lookup"><span data-stu-id="202d0-122">servicePlans</span></span>|<span data-ttu-id="202d0-123">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="202d0-123">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="202d0-p103">Сведения о планах обслуживания, назначенных вместе с лицензией. Только для чтения, не допускает значения null.</span><span class="sxs-lookup"><span data-stu-id="202d0-p103">Information about the service plans assigned with the license. Read-only, Not nullable</span></span> |
|<span data-ttu-id="202d0-126">skuId</span><span class="sxs-lookup"><span data-stu-id="202d0-126">skuId</span></span>|<span data-ttu-id="202d0-127">Guid</span><span class="sxs-lookup"><span data-stu-id="202d0-127">Guid</span></span>| <span data-ttu-id="202d0-p104">Уникальный идентификатор (GUID) для SKU службы. Имеет то же значение, что и свойство skuId в связанном объекте [SubscribedSku](subscribedsku.md). Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="202d0-p104">Unique identifier (GUID) for the service SKU. Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object. Read-only</span></span> |
|<span data-ttu-id="202d0-131">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="202d0-131">skuPartNumber</span></span>|<span data-ttu-id="202d0-132">String</span><span class="sxs-lookup"><span data-stu-id="202d0-132">String</span></span>| <span data-ttu-id="202d0-p105">Уникальное отображаемое имя SKU. Имеет то же значение, что и свойство skuPartNumber в связанном объекте [SubscribedSku](subscribedsku.md). Пример: AAD_Premium. Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="202d0-p105">Unique SKU display name. Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium". Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="202d0-136">Связи</span><span class="sxs-lookup"><span data-stu-id="202d0-136">Relationships</span></span>
<span data-ttu-id="202d0-137">Нет</span><span class="sxs-lookup"><span data-stu-id="202d0-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="202d0-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="202d0-138">JSON representation</span></span>
<span data-ttu-id="202d0-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="202d0-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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