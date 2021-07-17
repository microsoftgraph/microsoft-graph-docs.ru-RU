---
title: тип ресурса externalItem
description: Элемент, добавленный к подключению microsoft Graph.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8660365d5d08d0084066cea3349e841269469241
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467859"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="bd6f1-103">тип ресурса externalItem</span><span class="sxs-lookup"><span data-stu-id="bd6f1-103">externalItem resource type</span></span>

<span data-ttu-id="bd6f1-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="bd6f1-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd6f1-105">Элемент, добавленный к подключению microsoft [Graph.](externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="bd6f1-105">An item added to a Microsoft Graph [connection](externalconnectors-externalconnection.md).</span></span>

## <a name="methods"></a><span data-ttu-id="bd6f1-106">Методы</span><span class="sxs-lookup"><span data-stu-id="bd6f1-106">Methods</span></span>

| <span data-ttu-id="bd6f1-107">Метод</span><span class="sxs-lookup"><span data-stu-id="bd6f1-107">Method</span></span>                                                        | <span data-ttu-id="bd6f1-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bd6f1-108">Return Type</span></span>                     | <span data-ttu-id="bd6f1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bd6f1-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="bd6f1-110">Создание externalItem</span><span class="sxs-lookup"><span data-stu-id="bd6f1-110">Create externalItem</span></span>](../api/externalconnectors-externalconnection-put-items.md) | [<span data-ttu-id="bd6f1-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="bd6f1-111">externalItem</span></span>](externalconnectors-externalitem.md) | <span data-ttu-id="bd6f1-112">Создание externalItem.</span><span class="sxs-lookup"><span data-stu-id="bd6f1-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="bd6f1-113">Get externalItem</span><span class="sxs-lookup"><span data-stu-id="bd6f1-113">Get externalItem</span></span>](../api/externalconnectors-externalitem-get.md)                | [<span data-ttu-id="bd6f1-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="bd6f1-114">externalItem</span></span>](externalconnectors-externalitem.md) | <span data-ttu-id="bd6f1-115">Получите externalItem.</span><span class="sxs-lookup"><span data-stu-id="bd6f1-115">Get an externalItem.</span></span>    |
| [<span data-ttu-id="bd6f1-116">Обновление externalItem</span><span class="sxs-lookup"><span data-stu-id="bd6f1-116">Update externalItem</span></span>](../api/externalconnectors-externalitem-update.md)          | [<span data-ttu-id="bd6f1-117">externalItem</span><span class="sxs-lookup"><span data-stu-id="bd6f1-117">externalItem</span></span>](externalconnectors-externalitem.md) | <span data-ttu-id="bd6f1-118">Обновление externalItem.</span><span class="sxs-lookup"><span data-stu-id="bd6f1-118">Update an externalItem.</span></span> |
| [<span data-ttu-id="bd6f1-119">Удаление externalItem</span><span class="sxs-lookup"><span data-stu-id="bd6f1-119">Delete externalItem</span></span>](../api/externalconnectors-externalitem-delete.md)          | <span data-ttu-id="bd6f1-120">Нет</span><span class="sxs-lookup"><span data-stu-id="bd6f1-120">None</span></span>                            | <span data-ttu-id="bd6f1-121">Удаление externalItem.</span><span class="sxs-lookup"><span data-stu-id="bd6f1-121">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="bd6f1-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="bd6f1-122">Properties</span></span>

