---
title: licenseDetails тип ресурса
description: Содержит информацию о лицензии, назначенной пользователю.
localization_priority: Normal
author: jpettere
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 4e23dfcd15dc2b05a9d1c7356a532e6faf487662
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547192"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="efdf6-103">licenseDetails тип ресурса</span><span class="sxs-lookup"><span data-stu-id="efdf6-103">licenseDetails resource type</span></span>

<span data-ttu-id="efdf6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efdf6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="efdf6-105">Содержит информацию о лицензии, назначенной пользователю.</span><span class="sxs-lookup"><span data-stu-id="efdf6-105">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="efdf6-106">Методы</span><span class="sxs-lookup"><span data-stu-id="efdf6-106">Methods</span></span>

| <span data-ttu-id="efdf6-107">Метод</span><span class="sxs-lookup"><span data-stu-id="efdf6-107">Method</span></span>           | <span data-ttu-id="efdf6-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="efdf6-108">Return Type</span></span>    |<span data-ttu-id="efdf6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="efdf6-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="efdf6-110">Перечисление licenseDetails</span><span class="sxs-lookup"><span data-stu-id="efdf6-110">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="efdf6-111">Коллекция объектов licenseDetails</span><span class="sxs-lookup"><span data-stu-id="efdf6-111">licenseDetails collection</span></span> |<span data-ttu-id="efdf6-112">Получить список объектов licenseDetails для пользователя.</span><span class="sxs-lookup"><span data-stu-id="efdf6-112">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="efdf6-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="efdf6-113">Properties</span></span>
| <span data-ttu-id="efdf6-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="efdf6-114">Property</span></span>     | <span data-ttu-id="efdf6-115">Тип</span><span class="sxs-lookup"><span data-stu-id="efdf6-115">Type</span></span>   |<span data-ttu-id="efdf6-116">Описание</span><span class="sxs-lookup"><span data-stu-id="efdf6-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efdf6-117">id</span><span class="sxs-lookup"><span data-stu-id="efdf6-117">id</span></span>|<span data-ttu-id="efdf6-118">String</span><span class="sxs-lookup"><span data-stu-id="efdf6-118">String</span></span>| <span data-ttu-id="efdf6-119">Уникальный идентификатор объекта детализации лицензии.</span><span class="sxs-lookup"><span data-stu-id="efdf6-119">The unique identifier for the license detail object.</span></span> <span data-ttu-id="efdf6-120">Читать только, ключ, не сведены на нет</span><span class="sxs-lookup"><span data-stu-id="efdf6-120">Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="efdf6-121">servicePlans</span><span class="sxs-lookup"><span data-stu-id="efdf6-121">servicePlans</span></span>|<span data-ttu-id="efdf6-122">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="efdf6-122">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="efdf6-123">Информация о планах обслуживания, назначенных лицензией.</span><span class="sxs-lookup"><span data-stu-id="efdf6-123">Information about the service plans assigned with the license.</span></span> <span data-ttu-id="efdf6-124">Читать только, не обнуляемый</span><span class="sxs-lookup"><span data-stu-id="efdf6-124">Read-only, Not nullable</span></span> |
|<span data-ttu-id="efdf6-125">skuId</span><span class="sxs-lookup"><span data-stu-id="efdf6-125">skuId</span></span>|<span data-ttu-id="efdf6-126">Guid</span><span class="sxs-lookup"><span data-stu-id="efdf6-126">Guid</span></span>| <span data-ttu-id="efdf6-127">Уникальный идентификатор (GUID) для службы SKU.</span><span class="sxs-lookup"><span data-stu-id="efdf6-127">Unique identifier (GUID) for the service SKU.</span></span> <span data-ttu-id="efdf6-128">Равно свойству skuId на связанном [объекте SubscribedSku.](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="efdf6-128">Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object.</span></span> <span data-ttu-id="efdf6-129">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="efdf6-129">Read-only</span></span> |
|<span data-ttu-id="efdf6-130">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="efdf6-130">skuPartNumber</span></span>|<span data-ttu-id="efdf6-131">String</span><span class="sxs-lookup"><span data-stu-id="efdf6-131">String</span></span>| <span data-ttu-id="efdf6-132">Уникальное имя дисплея SKU.</span><span class="sxs-lookup"><span data-stu-id="efdf6-132">Unique SKU display name.</span></span> <span data-ttu-id="efdf6-133">Равный skuPartNumber на связанном [объекте SubscribedSku;](subscribedsku.md) например: "AAD_Premium".</span><span class="sxs-lookup"><span data-stu-id="efdf6-133">Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium".</span></span> <span data-ttu-id="efdf6-134">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="efdf6-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="efdf6-135">Связи</span><span class="sxs-lookup"><span data-stu-id="efdf6-135">Relationships</span></span>
<span data-ttu-id="efdf6-136">Нет</span><span class="sxs-lookup"><span data-stu-id="efdf6-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="efdf6-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="efdf6-137">JSON representation</span></span>
<span data-ttu-id="efdf6-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efdf6-138">Here is a JSON representation of the resource.</span></span>

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

