---
title: Тип ресурса Итемфоне
description: Тип ресурса Итемфоне
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 2ba1fce4492bfacb3a44f21a0fc55ddd8d37b068
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950439"
---
# <a name="itemphone-resource-type"></a><span data-ttu-id="e211a-103">Тип ресурса Итемфоне</span><span class="sxs-lookup"><span data-stu-id="e211a-103">itemPhone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e211a-104">Представляет подробные сведения о номерах телефонов, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="e211a-104">Represents detailed information about phone numbers associated with a user in various services.</span></span>

## <a name="methods"></a><span data-ttu-id="e211a-105">Методы</span><span class="sxs-lookup"><span data-stu-id="e211a-105">Methods</span></span>

| <span data-ttu-id="e211a-106">Метод</span><span class="sxs-lookup"><span data-stu-id="e211a-106">Method</span></span>                                     | <span data-ttu-id="e211a-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="e211a-107">Return Type</span></span>               | <span data-ttu-id="e211a-108">Описание</span><span class="sxs-lookup"><span data-stu-id="e211a-108">Description</span></span>                                            |
|:-------------------------------------------|:--------------------------|:-------------------------------------------------------|
| [<span data-ttu-id="e211a-109">Получение Итемфоне</span><span class="sxs-lookup"><span data-stu-id="e211a-109">Get itemPhone</span></span>](../api/itemphone-get.md)   | [<span data-ttu-id="e211a-110">итемфоне</span><span class="sxs-lookup"><span data-stu-id="e211a-110">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="e211a-111">Чтение свойств и связей объекта **итемфоне** .</span><span class="sxs-lookup"><span data-stu-id="e211a-111">Read the properties and relationships of an **itemPhone** object.</span></span> |
| [<span data-ttu-id="e211a-112">Обновление Итемфоне</span><span class="sxs-lookup"><span data-stu-id="e211a-112">Update itemPhone</span></span>](../api/itemphone-update.md)       | [<span data-ttu-id="e211a-113">итемфоне</span><span class="sxs-lookup"><span data-stu-id="e211a-113">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="e211a-114">Обновление объекта **итемфоне** .</span><span class="sxs-lookup"><span data-stu-id="e211a-114">Update an **itemPhone** object.</span></span>                               |
| [<span data-ttu-id="e211a-115">Удаление Итемфоне</span><span class="sxs-lookup"><span data-stu-id="e211a-115">Delete itemPhone</span></span>](../api/itemphone-delete.md)       | <span data-ttu-id="e211a-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="e211a-116">None</span></span>                      | <span data-ttu-id="e211a-117">Удаление объекта **итемфоне** .</span><span class="sxs-lookup"><span data-stu-id="e211a-117">Delete an **itemPhone** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="e211a-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="e211a-118">Properties</span></span>

| <span data-ttu-id="e211a-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="e211a-119">Property</span></span>     | <span data-ttu-id="e211a-120">Тип</span><span class="sxs-lookup"><span data-stu-id="e211a-120">Type</span></span>        | <span data-ttu-id="e211a-121">Описание</span><span class="sxs-lookup"><span data-stu-id="e211a-121">Description</span></span>                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="e211a-122">displayName</span><span class="sxs-lookup"><span data-stu-id="e211a-122">displayName</span></span>   |<span data-ttu-id="e211a-123">Строка</span><span class="sxs-lookup"><span data-stu-id="e211a-123">String</span></span>       | <span data-ttu-id="e211a-124">Содержит понятное имя для номера телефона.</span><span class="sxs-lookup"><span data-stu-id="e211a-124">Contains a friendly name for the phone number.</span></span>                                                                                  |
|<span data-ttu-id="e211a-125">число</span><span class="sxs-lookup"><span data-stu-id="e211a-125">number</span></span>        |<span data-ttu-id="e211a-126">String</span><span class="sxs-lookup"><span data-stu-id="e211a-126">String</span></span>       | <span data-ttu-id="e211a-127">Содержит номер телефона.</span><span class="sxs-lookup"><span data-stu-id="e211a-127">Contains the phone number.</span></span>                                                                                                       |
|<span data-ttu-id="e211a-128">type</span><span class="sxs-lookup"><span data-stu-id="e211a-128">type</span></span>          |<span data-ttu-id="e211a-129">string</span><span class="sxs-lookup"><span data-stu-id="e211a-129">string</span></span>       | <span data-ttu-id="e211a-130">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="e211a-130">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e211a-131">Связи</span><span class="sxs-lookup"><span data-stu-id="e211a-131">Relationships</span></span>

<span data-ttu-id="e211a-132">Нет</span><span class="sxs-lookup"><span data-stu-id="e211a-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e211a-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e211a-133">JSON representation</span></span>

<span data-ttu-id="e211a-134">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e211a-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemPhone",
  "baseType": ""
}-->

```json
{
  "displayName": "String",
  "number": "String",
  "type": "string"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemPhone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
