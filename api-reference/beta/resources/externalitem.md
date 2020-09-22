---
title: Тип ресурса Екстерналитем
description: Элемент, индексируемый с помощью подключения поиска Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: d775cfefa7a0cd1fdb87a291ba7ac61bb4b40782
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013708"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="f92c3-103">Тип ресурса Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f92c3-103">externalItem resource type</span></span>

<span data-ttu-id="f92c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f92c3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f92c3-105">Элемент, индексируемый с помощью [подключения](externalconnection.md)поиска Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f92c3-105">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="f92c3-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f92c3-106">Methods</span></span>

| <span data-ttu-id="f92c3-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f92c3-107">Method</span></span>                                                        | <span data-ttu-id="f92c3-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f92c3-108">Return Type</span></span>                     | <span data-ttu-id="f92c3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f92c3-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="f92c3-110">Создание Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f92c3-110">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="f92c3-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="f92c3-111">externalItem</span></span>](externalitem.md) | <span data-ttu-id="f92c3-112">Создайте объект Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="f92c3-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="f92c3-113">Получение Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f92c3-113">Get externalItem</span></span>](../api/externalitem-get.md)                | [<span data-ttu-id="f92c3-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="f92c3-114">externalItem</span></span>](externalitem.md) | <span data-ttu-id="f92c3-115">Получение Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="f92c3-115">Get an externalItem.</span></span>    |
| [<span data-ttu-id="f92c3-116">Обновление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f92c3-116">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="f92c3-117">externalItem</span><span class="sxs-lookup"><span data-stu-id="f92c3-117">externalItem</span></span>](externalitem.md) | <span data-ttu-id="f92c3-118">Обновление Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="f92c3-118">Update an externalItem.</span></span> |
| [<span data-ttu-id="f92c3-119">Удаление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f92c3-119">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="f92c3-120">Нет</span><span class="sxs-lookup"><span data-stu-id="f92c3-120">None</span></span>                            | <span data-ttu-id="f92c3-121">Удаление Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="f92c3-121">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="f92c3-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="f92c3-122">Properties</span></span>

| <span data-ttu-id="f92c3-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="f92c3-123">Property</span></span>   | <span data-ttu-id="f92c3-124">Тип</span><span class="sxs-lookup"><span data-stu-id="f92c3-124">Type</span></span>                     | <span data-ttu-id="f92c3-125">Описание</span><span class="sxs-lookup"><span data-stu-id="f92c3-125">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="f92c3-126">списки</span><span class="sxs-lookup"><span data-stu-id="f92c3-126">acl</span></span>        | <span data-ttu-id="f92c3-127">Коллекция [списков управления доступом](acl.md)</span><span class="sxs-lookup"><span data-stu-id="f92c3-127">[acl](acl.md) collection</span></span> | <span data-ttu-id="f92c3-128">Массив элементов управления доступом.</span><span class="sxs-lookup"><span data-stu-id="f92c3-128">An array of access control entries.</span></span> <span data-ttu-id="f92c3-129">Каждая запись указывает доступ, который предоставляется пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="f92c3-129">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="f92c3-130">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f92c3-130">Required.</span></span> |
| <span data-ttu-id="f92c3-131">содержимое</span><span class="sxs-lookup"><span data-stu-id="f92c3-131">content</span></span>    | [<span data-ttu-id="f92c3-132">екстерналитемконтент</span><span class="sxs-lookup"><span data-stu-id="f92c3-132">externalItemContent</span></span>](externalitemcontent.md) | <span data-ttu-id="f92c3-133">Представление содержимого элемента в виде обычного текста или в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="f92c3-133">A plain-text or HTML representation of the contents of the item.</span></span> <span data-ttu-id="f92c3-134">Текст в этом свойстве является полнотекстовым индексированным.</span><span class="sxs-lookup"><span data-stu-id="f92c3-134">The text in this property is full-text indexed.</span></span> <span data-ttu-id="f92c3-135">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f92c3-135">Optional.</span></span> |
| <span data-ttu-id="f92c3-136">id</span><span class="sxs-lookup"><span data-stu-id="f92c3-136">id</span></span>         | <span data-ttu-id="f92c3-137">String</span><span class="sxs-lookup"><span data-stu-id="f92c3-137">String</span></span>                   | <span data-ttu-id="f92c3-138">Предоставленный разработчиком уникальный идентификатор элемента в содержащем [екстерналконнектион](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="f92c3-138">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="f92c3-139">Должен быть буквенно-цифровым и не превышать 128 символов.</span><span class="sxs-lookup"><span data-stu-id="f92c3-139">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="f92c3-140">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f92c3-140">Required.</span></span> |
| <span data-ttu-id="f92c3-141">properties</span><span class="sxs-lookup"><span data-stu-id="f92c3-141">properties</span></span> | <span data-ttu-id="f92c3-142">Объект</span><span class="sxs-lookup"><span data-stu-id="f92c3-142">Object</span></span>                   | <span data-ttu-id="f92c3-143">Контейнер свойств со свойствами элемента.</span><span class="sxs-lookup"><span data-stu-id="f92c3-143">A property bag with the properties of the item.</span></span> <span data-ttu-id="f92c3-144">Свойства должны соответствовать [схеме](schema.md) , определенной для [екстерналконнектион](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="f92c3-144">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="f92c3-145">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f92c3-145">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f92c3-146">Связи</span><span class="sxs-lookup"><span data-stu-id="f92c3-146">Relationships</span></span>

<span data-ttu-id="f92c3-147">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f92c3-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f92c3-148">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="f92c3-148">JSON representation</span></span>

<span data-ttu-id="f92c3-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f92c3-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItem",
  "baseType": "",
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


