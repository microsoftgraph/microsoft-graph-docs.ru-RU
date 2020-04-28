---
title: Тип ресурса Екстерналитем
description: Элемент, индексируемый с помощью подключения поиска Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e1497528e759a2fb5556aed3e9b936b1c9797ee0
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805658"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="f3fb4-103">Тип ресурса Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f3fb4-103">externalItem resource type</span></span>

<span data-ttu-id="f3fb4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3fb4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3fb4-105">Элемент, индексируемый с помощью [подключения](externalconnection.md)поиска Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f3fb4-105">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="f3fb4-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f3fb4-106">Methods</span></span>

| <span data-ttu-id="f3fb4-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f3fb4-107">Method</span></span>                                                        | <span data-ttu-id="f3fb4-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f3fb4-108">Return Type</span></span>                     | <span data-ttu-id="f3fb4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f3fb4-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="f3fb4-110">Создание Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f3fb4-110">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="f3fb4-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="f3fb4-111">externalItem</span></span>](externalitem.md) | <span data-ttu-id="f3fb4-112">Создайте объект Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="f3fb4-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="f3fb4-113">Обновление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f3fb4-113">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="f3fb4-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="f3fb4-114">externalItem</span></span>](externalitem.md) | <span data-ttu-id="f3fb4-115">Обновление Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="f3fb4-115">Update an externalItem.</span></span> |
| [<span data-ttu-id="f3fb4-116">Удаление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f3fb4-116">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="f3fb4-117">Нет</span><span class="sxs-lookup"><span data-stu-id="f3fb4-117">None</span></span>                            | <span data-ttu-id="f3fb4-118">Удаление Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="f3fb4-118">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="f3fb4-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3fb4-119">Properties</span></span>

| <span data-ttu-id="f3fb4-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3fb4-120">Property</span></span>   | <span data-ttu-id="f3fb4-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f3fb4-121">Type</span></span>                     | <span data-ttu-id="f3fb4-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f3fb4-122">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="f3fb4-123">списки</span><span class="sxs-lookup"><span data-stu-id="f3fb4-123">acl</span></span>        | <span data-ttu-id="f3fb4-124">Коллекция [списков управления доступом](acl.md)</span><span class="sxs-lookup"><span data-stu-id="f3fb4-124">[acl](acl.md) collection</span></span> | <span data-ttu-id="f3fb4-125">Массив элементов управления доступом.</span><span class="sxs-lookup"><span data-stu-id="f3fb4-125">An array of access control entries.</span></span> <span data-ttu-id="f3fb4-126">Каждая запись указывает доступ, который предоставляется пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="f3fb4-126">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="f3fb4-127">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3fb4-127">Required.</span></span> |
| <span data-ttu-id="f3fb4-128">содержимое</span><span class="sxs-lookup"><span data-stu-id="f3fb4-128">content</span></span>    | [<span data-ttu-id="f3fb4-129">екстерналитемконтент</span><span class="sxs-lookup"><span data-stu-id="f3fb4-129">externalItemContent</span></span>](externalitemcontent.md) | <span data-ttu-id="f3fb4-130">Представление содержимого элемента в виде обычного текста или в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="f3fb4-130">A plain-text or HTML representation of the contents of the item.</span></span> <span data-ttu-id="f3fb4-131">Текст в этом свойстве является полнотекстовым индексированным.</span><span class="sxs-lookup"><span data-stu-id="f3fb4-131">The text in this property is full-text indexed.</span></span> <span data-ttu-id="f3fb4-132">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="f3fb4-132">Optional.</span></span> |
| <span data-ttu-id="f3fb4-133">id</span><span class="sxs-lookup"><span data-stu-id="f3fb4-133">id</span></span>         | <span data-ttu-id="f3fb4-134">String</span><span class="sxs-lookup"><span data-stu-id="f3fb4-134">String</span></span>                   | <span data-ttu-id="f3fb4-135">Предоставленный разработчиком уникальный идентификатор элемента в содержащем [екстерналконнектион](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="f3fb4-135">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="f3fb4-136">Должен быть буквенно-цифровым и не превышать 128 символов.</span><span class="sxs-lookup"><span data-stu-id="f3fb4-136">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="f3fb4-137">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3fb4-137">Required.</span></span> |
| <span data-ttu-id="f3fb4-138">properties</span><span class="sxs-lookup"><span data-stu-id="f3fb4-138">properties</span></span> | <span data-ttu-id="f3fb4-139">Объект</span><span class="sxs-lookup"><span data-stu-id="f3fb4-139">Object</span></span>                   | <span data-ttu-id="f3fb4-140">Контейнер свойств со свойствами элемента.</span><span class="sxs-lookup"><span data-stu-id="f3fb4-140">A property bag with the properties of the item.</span></span> <span data-ttu-id="f3fb4-141">Свойства должны соответствовать [схеме](schema.md) , определенной для [екстерналконнектион](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="f3fb4-141">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="f3fb4-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f3fb4-142">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f3fb4-143">Связи</span><span class="sxs-lookup"><span data-stu-id="f3fb4-143">Relationships</span></span>

<span data-ttu-id="f3fb4-144">Нет</span><span class="sxs-lookup"><span data-stu-id="f3fb4-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3fb4-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3fb4-145">JSON representation</span></span>

<span data-ttu-id="f3fb4-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3fb4-146">The following is a JSON representation of the resource.</span></span>

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
