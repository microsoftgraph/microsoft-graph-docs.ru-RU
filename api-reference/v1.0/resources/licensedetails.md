---
title: Тип ресурса licenseDetails
description: Содержит сведения о лицензии, назначенной пользователю.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0d6f5824823af71f5ce7c1a63dce9d73eca8e5c6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447593"
---
# <a name="licensedetails-resource-type"></a><span data-ttu-id="4f0da-103">Тип ресурса licenseDetails</span><span class="sxs-lookup"><span data-stu-id="4f0da-103">licenseDetails resource type</span></span>

<span data-ttu-id="4f0da-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4f0da-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4f0da-105">Содержит сведения о лицензии, назначенной пользователю.</span><span class="sxs-lookup"><span data-stu-id="4f0da-105">Contains information about a license assigned to a user.</span></span>

## <a name="methods"></a><span data-ttu-id="4f0da-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4f0da-106">Methods</span></span>

| <span data-ttu-id="4f0da-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4f0da-107">Method</span></span>           | <span data-ttu-id="4f0da-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4f0da-108">Return Type</span></span>    |<span data-ttu-id="4f0da-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4f0da-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4f0da-110">Перечисление licenseDetails</span><span class="sxs-lookup"><span data-stu-id="4f0da-110">List licenseDetails</span></span>](../api/user-list-licensedetails.md) | <span data-ttu-id="4f0da-111">Коллекция объектов licenseDetails</span><span class="sxs-lookup"><span data-stu-id="4f0da-111">licenseDetails collection</span></span> |<span data-ttu-id="4f0da-112">Получение списка объектов licenseDetails для пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f0da-112">Retrieve a list of licenseDetails objects for a user.</span></span>|

<!--|[Get licenseDetails](../api/licensedetails-get.md) | licenseDetails |Read properties and relationships of a licenseDetails object.|-->

## <a name="properties"></a><span data-ttu-id="4f0da-113">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f0da-113">Properties</span></span>
| <span data-ttu-id="4f0da-114">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f0da-114">Property</span></span>     | <span data-ttu-id="4f0da-115">Тип</span><span class="sxs-lookup"><span data-stu-id="4f0da-115">Type</span></span>   |<span data-ttu-id="4f0da-116">Описание</span><span class="sxs-lookup"><span data-stu-id="4f0da-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f0da-117">id</span><span class="sxs-lookup"><span data-stu-id="4f0da-117">id</span></span>|<span data-ttu-id="4f0da-118">String</span><span class="sxs-lookup"><span data-stu-id="4f0da-118">String</span></span>| <span data-ttu-id="4f0da-119">Уникальный идентификатор для объекта сведений о лицензии.</span><span class="sxs-lookup"><span data-stu-id="4f0da-119">The unique identifier for the license detail object.</span></span> <span data-ttu-id="4f0da-120">Только для чтения, ключ, не допускающий значение null</span><span class="sxs-lookup"><span data-stu-id="4f0da-120">Read-only, Key, Not nullable</span></span> |
|<span data-ttu-id="4f0da-121">сервицепланс</span><span class="sxs-lookup"><span data-stu-id="4f0da-121">servicePlans</span></span>|<span data-ttu-id="4f0da-122">Коллекция [servicePlanInfo](serviceplaninfo.md)</span><span class="sxs-lookup"><span data-stu-id="4f0da-122">[servicePlanInfo](serviceplaninfo.md) collection</span></span>| <span data-ttu-id="4f0da-123">Сведения о планах обслуживания, назначенных с лицензией.</span><span class="sxs-lookup"><span data-stu-id="4f0da-123">Information about the service plans assigned with the license.</span></span> <span data-ttu-id="4f0da-124">Только для чтения, не допускает значение null</span><span class="sxs-lookup"><span data-stu-id="4f0da-124">Read-only, Not nullable</span></span> |
|<span data-ttu-id="4f0da-125">skuId</span><span class="sxs-lookup"><span data-stu-id="4f0da-125">skuId</span></span>|<span data-ttu-id="4f0da-126">Guid</span><span class="sxs-lookup"><span data-stu-id="4f0da-126">Guid</span></span>| <span data-ttu-id="4f0da-127">Уникальный идентификатор (GUID) для SKU службы.</span><span class="sxs-lookup"><span data-stu-id="4f0da-127">Unique identifier (GUID) for the service SKU.</span></span> <span data-ttu-id="4f0da-128">Равно свойству skuId в связанном объекте [SubscribedSku](subscribedsku.md) .</span><span class="sxs-lookup"><span data-stu-id="4f0da-128">Equal to the skuId property on the related [SubscribedSku](subscribedsku.md) object.</span></span> <span data-ttu-id="4f0da-129">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="4f0da-129">Read-only</span></span> |
|<span data-ttu-id="4f0da-130">скупартнумбер</span><span class="sxs-lookup"><span data-stu-id="4f0da-130">skuPartNumber</span></span>|<span data-ttu-id="4f0da-131">String</span><span class="sxs-lookup"><span data-stu-id="4f0da-131">String</span></span>| <span data-ttu-id="4f0da-132">Имя уникального отображаемого номера SKU.</span><span class="sxs-lookup"><span data-stu-id="4f0da-132">Unique SKU display name.</span></span> <span data-ttu-id="4f0da-133">Равно Скупартнумбер для связанного объекта [SubscribedSku](subscribedsku.md) ; Пример: "AAD_Premium".</span><span class="sxs-lookup"><span data-stu-id="4f0da-133">Equal to the skuPartNumber on the related [SubscribedSku](subscribedsku.md) object; for example: "AAD_Premium".</span></span> <span data-ttu-id="4f0da-134">Только для чтения</span><span class="sxs-lookup"><span data-stu-id="4f0da-134">Read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="4f0da-135">Связи</span><span class="sxs-lookup"><span data-stu-id="4f0da-135">Relationships</span></span>
<span data-ttu-id="4f0da-136">Нет</span><span class="sxs-lookup"><span data-stu-id="4f0da-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f0da-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f0da-137">JSON representation</span></span>
<span data-ttu-id="4f0da-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f0da-138">Here is a JSON representation of the resource.</span></span>

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
