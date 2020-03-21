---
title: Тип ресурса схемы
description: Описывает тип контента и способ индексирования каждого свойства элементов в подключении Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: be9001d1fab756be09e88768f0b34540c14aafcf
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892537"
---
# <a name="schema-resource-type"></a><span data-ttu-id="4e8ab-103">Тип ресурса схемы</span><span class="sxs-lookup"><span data-stu-id="4e8ab-103">schema resource type</span></span>

<span data-ttu-id="4e8ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e8ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e8ab-105">Описывает тип контента и способ индексирования каждого свойства элементов в [подключении](externalconnection.md)Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="4e8ab-105">Describes the type of content and how to index each property in items in a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="4e8ab-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4e8ab-106">Methods</span></span>

| <span data-ttu-id="4e8ab-107">Метод</span><span class="sxs-lookup"><span data-stu-id="4e8ab-107">Method</span></span>                                                    | <span data-ttu-id="4e8ab-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="4e8ab-108">Return Type</span></span>                   | <span data-ttu-id="4e8ab-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4e8ab-109">Description</span></span> |
|:----------------------------------------------------------|:------------------------------|:--|
| [<span data-ttu-id="4e8ab-110">Создание схемы</span><span class="sxs-lookup"><span data-stu-id="4e8ab-110">Create schema</span></span>](../api/externalconnection-post-schema.md) | <span data-ttu-id="4e8ab-111">Нет *или* [схема](schema.md)</span><span class="sxs-lookup"><span data-stu-id="4e8ab-111">None *or* [schema](schema.md)</span></span> | <span data-ttu-id="4e8ab-112">Регистрация схемы подключения.</span><span class="sxs-lookup"><span data-stu-id="4e8ab-112">Register connection schema.</span></span> |
| [<span data-ttu-id="4e8ab-113">Получение схемы</span><span class="sxs-lookup"><span data-stu-id="4e8ab-113">Get schema</span></span>](../api/schema-get.md)                        | [<span data-ttu-id="4e8ab-114">schema</span><span class="sxs-lookup"><span data-stu-id="4e8ab-114">schema</span></span>](schema.md)           | <span data-ttu-id="4e8ab-115">Чтение свойств объекта Schema.</span><span class="sxs-lookup"><span data-stu-id="4e8ab-115">Read properties of a schema object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4e8ab-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="4e8ab-116">Properties</span></span>

| <span data-ttu-id="4e8ab-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="4e8ab-117">Property</span></span>   | <span data-ttu-id="4e8ab-118">Тип</span><span class="sxs-lookup"><span data-stu-id="4e8ab-118">Type</span></span>                               | <span data-ttu-id="4e8ab-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4e8ab-119">Description</span></span>                |
|:-----------|:-----------------------------------|:---------------------------|
| <span data-ttu-id="4e8ab-120">baseType</span><span class="sxs-lookup"><span data-stu-id="4e8ab-120">baseType</span></span>   | <span data-ttu-id="4e8ab-121">String</span><span class="sxs-lookup"><span data-stu-id="4e8ab-121">String</span></span>                             | <span data-ttu-id="4e8ab-122">Необходимо указать значение `microsoft.graph.externalItem`.</span><span class="sxs-lookup"><span data-stu-id="4e8ab-122">Must be set to `microsoft.graph.externalItem`.</span></span> <span data-ttu-id="4e8ab-123">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4e8ab-123">Required.</span></span> |
| <span data-ttu-id="4e8ab-124">properties</span><span class="sxs-lookup"><span data-stu-id="4e8ab-124">properties</span></span> | <span data-ttu-id="4e8ab-125">Коллекция [свойств](property.md)</span><span class="sxs-lookup"><span data-stu-id="4e8ab-125">[property](property.md) collection</span></span> | <span data-ttu-id="4e8ab-126">Свойства, заданные для элементов в подключении.</span><span class="sxs-lookup"><span data-stu-id="4e8ab-126">The properties defined for the items in the connection.</span></span> <span data-ttu-id="4e8ab-127">Минимальное число свойств — 1, максимальное — 64.</span><span class="sxs-lookup"><span data-stu-id="4e8ab-127">The minimum number of properties is one, the maximum is 64.</span></span> |

## <a name="relationships"></a><span data-ttu-id="4e8ab-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="4e8ab-128">Relationships</span></span>

<span data-ttu-id="4e8ab-129">Нет</span><span class="sxs-lookup"><span data-stu-id="4e8ab-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4e8ab-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4e8ab-130">JSON representation</span></span>

<span data-ttu-id="4e8ab-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4e8ab-131">The following is a JSON representation of the resource.</span></span>

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
