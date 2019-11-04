---
title: Тип ресурса Екстерналитем
description: Элемент, индексируемый с помощью подключения поиска Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ffcc69cd71d2508a2ceae568d767dc991af063d6
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938978"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="d4780-103">Тип ресурса Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="d4780-103">externalItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4780-104">Элемент, индексируемый с помощью [подключения](externalconnection.md)поиска Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d4780-104">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d4780-105">Методы</span><span class="sxs-lookup"><span data-stu-id="d4780-105">Methods</span></span>

| <span data-ttu-id="d4780-106">Метод</span><span class="sxs-lookup"><span data-stu-id="d4780-106">Method</span></span>                                                        | <span data-ttu-id="d4780-107">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="d4780-107">Return Type</span></span>                     | <span data-ttu-id="d4780-108">Описание</span><span class="sxs-lookup"><span data-stu-id="d4780-108">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="d4780-109">Создание Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="d4780-109">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="d4780-110">екстерналитем</span><span class="sxs-lookup"><span data-stu-id="d4780-110">externalItem</span></span>](externalitem.md) | <span data-ttu-id="d4780-111">Создайте объект Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="d4780-111">Create an externalItem.</span></span> |
| [<span data-ttu-id="d4780-112">Обновление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="d4780-112">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="d4780-113">екстерналитем</span><span class="sxs-lookup"><span data-stu-id="d4780-113">externalItem</span></span>](externalitem.md) | <span data-ttu-id="d4780-114">Обновление Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="d4780-114">Update an externalItem.</span></span> |
| [<span data-ttu-id="d4780-115">Удаление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="d4780-115">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="d4780-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="d4780-116">None</span></span>                            | <span data-ttu-id="d4780-117">Удаление Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="d4780-117">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="d4780-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4780-118">Properties</span></span>

| <span data-ttu-id="d4780-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4780-119">Property</span></span>   | <span data-ttu-id="d4780-120">Тип</span><span class="sxs-lookup"><span data-stu-id="d4780-120">Type</span></span>                     | <span data-ttu-id="d4780-121">Описание</span><span class="sxs-lookup"><span data-stu-id="d4780-121">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="d4780-122">списки</span><span class="sxs-lookup"><span data-stu-id="d4780-122">acl</span></span>        | <span data-ttu-id="d4780-123">Коллекция [списков управления доступом](acl.md)</span><span class="sxs-lookup"><span data-stu-id="d4780-123">[acl](acl.md) collection</span></span> | <span data-ttu-id="d4780-124">Массив элементов управления доступом.</span><span class="sxs-lookup"><span data-stu-id="d4780-124">An array of access control entries.</span></span> <span data-ttu-id="d4780-125">Каждая запись указывает доступ, который предоставляется пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="d4780-125">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="d4780-126">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="d4780-126">Required.</span></span> |
| <span data-ttu-id="d4780-127">content</span><span class="sxs-lookup"><span data-stu-id="d4780-127">content</span></span>    | <span data-ttu-id="d4780-128">String</span><span class="sxs-lookup"><span data-stu-id="d4780-128">String</span></span>                   | <span data-ttu-id="d4780-129">Представление содержимого элемента в виде обычного текста.</span><span class="sxs-lookup"><span data-stu-id="d4780-129">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="d4780-130">Текст в этом свойстве является полнотекстовым индексированным.</span><span class="sxs-lookup"><span data-stu-id="d4780-130">The text in this property is full-text indexed.</span></span> <span data-ttu-id="d4780-131">Необязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="d4780-131">Optional.</span></span> |
| <span data-ttu-id="d4780-132">id</span><span class="sxs-lookup"><span data-stu-id="d4780-132">id</span></span>         | <span data-ttu-id="d4780-133">Строка</span><span class="sxs-lookup"><span data-stu-id="d4780-133">String</span></span>                   | <span data-ttu-id="d4780-134">Предоставленный разработчиком уникальный идентификатор элемента в содержащем [екстерналконнектион](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="d4780-134">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="d4780-135">Должен быть буквенно-цифровым и не превышать 128 символов.</span><span class="sxs-lookup"><span data-stu-id="d4780-135">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="d4780-136">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="d4780-136">Required.</span></span> |
| <span data-ttu-id="d4780-137">properties</span><span class="sxs-lookup"><span data-stu-id="d4780-137">properties</span></span> | <span data-ttu-id="d4780-138">Object</span><span class="sxs-lookup"><span data-stu-id="d4780-138">Object</span></span>                   | <span data-ttu-id="d4780-139">Контейнер свойств со свойствами элемента.</span><span class="sxs-lookup"><span data-stu-id="d4780-139">A property bag with the properties of the item.</span></span> <span data-ttu-id="d4780-140">Свойства должны соответствовать [схеме](schema.md) , определенной для [екстерналконнектион](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="d4780-140">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="d4780-141">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="d4780-141">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d4780-142">Связи</span><span class="sxs-lookup"><span data-stu-id="d4780-142">Relationships</span></span>

<span data-ttu-id="d4780-143">Нет</span><span class="sxs-lookup"><span data-stu-id="d4780-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4780-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d4780-144">JSON representation</span></span>

<span data-ttu-id="d4780-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4780-145">The following is a JSON representation of the resource.</span></span>

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
