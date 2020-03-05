---
title: Тип ресурса Екстерналитем
description: Элемент, индексируемый с помощью подключения поиска Microsoft.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e115135bedecfe4b055e028d5c19902a068c8a53
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498702"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="f677c-103">Тип ресурса Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f677c-103">externalItem resource type</span></span>

<span data-ttu-id="f677c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f677c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f677c-105">Элемент, индексируемый с помощью [подключения](externalconnection.md)поиска Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f677c-105">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="f677c-106">Методы</span><span class="sxs-lookup"><span data-stu-id="f677c-106">Methods</span></span>

| <span data-ttu-id="f677c-107">Метод</span><span class="sxs-lookup"><span data-stu-id="f677c-107">Method</span></span>                                                        | <span data-ttu-id="f677c-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="f677c-108">Return Type</span></span>                     | <span data-ttu-id="f677c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f677c-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="f677c-110">Создание Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f677c-110">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="f677c-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="f677c-111">externalItem</span></span>](externalitem.md) | <span data-ttu-id="f677c-112">Создайте объект Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="f677c-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="f677c-113">Обновление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f677c-113">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="f677c-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="f677c-114">externalItem</span></span>](externalitem.md) | <span data-ttu-id="f677c-115">Обновление Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="f677c-115">Update an externalItem.</span></span> |
| [<span data-ttu-id="f677c-116">Удаление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="f677c-116">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="f677c-117">Нет</span><span class="sxs-lookup"><span data-stu-id="f677c-117">None</span></span>                            | <span data-ttu-id="f677c-118">Удаление Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="f677c-118">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="f677c-119">Свойства</span><span class="sxs-lookup"><span data-stu-id="f677c-119">Properties</span></span>

| <span data-ttu-id="f677c-120">Свойство</span><span class="sxs-lookup"><span data-stu-id="f677c-120">Property</span></span>   | <span data-ttu-id="f677c-121">Тип</span><span class="sxs-lookup"><span data-stu-id="f677c-121">Type</span></span>                     | <span data-ttu-id="f677c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="f677c-122">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="f677c-123">списки</span><span class="sxs-lookup"><span data-stu-id="f677c-123">acl</span></span>        | <span data-ttu-id="f677c-124">Коллекция [списков управления доступом](acl.md)</span><span class="sxs-lookup"><span data-stu-id="f677c-124">[acl](acl.md) collection</span></span> | <span data-ttu-id="f677c-125">Массив элементов управления доступом.</span><span class="sxs-lookup"><span data-stu-id="f677c-125">An array of access control entries.</span></span> <span data-ttu-id="f677c-126">Каждая запись указывает доступ, который предоставляется пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="f677c-126">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="f677c-127">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="f677c-127">Required.</span></span> |
| <span data-ttu-id="f677c-128">content</span><span class="sxs-lookup"><span data-stu-id="f677c-128">content</span></span>    | <span data-ttu-id="f677c-129">String</span><span class="sxs-lookup"><span data-stu-id="f677c-129">String</span></span>                   | <span data-ttu-id="f677c-130">Представление содержимого элемента в виде обычного текста.</span><span class="sxs-lookup"><span data-stu-id="f677c-130">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="f677c-131">Текст в этом свойстве является полнотекстовым индексированным.</span><span class="sxs-lookup"><span data-stu-id="f677c-131">The text in this property is full-text indexed.</span></span> <span data-ttu-id="f677c-132">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="f677c-132">Optional.</span></span> |
| <span data-ttu-id="f677c-133">id</span><span class="sxs-lookup"><span data-stu-id="f677c-133">id</span></span>         | <span data-ttu-id="f677c-134">String</span><span class="sxs-lookup"><span data-stu-id="f677c-134">String</span></span>                   | <span data-ttu-id="f677c-135">Предоставленный разработчиком уникальный идентификатор элемента в содержащем [екстерналконнектион](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="f677c-135">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="f677c-136">Должен быть буквенно-цифровым и не превышать 128 символов.</span><span class="sxs-lookup"><span data-stu-id="f677c-136">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="f677c-137">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="f677c-137">Required.</span></span> |
| <span data-ttu-id="f677c-138">properties</span><span class="sxs-lookup"><span data-stu-id="f677c-138">properties</span></span> | <span data-ttu-id="f677c-139">Объект</span><span class="sxs-lookup"><span data-stu-id="f677c-139">Object</span></span>                   | <span data-ttu-id="f677c-140">Контейнер свойств со свойствами элемента.</span><span class="sxs-lookup"><span data-stu-id="f677c-140">A property bag with the properties of the item.</span></span> <span data-ttu-id="f677c-141">Свойства должны соответствовать [схеме](schema.md) , определенной для [екстерналконнектион](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="f677c-141">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="f677c-142">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="f677c-142">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f677c-143">Связи</span><span class="sxs-lookup"><span data-stu-id="f677c-143">Relationships</span></span>

<span data-ttu-id="f677c-144">Нет</span><span class="sxs-lookup"><span data-stu-id="f677c-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f677c-145">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f677c-145">JSON representation</span></span>

<span data-ttu-id="f677c-146">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f677c-146">The following is a JSON representation of the resource.</span></span>

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
