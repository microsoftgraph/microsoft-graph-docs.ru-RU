---
title: Тип ресурса Итемфоне
description: Тип ресурса Итемфоне
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 48c585a05043b4f17e5e7406eb44b9150b5e5bdc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523067"
---
# <a name="itemphone-resource-type"></a><span data-ttu-id="70823-103">Тип ресурса Итемфоне</span><span class="sxs-lookup"><span data-stu-id="70823-103">itemPhone resource type</span></span>

<span data-ttu-id="70823-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="70823-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70823-105">Представляет подробные сведения о номерах телефонов, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="70823-105">Represents detailed information about phone numbers associated with a user in various services.</span></span>

## <a name="methods"></a><span data-ttu-id="70823-106">Методы</span><span class="sxs-lookup"><span data-stu-id="70823-106">Methods</span></span>

| <span data-ttu-id="70823-107">Метод</span><span class="sxs-lookup"><span data-stu-id="70823-107">Method</span></span>                                     | <span data-ttu-id="70823-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="70823-108">Return Type</span></span>               | <span data-ttu-id="70823-109">Описание</span><span class="sxs-lookup"><span data-stu-id="70823-109">Description</span></span>                                            |
|:-------------------------------------------|:--------------------------|:-------------------------------------------------------|
| [<span data-ttu-id="70823-110">Получение Итемфоне</span><span class="sxs-lookup"><span data-stu-id="70823-110">Get itemPhone</span></span>](../api/itemphone-get.md)   | [<span data-ttu-id="70823-111">итемфоне</span><span class="sxs-lookup"><span data-stu-id="70823-111">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="70823-112">Чтение свойств и связей объекта **итемфоне** .</span><span class="sxs-lookup"><span data-stu-id="70823-112">Read the properties and relationships of an **itemPhone** object.</span></span> |
| [<span data-ttu-id="70823-113">Обновление Итемфоне</span><span class="sxs-lookup"><span data-stu-id="70823-113">Update itemPhone</span></span>](../api/itemphone-update.md)       | [<span data-ttu-id="70823-114">итемфоне</span><span class="sxs-lookup"><span data-stu-id="70823-114">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="70823-115">Обновление объекта **итемфоне** .</span><span class="sxs-lookup"><span data-stu-id="70823-115">Update an **itemPhone** object.</span></span>                               |
| [<span data-ttu-id="70823-116">Удаление Итемфоне</span><span class="sxs-lookup"><span data-stu-id="70823-116">Delete itemPhone</span></span>](../api/itemphone-delete.md)       | <span data-ttu-id="70823-117">Нет</span><span class="sxs-lookup"><span data-stu-id="70823-117">None</span></span>                      | <span data-ttu-id="70823-118">Удаление объекта **итемфоне** .</span><span class="sxs-lookup"><span data-stu-id="70823-118">Delete an **itemPhone** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="70823-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="70823-119">Properties</span></span>

| <span data-ttu-id="70823-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="70823-120">Property</span></span>     | <span data-ttu-id="70823-121">Тип</span><span class="sxs-lookup"><span data-stu-id="70823-121">Type</span></span>        | <span data-ttu-id="70823-122">Описание</span><span class="sxs-lookup"><span data-stu-id="70823-122">Description</span></span>                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="70823-123">displayName</span><span class="sxs-lookup"><span data-stu-id="70823-123">displayName</span></span>   |<span data-ttu-id="70823-124">Строка</span><span class="sxs-lookup"><span data-stu-id="70823-124">String</span></span>       | <span data-ttu-id="70823-125">Содержит понятное имя для номера телефона.</span><span class="sxs-lookup"><span data-stu-id="70823-125">Contains a friendly name for the phone number.</span></span>                                                                                  |
|<span data-ttu-id="70823-126">число</span><span class="sxs-lookup"><span data-stu-id="70823-126">number</span></span>        |<span data-ttu-id="70823-127">String</span><span class="sxs-lookup"><span data-stu-id="70823-127">String</span></span>       | <span data-ttu-id="70823-128">Содержит номер телефона.</span><span class="sxs-lookup"><span data-stu-id="70823-128">Contains the phone number.</span></span>                                                                                                       |
|<span data-ttu-id="70823-129">type</span><span class="sxs-lookup"><span data-stu-id="70823-129">type</span></span>          |<span data-ttu-id="70823-130">string</span><span class="sxs-lookup"><span data-stu-id="70823-130">string</span></span>       | <span data-ttu-id="70823-131">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="70823-131">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="70823-132">Связи</span><span class="sxs-lookup"><span data-stu-id="70823-132">Relationships</span></span>

<span data-ttu-id="70823-133">Нет</span><span class="sxs-lookup"><span data-stu-id="70823-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="70823-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="70823-134">JSON representation</span></span>

<span data-ttu-id="70823-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70823-135">The following is a JSON representation of the resource.</span></span>

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
