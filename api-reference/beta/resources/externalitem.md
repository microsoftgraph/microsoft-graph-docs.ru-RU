---
title: тип ресурса externalItem
description: Элемент, добавленный к подключению microsoft Graph.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7c570a7e4754724ca4239b7e3dbe128d09db9d75
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366533"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="98f75-103">тип ресурса externalItem</span><span class="sxs-lookup"><span data-stu-id="98f75-103">externalItem resource type</span></span>

<span data-ttu-id="98f75-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98f75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98f75-105">Элемент, добавленный к подключению microsoft [Graph.](externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="98f75-105">An item added to a Microsoft Graph [connection](externalconnection.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="98f75-106">Методы</span><span class="sxs-lookup"><span data-stu-id="98f75-106">Methods</span></span>

| <span data-ttu-id="98f75-107">Метод</span><span class="sxs-lookup"><span data-stu-id="98f75-107">Method</span></span>                                                        | <span data-ttu-id="98f75-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="98f75-108">Return Type</span></span>                     | <span data-ttu-id="98f75-109">Описание</span><span class="sxs-lookup"><span data-stu-id="98f75-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="98f75-110">Создание externalItem</span><span class="sxs-lookup"><span data-stu-id="98f75-110">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="98f75-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="98f75-111">externalItem</span></span>](externalitem.md) | <span data-ttu-id="98f75-112">Создание externalItem.</span><span class="sxs-lookup"><span data-stu-id="98f75-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="98f75-113">Get externalItem</span><span class="sxs-lookup"><span data-stu-id="98f75-113">Get externalItem</span></span>](../api/externalitem-get.md)                | [<span data-ttu-id="98f75-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="98f75-114">externalItem</span></span>](externalitem.md) | <span data-ttu-id="98f75-115">Получите externalItem.</span><span class="sxs-lookup"><span data-stu-id="98f75-115">Get an externalItem.</span></span>    |
| [<span data-ttu-id="98f75-116">Обновление externalItem</span><span class="sxs-lookup"><span data-stu-id="98f75-116">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="98f75-117">externalItem</span><span class="sxs-lookup"><span data-stu-id="98f75-117">externalItem</span></span>](externalitem.md) | <span data-ttu-id="98f75-118">Обновление externalItem.</span><span class="sxs-lookup"><span data-stu-id="98f75-118">Update an externalItem.</span></span> |
| [<span data-ttu-id="98f75-119">Удаление externalItem</span><span class="sxs-lookup"><span data-stu-id="98f75-119">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="98f75-120">Нет</span><span class="sxs-lookup"><span data-stu-id="98f75-120">None</span></span>                            | <span data-ttu-id="98f75-121">Удаление externalItem.</span><span class="sxs-lookup"><span data-stu-id="98f75-121">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="98f75-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="98f75-122">Properties</span></span>

| <span data-ttu-id="98f75-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="98f75-123">Property</span></span>   | <span data-ttu-id="98f75-124">Тип</span><span class="sxs-lookup"><span data-stu-id="98f75-124">Type</span></span>                     | <span data-ttu-id="98f75-125">Описание</span><span class="sxs-lookup"><span data-stu-id="98f75-125">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="98f75-126">acl</span><span class="sxs-lookup"><span data-stu-id="98f75-126">acl</span></span>        | <span data-ttu-id="98f75-127">[коллекция acl](acl.md)</span><span class="sxs-lookup"><span data-stu-id="98f75-127">[acl](acl.md) collection</span></span> | <span data-ttu-id="98f75-128">Массив записей управления доступом.</span><span class="sxs-lookup"><span data-stu-id="98f75-128">An array of access control entries.</span></span> <span data-ttu-id="98f75-129">Каждая запись указывает доступ, предоставленный пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="98f75-129">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="98f75-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98f75-130">Required.</span></span> |
| <span data-ttu-id="98f75-131">содержимое</span><span class="sxs-lookup"><span data-stu-id="98f75-131">content</span></span>    | [<span data-ttu-id="98f75-132">externalItemContent</span><span class="sxs-lookup"><span data-stu-id="98f75-132">externalItemContent</span></span>](externalitemcontent.md) | <span data-ttu-id="98f75-133">Простое текстовое представление содержимого элемента.</span><span class="sxs-lookup"><span data-stu-id="98f75-133">A plain-text  representation of the contents of the item.</span></span> <span data-ttu-id="98f75-134">Текст в этом свойстве индексироваться с полным текстом.</span><span class="sxs-lookup"><span data-stu-id="98f75-134">The text in this property is full-text indexed.</span></span> <span data-ttu-id="98f75-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="98f75-135">Optional.</span></span> |
| <span data-ttu-id="98f75-136">id</span><span class="sxs-lookup"><span data-stu-id="98f75-136">id</span></span>         | <span data-ttu-id="98f75-137">String</span><span class="sxs-lookup"><span data-stu-id="98f75-137">String</span></span>                   | <span data-ttu-id="98f75-138">Уникальный ID элемента, предоставленного разработчиком, в пределах элемента, содержащего [externalConnection.](externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="98f75-138">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="98f75-139">Должно быть альфа-числом и не более 128 символов.</span><span class="sxs-lookup"><span data-stu-id="98f75-139">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="98f75-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98f75-140">Required.</span></span> |
| <span data-ttu-id="98f75-141">properties</span><span class="sxs-lookup"><span data-stu-id="98f75-141">properties</span></span> | <span data-ttu-id="98f75-142">Объект</span><span class="sxs-lookup"><span data-stu-id="98f75-142">Object</span></span>                   | <span data-ttu-id="98f75-143">Пакет свойств со свойствами элемента.</span><span class="sxs-lookup"><span data-stu-id="98f75-143">A property bag with the properties of the item.</span></span> <span data-ttu-id="98f75-144">Свойства должны соответствовать [схеме,](schema.md) определенной для [externalConnection.](externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="98f75-144">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="98f75-145">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98f75-145">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="98f75-146">Связи</span><span class="sxs-lookup"><span data-stu-id="98f75-146">Relationships</span></span>

<span data-ttu-id="98f75-147">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="98f75-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="98f75-148">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="98f75-148">JSON representation</span></span>

<span data-ttu-id="98f75-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98f75-149">The following is a JSON representation of the resource.</span></span>

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
