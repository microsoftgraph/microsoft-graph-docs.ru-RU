---
title: Тип ресурса Екстерналитем
description: Элемент, добавляемый в подключение Microsoft Graph.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: ec2c66c91612738295ac4ba49524593d61ff70e4
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193409"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="72e17-103">Тип ресурса Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="72e17-103">externalItem resource type</span></span>

<span data-ttu-id="72e17-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72e17-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="72e17-105">Элемент, добавляемый в [Подключение](externalconnection.md)Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="72e17-105">An item added to a Microsoft Graph [connection](externalconnection.md).</span></span> 

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="72e17-106">Методы</span><span class="sxs-lookup"><span data-stu-id="72e17-106">Methods</span></span>

| <span data-ttu-id="72e17-107">Метод</span><span class="sxs-lookup"><span data-stu-id="72e17-107">Method</span></span>                                                        | <span data-ttu-id="72e17-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="72e17-108">Return Type</span></span>                     | <span data-ttu-id="72e17-109">Описание</span><span class="sxs-lookup"><span data-stu-id="72e17-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="72e17-110">Создание Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="72e17-110">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="72e17-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="72e17-111">externalItem</span></span>](externalitem.md) | <span data-ttu-id="72e17-112">Создайте объект Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="72e17-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="72e17-113">Получение Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="72e17-113">Get externalItem</span></span>](../api/externalitem-get.md)                | [<span data-ttu-id="72e17-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="72e17-114">externalItem</span></span>](externalitem.md) | <span data-ttu-id="72e17-115">Получение Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="72e17-115">Get an externalItem.</span></span>    |
| [<span data-ttu-id="72e17-116">Обновление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="72e17-116">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="72e17-117">externalItem</span><span class="sxs-lookup"><span data-stu-id="72e17-117">externalItem</span></span>](externalitem.md) | <span data-ttu-id="72e17-118">Обновление Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="72e17-118">Update an externalItem.</span></span> |
| [<span data-ttu-id="72e17-119">Удаление Екстерналитем</span><span class="sxs-lookup"><span data-stu-id="72e17-119">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="72e17-120">Нет</span><span class="sxs-lookup"><span data-stu-id="72e17-120">None</span></span>                            | <span data-ttu-id="72e17-121">Удаление Екстерналитем.</span><span class="sxs-lookup"><span data-stu-id="72e17-121">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="72e17-122">Свойства</span><span class="sxs-lookup"><span data-stu-id="72e17-122">Properties</span></span>

| <span data-ttu-id="72e17-123">Свойство</span><span class="sxs-lookup"><span data-stu-id="72e17-123">Property</span></span>   | <span data-ttu-id="72e17-124">Тип</span><span class="sxs-lookup"><span data-stu-id="72e17-124">Type</span></span>                     | <span data-ttu-id="72e17-125">Описание</span><span class="sxs-lookup"><span data-stu-id="72e17-125">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="72e17-126">списки</span><span class="sxs-lookup"><span data-stu-id="72e17-126">acl</span></span>        | <span data-ttu-id="72e17-127">Коллекция [списков управления доступом](acl.md)</span><span class="sxs-lookup"><span data-stu-id="72e17-127">[acl](acl.md) collection</span></span> | <span data-ttu-id="72e17-128">Массив элементов управления доступом.</span><span class="sxs-lookup"><span data-stu-id="72e17-128">An array of access control entries.</span></span> <span data-ttu-id="72e17-129">Каждая запись указывает доступ, который предоставляется пользователю или группе.</span><span class="sxs-lookup"><span data-stu-id="72e17-129">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="72e17-130">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="72e17-130">Required.</span></span> |
| <span data-ttu-id="72e17-131">содержимое</span><span class="sxs-lookup"><span data-stu-id="72e17-131">content</span></span>    | [<span data-ttu-id="72e17-132">екстерналитемконтент</span><span class="sxs-lookup"><span data-stu-id="72e17-132">externalItemContent</span></span>](externalitemcontent.md) | <span data-ttu-id="72e17-133">Представление содержимого элемента в виде обычного текста.</span><span class="sxs-lookup"><span data-stu-id="72e17-133">A plain-text  representation of the contents of the item.</span></span> <span data-ttu-id="72e17-134">Текст в этом свойстве является полнотекстовым индексированным.</span><span class="sxs-lookup"><span data-stu-id="72e17-134">The text in this property is full-text indexed.</span></span> <span data-ttu-id="72e17-135">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="72e17-135">Optional.</span></span> |
| <span data-ttu-id="72e17-136">id</span><span class="sxs-lookup"><span data-stu-id="72e17-136">id</span></span>         | <span data-ttu-id="72e17-137">String</span><span class="sxs-lookup"><span data-stu-id="72e17-137">String</span></span>                   | <span data-ttu-id="72e17-138">Предоставленный разработчиком уникальный идентификатор элемента в содержащем [екстерналконнектион](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="72e17-138">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="72e17-139">Должен быть буквенно-цифровым и не превышать 128 символов.</span><span class="sxs-lookup"><span data-stu-id="72e17-139">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="72e17-140">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="72e17-140">Required.</span></span> |
| <span data-ttu-id="72e17-141">properties</span><span class="sxs-lookup"><span data-stu-id="72e17-141">properties</span></span> | <span data-ttu-id="72e17-142">Объект</span><span class="sxs-lookup"><span data-stu-id="72e17-142">Object</span></span>                   | <span data-ttu-id="72e17-143">Контейнер свойств со свойствами элемента.</span><span class="sxs-lookup"><span data-stu-id="72e17-143">A property bag with the properties of the item.</span></span> <span data-ttu-id="72e17-144">Свойства должны соответствовать [схеме](schema.md) , определенной для [екстерналконнектион](externalconnection.md).</span><span class="sxs-lookup"><span data-stu-id="72e17-144">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="72e17-145">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72e17-145">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="72e17-146">Связи</span><span class="sxs-lookup"><span data-stu-id="72e17-146">Relationships</span></span>

<span data-ttu-id="72e17-147">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="72e17-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="72e17-148">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="72e17-148">JSON representation</span></span>

<span data-ttu-id="72e17-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72e17-149">The following is a JSON representation of the resource.</span></span>

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
