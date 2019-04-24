---
title: Тип ресурса licenseDetails
description: Содержит сведения о лицензии, назначенной пользователю.
localization_priority: Normal
ms.openlocfilehash: 4495e85b45f6fcfda4f37e467e9cdc5393787dc1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585190"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="c8748-103">Тип ресурса licenseDetails</span><span class="sxs-lookup"><span data-stu-id="c8748-103">licenseDetails resource type</span></span>

<span data-ttu-id="c8748-104">Содержит сведения о лицензии, назначенной пользователю.</span><span class="sxs-lookup"><span data-stu-id="c8748-104">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="c8748-105">Методы</span><span class="sxs-lookup"><span data-stu-id="c8748-105">Methods</span></span>

| <span data-ttu-id="c8748-106">Метод</span><span class="sxs-lookup"><span data-stu-id="c8748-106">Method</span></span>           | <span data-ttu-id="c8748-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="c8748-107">Return Type</span></span>    |<span data-ttu-id="c8748-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c8748-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c8748-109">Перечисление licenseDetails</span><span class="sxs-lookup"><span data-stu-id="c8748-109">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="c8748-110">Коллекция объектов licenseDetails</span><span class="sxs-lookup"><span data-stu-id="c8748-110">licenseDetails collection</span></span> |<span data-ttu-id="c8748-111">Получение списка объектов licenseDetails для пользователя.</span><span class="sxs-lookup"><span data-stu-id="c8748-111">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="c8748-112">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8748-112">Properties</span></span>
| <span data-ttu-id="c8748-113">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8748-113">Property</span></span>     | <span data-ttu-id="c8748-114">Тип</span><span class="sxs-lookup"><span data-stu-id="c8748-114">Type</span></span>   |<span data-ttu-id="c8748-115">Описание</span><span class="sxs-lookup"><span data-stu-id="c8748-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c8748-116">id</span><span class="sxs-lookup"><span data-stu-id="c8748-116">id</span></span>|<span data-ttu-id="c8748-117">String</span><span class="sxs-lookup"><span data-stu-id="c8748-117">String</span></span>| <span data-ttu-id="c8748-118">Уникальный идентификатор для объекта сведений о лицензии.</span><span class="sxs-lookup"><span data-stu-id="c8748-118">The unique identifier for the license detail object.</span></span> <span data-ttu-id="c8748-119">Только для чтения, ключ, не допускающий значение null</span><span class="sxs-lookup"><span data-stu-id="c8748-119">Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="c8748-120">Сервицепланс</span><span class="sxs-lookup"><span data-stu-id="c8748-120">servicePlans</span></span>|<span data-ttu-id="c8748-121">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="c8748-121">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="c8748-122">Сведения о планах обслуживания, назначенных с лицензией.</span><span class="sxs-lookup"><span data-stu-id="c8748-122">Information about the service plans assigned with the license.</span></span> <span data-ttu-id="c8748-123">Только для чтения, не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="c8748-123">Read-only, Not nullable</span></span> |
|<span data-ttu-id="c8748-124">skuId</span><span class="sxs-lookup"><span data-stu-id="c8748-124">skuId</span></span>|<span data-ttu-id="c8748-125">Guid</span><span class="sxs-lookup"><span data-stu-id="c8748-125">Guid</span></span>| <span data-ttu-id="c8748-126">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="c8748-126">Unique identifier (GUID) for the service SKU.</span></span> <span data-ttu-id="c8748-127">Равно свойству skuId в связанном объекте [SubscribedSku](subscribedsku.md) .</span><span class="sxs-lookup"><span data-stu-id="c8748-127">Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object.</span></span> <span data-ttu-id="c8748-128">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="c8748-128">Read-only</span></span> |
|<span data-ttu-id="c8748-129">Скупартнумбер</span><span class="sxs-lookup"><span data-stu-id="c8748-129">skuPartNumber</span></span>|<span data-ttu-id="c8748-130">String</span><span class="sxs-lookup"><span data-stu-id="c8748-130">String</span></span>| <span data-ttu-id="c8748-131">Имя уникального отображаемого номера SKU.</span><span class="sxs-lookup"><span data-stu-id="c8748-131">Unique SKU display name.</span></span> <span data-ttu-id="c8748-132">Равно Скупартнумбер для связанного объекта [SubscribedSku](subscribedsku.md) ; Пример: "Аад_премиум".</span><span class="sxs-lookup"><span data-stu-id="c8748-132">Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium".</span></span> <span data-ttu-id="c8748-133">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="c8748-133">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="c8748-134">Отношения</span><span class="sxs-lookup"><span data-stu-id="c8748-134">Relationships</span></span>
<span data-ttu-id="c8748-135">Нет</span><span class="sxs-lookup"><span data-stu-id="c8748-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8748-136">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c8748-136">JSON representation</span></span>
<span data-ttu-id="c8748-137">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8748-137">Here is a JSON representation of the resource.</span></span>

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
