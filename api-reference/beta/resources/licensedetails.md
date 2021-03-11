---
title: тип ресурса licenseDetails
description: Содержит сведения о лицензии, назначенной пользователю.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: jpettere
ms.openlocfilehash: 7a00c1aa5de5684c71a1d83f00b303ada6f54056
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720524"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="81cdc-103">тип ресурса licenseDetails</span><span class="sxs-lookup"><span data-stu-id="81cdc-103">licenseDetails resource type</span></span>

<span data-ttu-id="81cdc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81cdc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81cdc-105">Содержит сведения о лицензии, назначенной пользователю.</span><span class="sxs-lookup"><span data-stu-id="81cdc-105">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="81cdc-106">Методы</span><span class="sxs-lookup"><span data-stu-id="81cdc-106">Methods</span></span>

| <span data-ttu-id="81cdc-107">Метод</span><span class="sxs-lookup"><span data-stu-id="81cdc-107">Method</span></span>           | <span data-ttu-id="81cdc-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="81cdc-108">Return Type</span></span>    |<span data-ttu-id="81cdc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="81cdc-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="81cdc-110">Перечисление licenseDetails</span><span class="sxs-lookup"><span data-stu-id="81cdc-110">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="81cdc-111">Коллекция объектов licenseDetails</span><span class="sxs-lookup"><span data-stu-id="81cdc-111">licenseDetails collection</span></span> |<span data-ttu-id="81cdc-112">Извлечение списка объектов licenseDetails для пользователя.</span><span class="sxs-lookup"><span data-stu-id="81cdc-112">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="81cdc-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="81cdc-113">Properties</span></span>
| <span data-ttu-id="81cdc-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="81cdc-114">Property</span></span>     | <span data-ttu-id="81cdc-115">Тип</span><span class="sxs-lookup"><span data-stu-id="81cdc-115">Type</span></span>   |<span data-ttu-id="81cdc-116">Описание</span><span class="sxs-lookup"><span data-stu-id="81cdc-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="81cdc-117">id</span><span class="sxs-lookup"><span data-stu-id="81cdc-117">id</span></span>|<span data-ttu-id="81cdc-118">String</span><span class="sxs-lookup"><span data-stu-id="81cdc-118">String</span></span>| <span data-ttu-id="81cdc-119">Уникальный идентификатор объекта детализации лицензии.</span><span class="sxs-lookup"><span data-stu-id="81cdc-119">The unique identifier for the license detail object.</span></span> <span data-ttu-id="81cdc-120">Только для чтения, клавиши, а не nullable</span><span class="sxs-lookup"><span data-stu-id="81cdc-120">Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="81cdc-121">servicePlans</span><span class="sxs-lookup"><span data-stu-id="81cdc-121">servicePlans</span></span>|<span data-ttu-id="81cdc-122">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="81cdc-122">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="81cdc-123">Сведения о планах служб, присвоенных лицензией.</span><span class="sxs-lookup"><span data-stu-id="81cdc-123">Information about the service plans assigned with the license.</span></span> <span data-ttu-id="81cdc-124">Только для чтения, не является недействительным</span><span class="sxs-lookup"><span data-stu-id="81cdc-124">Read-only, Not nullable</span></span> |
|<span data-ttu-id="81cdc-125">skuId</span><span class="sxs-lookup"><span data-stu-id="81cdc-125">skuId</span></span>|<span data-ttu-id="81cdc-126">Guid</span><span class="sxs-lookup"><span data-stu-id="81cdc-126">Guid</span></span>| <span data-ttu-id="81cdc-127">Уникальный идентификатор (GUID) для службы SKU.</span><span class="sxs-lookup"><span data-stu-id="81cdc-127">Unique identifier (GUID) for the service SKU.</span></span> <span data-ttu-id="81cdc-128">Равно свойству skuId на связанном [объекте SubscribedSku.](subscribedsku.md)</span><span class="sxs-lookup"><span data-stu-id="81cdc-128">Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object.</span></span> <span data-ttu-id="81cdc-129">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="81cdc-129">Read-only</span></span> |
|<span data-ttu-id="81cdc-130">skuPartNumber</span><span class="sxs-lookup"><span data-stu-id="81cdc-130">skuPartNumber</span></span>|<span data-ttu-id="81cdc-131">String</span><span class="sxs-lookup"><span data-stu-id="81cdc-131">String</span></span>| <span data-ttu-id="81cdc-132">Уникальное имя отображения SKU.</span><span class="sxs-lookup"><span data-stu-id="81cdc-132">Unique SKU display name.</span></span> <span data-ttu-id="81cdc-133">Равно skuPartNumber на связанном [объекте SubscribedSku;](subscribedsku.md) например: "AAD_Premium".</span><span class="sxs-lookup"><span data-stu-id="81cdc-133">Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium".</span></span> <span data-ttu-id="81cdc-134">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="81cdc-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="81cdc-135">Связи</span><span class="sxs-lookup"><span data-stu-id="81cdc-135">Relationships</span></span>
<span data-ttu-id="81cdc-136">Нет</span><span class="sxs-lookup"><span data-stu-id="81cdc-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81cdc-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="81cdc-137">JSON representation</span></span>
<span data-ttu-id="81cdc-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="81cdc-138">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "licenseDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


