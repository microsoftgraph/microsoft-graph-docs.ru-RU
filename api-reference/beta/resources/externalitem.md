---
title: Тип ресурса externalItem
description: Элемент, добавленный к подключению Microsoft Graph.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 63f0285427a17280169d31a35c3a622d38a6a8c6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161710"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="7ed8f-103">Тип ресурса externalItem</span><span class="sxs-lookup"><span data-stu-id="7ed8f-103">externalItem resource type</span></span>

<span data-ttu-id="7ed8f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ed8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ed8f-105">Элемент, добавленный в подключение Microsoft [Graph.](externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="7ed8f-105">An item added to a Microsoft Graph [connection](externalconnection.md).</span></span> 

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="7ed8f-106">Методы</span><span class="sxs-lookup"><span data-stu-id="7ed8f-106">Methods</span></span>

| <span data-ttu-id="7ed8f-107">Метод</span><span class="sxs-lookup"><span data-stu-id="7ed8f-107">Method</span></span>                                                        | <span data-ttu-id="7ed8f-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="7ed8f-108">Return Type</span></span>                     | <span data-ttu-id="7ed8f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="7ed8f-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="7ed8f-110">Создание externalItem</span><span class="sxs-lookup"><span data-stu-id="7ed8f-110">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="7ed8f-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="7ed8f-111">externalItem</span></span>](externalitem.md) | <span data-ttu-id="7ed8f-112">Создайте externalItem.</span><span class="sxs-lookup"><span data-stu-id="7ed8f-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="7ed8f-113">Get externalItem</span><span class="sxs-lookup"><span data-stu-id="7ed8f-113">Get externalItem</span></span>](../api/externalitem-get.md)                | [<span data-ttu-id="7ed8f-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="7ed8f-114">externalItem</span></span>](externalitem.md) | <span data-ttu-id="7ed8f-115">Получите externalItem.</span><span class="sxs-lookup"><span data-stu-id="7ed8f-115">Get an externalItem.</span></span>    |
| [<span data-ttu-id="7ed8f-116">Обновление externalItem</span><span class="sxs-lookup"><span data-stu-id="7ed8f-116">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="7ed8f-117">externalItem</span><span class="sxs-lookup"><span data-stu-id="7ed8f-117">externalItem</span></span>](externalitem.md) | <span data-ttu-id="7ed8f-118">Обновление externalItem.</span><span class="sxs-lookup"><span data-stu-id="7ed8f-118">Update an externalItem.</span></span> |
| [<span data-ttu-id="7ed8f-119">Удаление externalItem</span><span class="sxs-lookup"><span data-stu-id="7ed8f-119">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="7ed8f-120">Нет</span><span class="sxs-lookup"><span data-stu-id="7ed8f-120">None</span></span>                            | <span data-ttu-id="7ed8f-121">Удаление externalItem.</span><span class="sxs-lookup"><span data-stu-id="7ed8f-121">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="7ed8f-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ed8f-122">Properties</span></span>

| <span data-ttu-id="7ed8f-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ed8f-123">Property</span></span>   | <span data-ttu-id="7ed8f-124">Тип</span><span class="sxs-lookup"><span data-stu-id="7ed8f-124">Type</span></span>                     | <span data-ttu-id="7ed8f-125">Описание</span><span class="sxs-lookup"><span data-stu-id="7ed8f-125">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="7ed8f-126">acl</span><span class="sxs-lookup"><span data-stu-id="7ed8f-126">acl</span></span>        | <span data-ttu-id="7ed8f-127">[Коллекция acl](acl.md)</span><span class="sxs-lookup"><span data-stu-id="7ed8f-127">[acl](acl.md) collection</span></span> | <span data-ttu-id="7ed8f-128">Массив записей управления доступом.</span><span class="sxs-lookup"><span data-stu-id="7ed8f-128">An array of access control entries.</span></span> <span data-ttu-id="7ed8f-129">Каждая запись указывает доступ, предоставленный пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="7ed8f-129">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="7ed8f-130">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7ed8f-130">Required.</span></span> |
| <span data-ttu-id="7ed8f-131">содержимое</span><span class="sxs-lookup"><span data-stu-id="7ed8f-131">content</span></span>    | [<span data-ttu-id="7ed8f-132">externalItemContent</span><span class="sxs-lookup"><span data-stu-id="7ed8f-132">externalItemContent</span></span>](externalitemcontent.md) | <span data-ttu-id="7ed8f-133">Обычное представление содержимого элемента.</span><span class="sxs-lookup"><span data-stu-id="7ed8f-133">A plain-text  representation of the contents of the item.</span></span> <span data-ttu-id="7ed8f-134">Текст в этом свойстве индексироваться в полном тексте.</span><span class="sxs-lookup"><span data-stu-id="7ed8f-134">The text in this property is full-text indexed.</span></span> <span data-ttu-id="7ed8f-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="7ed8f-135">Optional.</span></span> |
| <span data-ttu-id="7ed8f-136">id</span><span class="sxs-lookup"><span data-stu-id="7ed8f-136">id</span></span>         | <span data-ttu-id="7ed8f-137">String</span><span class="sxs-lookup"><span data-stu-id="7ed8f-137">String</span></span>                   | <span data-ttu-id="7ed8f-138">Предоставленный разработчиком уникальный ИД элемента в пределах содержащего [externalConnection.](externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="7ed8f-138">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="7ed8f-139">Должно быть буквано-цифровая и не более 128 символов.</span><span class="sxs-lookup"><span data-stu-id="7ed8f-139">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="7ed8f-140">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="7ed8f-140">Required.</span></span> |
| <span data-ttu-id="7ed8f-141">properties</span><span class="sxs-lookup"><span data-stu-id="7ed8f-141">properties</span></span> | <span data-ttu-id="7ed8f-142">Объект</span><span class="sxs-lookup"><span data-stu-id="7ed8f-142">Object</span></span>                   | <span data-ttu-id="7ed8f-143">Пакет свойств со свойствами элемента.</span><span class="sxs-lookup"><span data-stu-id="7ed8f-143">A property bag with the properties of the item.</span></span> <span data-ttu-id="7ed8f-144">Свойства ДОЛЖНЫ соответствовать схеме, [определенной](schema.md) для [externalConnection.](externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="7ed8f-144">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="7ed8f-145">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ed8f-145">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7ed8f-146">Связи</span><span class="sxs-lookup"><span data-stu-id="7ed8f-146">Relationships</span></span>

<span data-ttu-id="7ed8f-147">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7ed8f-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ed8f-148">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="7ed8f-148">JSON representation</span></span>

<span data-ttu-id="7ed8f-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7ed8f-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItem",
  "keyProperty": "id"
}-->

```json
{
  "acl": [{"@odata.type": "microsoft.graph.acl"}],
  "content": {"@odata.type": "microsoft.graph.externalItemContent"},
  "id": "String (identifier)",
  "properties": "Object"
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
    "Error: microsoft.graph.externalItem/properties:\r\n      Referenced type microsoft.graph.object is not defined in the doc set! Potential suggestion: microsoft.graph.directoryObject"
  ]
}-->
