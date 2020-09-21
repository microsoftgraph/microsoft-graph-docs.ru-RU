---
title: Тип ресурса licenseDetails
description: Содержит сведения о лицензии, назначенной пользователю.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: krbain
ms.openlocfilehash: 5236a73697ea6969698fa0cdb6a8368188d0271c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029199"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="f5ab0-103">Тип ресурса licenseDetails</span><span class="sxs-lookup"><span data-stu-id="f5ab0-103">licenseDetails resource type</span></span>

<span data-ttu-id="f5ab0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5ab0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5ab0-105">Содержит сведения о лицензии, назначенной пользователю.</span><span class="sxs-lookup"><span data-stu-id="f5ab0-105">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="f5ab0-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f5ab0-106">Methods</span></span>

| <span data-ttu-id="f5ab0-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f5ab0-107">Method</span></span>           | <span data-ttu-id="f5ab0-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f5ab0-108">Return Type</span></span>    |<span data-ttu-id="f5ab0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f5ab0-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f5ab0-110">Перечисление licenseDetails</span><span class="sxs-lookup"><span data-stu-id="f5ab0-110">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="f5ab0-111">Коллекция объектов licenseDetails</span><span class="sxs-lookup"><span data-stu-id="f5ab0-111">licenseDetails collection</span></span> |<span data-ttu-id="f5ab0-112">Получение списка объектов licenseDetails для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f5ab0-112">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="f5ab0-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="f5ab0-113">Properties</span></span>
| <span data-ttu-id="f5ab0-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="f5ab0-114">Property</span></span>     | <span data-ttu-id="f5ab0-115">Тип</span><span class="sxs-lookup"><span data-stu-id="f5ab0-115">Type</span></span>   |<span data-ttu-id="f5ab0-116">Описание</span><span class="sxs-lookup"><span data-stu-id="f5ab0-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5ab0-117">id</span><span class="sxs-lookup"><span data-stu-id="f5ab0-117">id</span></span>|<span data-ttu-id="f5ab0-118">String</span><span class="sxs-lookup"><span data-stu-id="f5ab0-118">String</span></span>| <span data-ttu-id="f5ab0-119">Уникальный идентификатор для объекта сведений о лицензии.</span><span class="sxs-lookup"><span data-stu-id="f5ab0-119">The unique identifier for the license detail object.</span></span> <span data-ttu-id="f5ab0-120">Только для чтения, ключ, не допускающий значение null</span><span class="sxs-lookup"><span data-stu-id="f5ab0-120">Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="f5ab0-121">сервицепланс</span><span class="sxs-lookup"><span data-stu-id="f5ab0-121">servicePlans</span></span>|<span data-ttu-id="f5ab0-122">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="f5ab0-122">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="f5ab0-123">Сведения о планах обслуживания, назначенных с лицензией.</span><span class="sxs-lookup"><span data-stu-id="f5ab0-123">Information about the service plans assigned with the license.</span></span> <span data-ttu-id="f5ab0-124">Только для чтения, не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="f5ab0-124">Read-only, Not nullable</span></span> |
|<span data-ttu-id="f5ab0-125">skuId</span><span class="sxs-lookup"><span data-stu-id="f5ab0-125">skuId</span></span>|<span data-ttu-id="f5ab0-126">Guid</span><span class="sxs-lookup"><span data-stu-id="f5ab0-126">Guid</span></span>| <span data-ttu-id="f5ab0-127">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="f5ab0-127">Unique identifier (GUID) for the service SKU.</span></span> <span data-ttu-id="f5ab0-128">Равно свойству skuId в связанном объекте [SubscribedSku](subscribedsku.md) .</span><span class="sxs-lookup"><span data-stu-id="f5ab0-128">Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object.</span></span> <span data-ttu-id="f5ab0-129">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="f5ab0-129">Read-only</span></span> |
|<span data-ttu-id="f5ab0-130">скупартнумбер</span><span class="sxs-lookup"><span data-stu-id="f5ab0-130">skuPartNumber</span></span>|<span data-ttu-id="f5ab0-131">String</span><span class="sxs-lookup"><span data-stu-id="f5ab0-131">String</span></span>| <span data-ttu-id="f5ab0-132">Имя уникального отображаемого номера SKU.</span><span class="sxs-lookup"><span data-stu-id="f5ab0-132">Unique SKU display name.</span></span> <span data-ttu-id="f5ab0-133">Равно Скупартнумбер для связанного объекта [SubscribedSku](subscribedsku.md) ; Пример: "AAD_Premium".</span><span class="sxs-lookup"><span data-stu-id="f5ab0-133">Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium".</span></span> <span data-ttu-id="f5ab0-134">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="f5ab0-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="f5ab0-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="f5ab0-135">Relationships</span></span>
<span data-ttu-id="f5ab0-136">Нет</span><span class="sxs-lookup"><span data-stu-id="f5ab0-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5ab0-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f5ab0-137">JSON representation</span></span>
<span data-ttu-id="f5ab0-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f5ab0-138">Here is a JSON representation of the resource.</span></span>

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


