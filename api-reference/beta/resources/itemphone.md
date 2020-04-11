---
title: Тип ресурса Итемфоне
description: Тип ресурса Итемфоне
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 4bc101ca8cbfb063fa1bba3a2ebdb4e6afc2fd57
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229404"
---
# <a name="itemphone-resource-type"></a><span data-ttu-id="71967-103">Тип ресурса Итемфоне</span><span class="sxs-lookup"><span data-stu-id="71967-103">itemPhone resource type</span></span>

<span data-ttu-id="71967-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71967-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71967-105">Представляет подробные сведения о номерах телефонов, связанных с пользователем в различных службах.</span><span class="sxs-lookup"><span data-stu-id="71967-105">Represents detailed information about phone numbers associated with a user in various services.</span></span>

## <a name="methods"></a><span data-ttu-id="71967-106">Методы</span><span class="sxs-lookup"><span data-stu-id="71967-106">Methods</span></span>

| <span data-ttu-id="71967-107">Метод</span><span class="sxs-lookup"><span data-stu-id="71967-107">Method</span></span>                                               | <span data-ttu-id="71967-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="71967-108">Return Type</span></span>               | <span data-ttu-id="71967-109">Описание</span><span class="sxs-lookup"><span data-stu-id="71967-109">Description</span></span>                                                       |
|:-----------------------------------------------------|:--------------------------|:------------------------------------------------------------------|
| [<span data-ttu-id="71967-110">Получение Итемфоне</span><span class="sxs-lookup"><span data-stu-id="71967-110">Get itemPhone</span></span>](../api/itemphone-get.md)             | [<span data-ttu-id="71967-111">итемфоне</span><span class="sxs-lookup"><span data-stu-id="71967-111">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="71967-112">Чтение свойств и связей объекта **итемфоне** .</span><span class="sxs-lookup"><span data-stu-id="71967-112">Read the properties and relationships of an **itemPhone** object.</span></span> |
| [<span data-ttu-id="71967-113">Обновление Итемфоне</span><span class="sxs-lookup"><span data-stu-id="71967-113">Update itemPhone</span></span>](../api/itemphone-update.md)       | [<span data-ttu-id="71967-114">итемфоне</span><span class="sxs-lookup"><span data-stu-id="71967-114">itemPhone</span></span>](itemphone.md) | <span data-ttu-id="71967-115">Обновление объекта **итемфоне** .</span><span class="sxs-lookup"><span data-stu-id="71967-115">Update an **itemPhone** object.</span></span>                                   |
| [<span data-ttu-id="71967-116">Удаление Итемфоне</span><span class="sxs-lookup"><span data-stu-id="71967-116">Delete itemPhone</span></span>](../api/itemphone-delete.md)       | <span data-ttu-id="71967-117">Нет</span><span class="sxs-lookup"><span data-stu-id="71967-117">None</span></span>                      | <span data-ttu-id="71967-118">Удаление объекта **итемфоне** .</span><span class="sxs-lookup"><span data-stu-id="71967-118">Delete an **itemPhone** object.</span></span>                                   |

## <a name="properties"></a><span data-ttu-id="71967-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="71967-119">Properties</span></span>

| <span data-ttu-id="71967-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="71967-120">Property</span></span>     | <span data-ttu-id="71967-121">Тип</span><span class="sxs-lookup"><span data-stu-id="71967-121">Type</span></span>        | <span data-ttu-id="71967-122">Описание</span><span class="sxs-lookup"><span data-stu-id="71967-122">Description</span></span>                                                                                                                     |
|:-------------|:------------|:--------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="71967-123">displayName</span><span class="sxs-lookup"><span data-stu-id="71967-123">displayName</span></span>   |<span data-ttu-id="71967-124">Строка</span><span class="sxs-lookup"><span data-stu-id="71967-124">String</span></span>       | <span data-ttu-id="71967-125">Содержит понятное имя для номера телефона.</span><span class="sxs-lookup"><span data-stu-id="71967-125">Contains a friendly name for the phone number.</span></span>                                                                                  |
|<span data-ttu-id="71967-126">число</span><span class="sxs-lookup"><span data-stu-id="71967-126">number</span></span>        |<span data-ttu-id="71967-127">String</span><span class="sxs-lookup"><span data-stu-id="71967-127">String</span></span>       | <span data-ttu-id="71967-128">Содержит номер телефона.</span><span class="sxs-lookup"><span data-stu-id="71967-128">Contains the phone number.</span></span>                                                                                                      |
|<span data-ttu-id="71967-129">type</span><span class="sxs-lookup"><span data-stu-id="71967-129">type</span></span>          |<span data-ttu-id="71967-130">string</span><span class="sxs-lookup"><span data-stu-id="71967-130">string</span></span>       | <span data-ttu-id="71967-131">Возможные значения: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span><span class="sxs-lookup"><span data-stu-id="71967-131">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71967-132">Связи</span><span class="sxs-lookup"><span data-stu-id="71967-132">Relationships</span></span>

<span data-ttu-id="71967-133">Нет</span><span class="sxs-lookup"><span data-stu-id="71967-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71967-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71967-134">JSON representation</span></span>

<span data-ttu-id="71967-135">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71967-135">The following is a JSON representation of the resource.</span></span>

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
