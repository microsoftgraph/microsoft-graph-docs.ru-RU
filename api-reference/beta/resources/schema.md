---
title: Тип ресурса схемы
description: Описывает тип контента и способ индексирования каждого свойства элементов в подключении Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 0d5182e68fd1b1d53abb5b3fa623f3048abfe723
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083969"
---
# <a name="schema-resource-type"></a><span data-ttu-id="cc037-103">Тип ресурса схемы</span><span class="sxs-lookup"><span data-stu-id="cc037-103">schema resource type</span></span>

<span data-ttu-id="cc037-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc037-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc037-105">Описывает тип контента и способ индексирования каждого свойства элементов в [подключении](externalconnection.md)Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="cc037-105">Describes the type of content and how to index each property in items in a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="cc037-106">Методы</span><span class="sxs-lookup"><span data-stu-id="cc037-106">Methods</span></span>

| <span data-ttu-id="cc037-107">Метод</span><span class="sxs-lookup"><span data-stu-id="cc037-107">Method</span></span>                                                    | <span data-ttu-id="cc037-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="cc037-108">Return Type</span></span>                   | <span data-ttu-id="cc037-109">Описание</span><span class="sxs-lookup"><span data-stu-id="cc037-109">Description</span></span> |
|:----------------------------------------------------------|:------------------------------|:--|
| [<span data-ttu-id="cc037-110">Создание схемы</span><span class="sxs-lookup"><span data-stu-id="cc037-110">Create schema</span></span>](../api/externalconnection-post-schema.md) | <span data-ttu-id="cc037-111">Нет *или* [схема](schema.md)</span><span class="sxs-lookup"><span data-stu-id="cc037-111">None *or* [schema](schema.md)</span></span> | <span data-ttu-id="cc037-112">Регистрация схемы подключения.</span><span class="sxs-lookup"><span data-stu-id="cc037-112">Register connection schema.</span></span> |
| [<span data-ttu-id="cc037-113">Получение схемы</span><span class="sxs-lookup"><span data-stu-id="cc037-113">Get schema</span></span>](../api/schema-get.md)                        | [<span data-ttu-id="cc037-114">schema</span><span class="sxs-lookup"><span data-stu-id="cc037-114">schema</span></span>](schema.md)           | <span data-ttu-id="cc037-115">Чтение свойств объекта Schema.</span><span class="sxs-lookup"><span data-stu-id="cc037-115">Read properties of a schema object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cc037-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc037-116">Properties</span></span>

| <span data-ttu-id="cc037-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc037-117">Property</span></span>   | <span data-ttu-id="cc037-118">Тип</span><span class="sxs-lookup"><span data-stu-id="cc037-118">Type</span></span>                               | <span data-ttu-id="cc037-119">Описание</span><span class="sxs-lookup"><span data-stu-id="cc037-119">Description</span></span>                |
|:-----------|:-----------------------------------|:---------------------------|
| <span data-ttu-id="cc037-120">baseType</span><span class="sxs-lookup"><span data-stu-id="cc037-120">baseType</span></span>   | <span data-ttu-id="cc037-121">Строка</span><span class="sxs-lookup"><span data-stu-id="cc037-121">String</span></span>                             | <span data-ttu-id="cc037-122">Необходимо указать значение `microsoft.graph.externalItem`.</span><span class="sxs-lookup"><span data-stu-id="cc037-122">Must be set to `microsoft.graph.externalItem`.</span></span> <span data-ttu-id="cc037-123">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cc037-123">Required.</span></span> |
| <span data-ttu-id="cc037-124">properties</span><span class="sxs-lookup"><span data-stu-id="cc037-124">properties</span></span> | <span data-ttu-id="cc037-125">Коллекция [свойств](property.md)</span><span class="sxs-lookup"><span data-stu-id="cc037-125">[property](property.md) collection</span></span> | <span data-ttu-id="cc037-126">Свойства, заданные для элементов в подключении.</span><span class="sxs-lookup"><span data-stu-id="cc037-126">The properties defined for the items in the connection.</span></span> <span data-ttu-id="cc037-127">Минимальное число свойств — 1, максимальное — 128.</span><span class="sxs-lookup"><span data-stu-id="cc037-127">The minimum number of properties is one, the maximum is 128.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cc037-128">Связи</span><span class="sxs-lookup"><span data-stu-id="cc037-128">Relationships</span></span>

<span data-ttu-id="cc037-129">Нет</span><span class="sxs-lookup"><span data-stu-id="cc037-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc037-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc037-130">JSON representation</span></span>

<span data-ttu-id="cc037-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc037-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.schema",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "baseType": "String",
  "id": "String (identifier)",
  "properties": [{"@odata.type": "microsoft.graph.property"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "schema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


