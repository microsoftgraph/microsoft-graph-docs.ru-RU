---
title: Тип ресурса Екстерналитем
description: Элемент, индексируемый с помощью подключения поиска Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5a396d41ffaf0e602a586635296586cbdce42f50
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866828"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="9de9d-103">Тип ресурса Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="9de9d-103">externalItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9de9d-104">Элемент, индексируемый с помощью [подключения](externalconnection.md)поиска Microsoft.</span><span class="sxs-lookup"><span data-stu-id="9de9d-104">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="9de9d-105">Методы</span><span class="sxs-lookup"><span data-stu-id="9de9d-105">Methods</span></span>

| <span data-ttu-id="9de9d-106">Метод</span><span class="sxs-lookup"><span data-stu-id="9de9d-106">Method</span></span>                                                        | <span data-ttu-id="9de9d-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9de9d-107">Return Type</span></span>                     | <span data-ttu-id="9de9d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="9de9d-108">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="9de9d-109">Создание Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="9de9d-109">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="9de9d-110">externalItem</span><span class="sxs-lookup"><span data-stu-id="9de9d-110">externalItem</span></span>](externalitem.md) | <span data-ttu-id="9de9d-111">Создайте объект Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="9de9d-111">Create an externalItem.</span></span> |
| [<span data-ttu-id="9de9d-112">Обновление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="9de9d-112">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="9de9d-113">externalItem</span><span class="sxs-lookup"><span data-stu-id="9de9d-113">externalItem</span></span>](externalitem.md) | <span data-ttu-id="9de9d-114">Обновление Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="9de9d-114">Update an externalItem.</span></span> |
| [<span data-ttu-id="9de9d-115">Удаление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="9de9d-115">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="9de9d-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="9de9d-116">None</span></span>                            | <span data-ttu-id="9de9d-117">Удаление Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="9de9d-117">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="9de9d-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="9de9d-118">Properties</span></span>

| <span data-ttu-id="9de9d-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="9de9d-119">Property</span></span>   | <span data-ttu-id="9de9d-120">Тип</span><span class="sxs-lookup"><span data-stu-id="9de9d-120">Type</span></span>                     | <span data-ttu-id="9de9d-121">Описание</span><span class="sxs-lookup"><span data-stu-id="9de9d-121">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="9de9d-122">списки</span><span class="sxs-lookup"><span data-stu-id="9de9d-122">acl</span></span>        | <span data-ttu-id="9de9d-123">Коллекция [списков управления доступом](acl.md)</span><span class="sxs-lookup"><span data-stu-id="9de9d-123">[acl](acl.md) collection</span></span> | <span data-ttu-id="9de9d-124">Массив элементов управления доступом.</span><span class="sxs-lookup"><span data-stu-id="9de9d-124">An array of access control entries.</span></span> <span data-ttu-id="9de9d-125">Каждая запись указывает доступ, который предоставляется пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="9de9d-125">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="9de9d-126">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="9de9d-126">Required.</span></span> |
| <span data-ttu-id="9de9d-127">content</span><span class="sxs-lookup"><span data-stu-id="9de9d-127">content</span></span>    | <span data-ttu-id="9de9d-128">String</span><span class="sxs-lookup"><span data-stu-id="9de9d-128">String</span></span>                   | <span data-ttu-id="9de9d-129">Представление содержимого элемента в виде обычного текста.</span><span class="sxs-lookup"><span data-stu-id="9de9d-129">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="9de9d-130">Текст в этом свойстве является полнотекстовым индексированным.</span><span class="sxs-lookup"><span data-stu-id="9de9d-130">The text in this property is full-text indexed.</span></span> <span data-ttu-id="9de9d-131">Необязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="9de9d-131">Optional.</span></span> |
| <span data-ttu-id="9de9d-132">id</span><span class="sxs-lookup"><span data-stu-id="9de9d-132">id</span></span>         | <span data-ttu-id="9de9d-133">String</span><span class="sxs-lookup"><span data-stu-id="9de9d-133">String</span></span>                   | <span data-ttu-id="9de9d-134">Предоставленный разработчиком уникальный идентификатор элемента в содержащем [екстерналконнектион](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="9de9d-134">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="9de9d-135">Должен быть буквенно-цифровым и не превышать 128 символов.</span><span class="sxs-lookup"><span data-stu-id="9de9d-135">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="9de9d-136">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="9de9d-136">Required.</span></span> |
| <span data-ttu-id="9de9d-137">properties</span><span class="sxs-lookup"><span data-stu-id="9de9d-137">properties</span></span> | <span data-ttu-id="9de9d-138">Object</span><span class="sxs-lookup"><span data-stu-id="9de9d-138">Object</span></span>                   | <span data-ttu-id="9de9d-139">Контейнер свойств со свойствами элемента.</span><span class="sxs-lookup"><span data-stu-id="9de9d-139">A property bag with the properties of the item.</span></span> <span data-ttu-id="9de9d-140">Свойства должны соответствовать [схеме](schema.md) , определенной для [екстерналконнектион](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="9de9d-140">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="9de9d-141">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="9de9d-141">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9de9d-142">Отношения</span><span class="sxs-lookup"><span data-stu-id="9de9d-142">Relationships</span></span>

<span data-ttu-id="9de9d-143">Нет</span><span class="sxs-lookup"><span data-stu-id="9de9d-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9de9d-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9de9d-144">JSON representation</span></span>

<span data-ttu-id="9de9d-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9de9d-145">The following is a JSON representation of the resource.</span></span>

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
