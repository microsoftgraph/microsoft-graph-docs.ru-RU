---
title: Тип ресурса Екстерналитем
description: Элемент, индексируемый с помощью подключения поиска Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 900cf61536204ff5924aea0de268befad6626b37
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704173"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="f3a2e-103">Тип ресурса Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f3a2e-103">externalItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3a2e-104">Элемент, индексируемый с помощью [подключения](externalconnection.md)поиска Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f3a2e-104">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="f3a2e-105">Методы</span><span class="sxs-lookup"><span data-stu-id="f3a2e-105">Methods</span></span>

| <span data-ttu-id="f3a2e-106">Метод</span><span class="sxs-lookup"><span data-stu-id="f3a2e-106">Method</span></span>                                                        | <span data-ttu-id="f3a2e-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f3a2e-107">Return Type</span></span>                     | <span data-ttu-id="f3a2e-108">Описание</span><span class="sxs-lookup"><span data-stu-id="f3a2e-108">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="f3a2e-109">Создание Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f3a2e-109">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="f3a2e-110">externalItem</span><span class="sxs-lookup"><span data-stu-id="f3a2e-110">externalItem</span></span>](externalitem.md) | <span data-ttu-id="f3a2e-111">Создайте объект Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="f3a2e-111">Create an externalItem.</span></span> |
| [<span data-ttu-id="f3a2e-112">Обновление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f3a2e-112">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="f3a2e-113">externalItem</span><span class="sxs-lookup"><span data-stu-id="f3a2e-113">externalItem</span></span>](externalitem.md) | <span data-ttu-id="f3a2e-114">Обновление Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="f3a2e-114">Update an externalItem.</span></span> |
| [<span data-ttu-id="f3a2e-115">Удаление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f3a2e-115">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="f3a2e-116">Нет</span><span class="sxs-lookup"><span data-stu-id="f3a2e-116">None</span></span>                            | <span data-ttu-id="f3a2e-117">Удаление Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="f3a2e-117">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="f3a2e-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="f3a2e-118">Properties</span></span>

| <span data-ttu-id="f3a2e-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="f3a2e-119">Property</span></span>   | <span data-ttu-id="f3a2e-120">Тип</span><span class="sxs-lookup"><span data-stu-id="f3a2e-120">Type</span></span>                     | <span data-ttu-id="f3a2e-121">Описание</span><span class="sxs-lookup"><span data-stu-id="f3a2e-121">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="f3a2e-122">списки</span><span class="sxs-lookup"><span data-stu-id="f3a2e-122">acl</span></span>        | <span data-ttu-id="f3a2e-123">Коллекция [списков управления доступом](acl.md)</span><span class="sxs-lookup"><span data-stu-id="f3a2e-123">[acl](acl.md) collection</span></span> | <span data-ttu-id="f3a2e-124">Массив элементов управления доступом.</span><span class="sxs-lookup"><span data-stu-id="f3a2e-124">An array of access control entries.</span></span> <span data-ttu-id="f3a2e-125">Каждая запись указывает доступ, который предоставляется пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="f3a2e-125">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="f3a2e-126">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f3a2e-126">Required.</span></span> |
| <span data-ttu-id="f3a2e-127">content</span><span class="sxs-lookup"><span data-stu-id="f3a2e-127">content</span></span>    | <span data-ttu-id="f3a2e-128">String</span><span class="sxs-lookup"><span data-stu-id="f3a2e-128">String</span></span>                   | <span data-ttu-id="f3a2e-129">Представление содержимого элемента в виде обычного текста.</span><span class="sxs-lookup"><span data-stu-id="f3a2e-129">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="f3a2e-130">Текст в этом свойстве является полнотекстовым индексированным.</span><span class="sxs-lookup"><span data-stu-id="f3a2e-130">The text in this property is full-text indexed.</span></span> <span data-ttu-id="f3a2e-131">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="f3a2e-131">Optional.</span></span> |
| <span data-ttu-id="f3a2e-132">id</span><span class="sxs-lookup"><span data-stu-id="f3a2e-132">id</span></span>         | <span data-ttu-id="f3a2e-133">String</span><span class="sxs-lookup"><span data-stu-id="f3a2e-133">String</span></span>                   | <span data-ttu-id="f3a2e-134">Предоставленный разработчиком уникальный идентификатор элемента в содержащем [екстерналконнектион](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="f3a2e-134">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="f3a2e-135">Должен быть буквенно-цифровым и не превышать 128 символов.</span><span class="sxs-lookup"><span data-stu-id="f3a2e-135">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="f3a2e-136">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f3a2e-136">Required.</span></span> |
| <span data-ttu-id="f3a2e-137">properties</span><span class="sxs-lookup"><span data-stu-id="f3a2e-137">properties</span></span> | <span data-ttu-id="f3a2e-138">Объект</span><span class="sxs-lookup"><span data-stu-id="f3a2e-138">Object</span></span>                   | <span data-ttu-id="f3a2e-139">Контейнер свойств со свойствами элемента.</span><span class="sxs-lookup"><span data-stu-id="f3a2e-139">A property bag with the properties of the item.</span></span> <span data-ttu-id="f3a2e-140">Свойства должны соответствовать [схеме](schema.md) , определенной для [екстерналконнектион](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="f3a2e-140">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="f3a2e-141">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="f3a2e-141">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f3a2e-142">Связи</span><span class="sxs-lookup"><span data-stu-id="f3a2e-142">Relationships</span></span>

<span data-ttu-id="f3a2e-143">Нет</span><span class="sxs-lookup"><span data-stu-id="f3a2e-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3a2e-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f3a2e-144">JSON representation</span></span>

<span data-ttu-id="f3a2e-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f3a2e-145">The following is a JSON representation of the resource.</span></span>

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
  "content": "String",
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