| <span data-ttu-id="bd6f1-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="bd6f1-123">Property</span></span>   | <span data-ttu-id="bd6f1-124">Тип</span><span class="sxs-lookup"><span data-stu-id="bd6f1-124">Type</span></span>                     | <span data-ttu-id="bd6f1-125">Описание</span><span class="sxs-lookup"><span data-stu-id="bd6f1-125">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="bd6f1-126">acl</span><span class="sxs-lookup"><span data-stu-id="bd6f1-126">acl</span></span>        | <span data-ttu-id="bd6f1-127">[коллекция microsoft.graph.externalConnectors.acl](externalconnectors-acl.md)</span><span class="sxs-lookup"><span data-stu-id="bd6f1-127">[microsoft.graph.externalConnectors.acl](externalconnectors-acl.md) collection</span></span> | <span data-ttu-id="bd6f1-128">Массив записей управления доступом.</span><span class="sxs-lookup"><span data-stu-id="bd6f1-128">An array of access control entries.</span></span> <span data-ttu-id="bd6f1-129">Каждая запись указывает доступ, предоставленный пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="bd6f1-129">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="bd6f1-130">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="bd6f1-130">Required.</span></span> |
| <span data-ttu-id="bd6f1-131">содержимое</span><span class="sxs-lookup"><span data-stu-id="bd6f1-131">content</span></span>    | [<span data-ttu-id="bd6f1-132">microsoft.graph.externalConnectors.externalItemContent</span><span class="sxs-lookup"><span data-stu-id="bd6f1-132">microsoft.graph.externalConnectors.externalItemContent</span></span>](externalconnectors-externalitemcontent.md) | <span data-ttu-id="bd6f1-133">Простое текстовое представление содержимого элемента.</span><span class="sxs-lookup"><span data-stu-id="bd6f1-133">A plain-text  representation of the contents of the item.</span></span> <span data-ttu-id="bd6f1-134">Текст в этом свойстве индексироваться с полным текстом.</span><span class="sxs-lookup"><span data-stu-id="bd6f1-134">The text in this property is full-text indexed.</span></span> <span data-ttu-id="bd6f1-135">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="bd6f1-135">Optional.</span></span> |
| <span data-ttu-id="bd6f1-136">id</span><span class="sxs-lookup"><span data-stu-id="bd6f1-136">id</span></span>         | <span data-ttu-id="bd6f1-137">String</span><span class="sxs-lookup"><span data-stu-id="bd6f1-137">String</span></span>                   | <span data-ttu-id="bd6f1-138">Уникальный ID элемента, предоставленного разработчиком, в пределах элемента, содержащего [externalConnection.](externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="bd6f1-138">Developer-provided unique ID of the item within the containing [externalConnection](externalconnectors-externalconnection.md).</span></span> <span data-ttu-id="bd6f1-139">Должно быть альфа-числом и не более 128 символов.</span><span class="sxs-lookup"><span data-stu-id="bd6f1-139">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="bd6f1-140">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="bd6f1-140">Required.</span></span> |
| <span data-ttu-id="bd6f1-141">properties</span><span class="sxs-lookup"><span data-stu-id="bd6f1-141">properties</span></span> | <span data-ttu-id="bd6f1-142">Объект</span><span class="sxs-lookup"><span data-stu-id="bd6f1-142">Object</span></span>                   | <span data-ttu-id="bd6f1-143">Пакет свойств со свойствами элемента.</span><span class="sxs-lookup"><span data-stu-id="bd6f1-143">A property bag with the properties of the item.</span></span> <span data-ttu-id="bd6f1-144">Свойства должны соответствовать [схеме,](externalconnectors-schema.md) определенной для [externalConnection.](externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="bd6f1-144">The properties MUST conform to the [schema](externalconnectors-schema.md) defined for the [externalConnection](externalconnectors-externalconnection.md).</span></span> <span data-ttu-id="bd6f1-145">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bd6f1-145">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bd6f1-146">Связи</span><span class="sxs-lookup"><span data-stu-id="bd6f1-146">Relationships</span></span>

<span data-ttu-id="bd6f1-147">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bd6f1-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd6f1-148">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="bd6f1-148">JSON representation</span></span>

<span data-ttu-id="bd6f1-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bd6f1-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.externalConnectors.externalItem",
  "keyProperty": "id"
}-->

```json
{
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    }
  ],
  "id": "String (identifier)",
  "properties": "Object",
  "content": { "@odata.type": "microsoft.graph.externalConnectors.externalItemContent" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: microsoft.graph.externalConnectors.externalItem/properties:\r\n      Referenced type microsoft.graph.object is not defined in the doc set! Potential suggestion: microsoft.graph.directoryObject"
  ]
}-->
