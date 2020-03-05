---
title: Тип ресурса схемы
description: Описывает тип контента и способ индексирования каждого свойства элементов в подключении Microsoft Search.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 40c31536f8d53c46563fda4205d34deee0501beb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520958"
---
# <a name="schema-resource-type"></a><span data-ttu-id="44ec1-103">Тип ресурса схемы</span><span class="sxs-lookup"><span data-stu-id="44ec1-103">schema resource type</span></span>

<span data-ttu-id="44ec1-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="44ec1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44ec1-105">Описывает тип контента и способ индексирования каждого свойства элементов в [подключении](externalconnection.md)Microsoft Search.</span><span class="sxs-lookup"><span data-stu-id="44ec1-105">Describes the type of content and how to index each property in items in a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="44ec1-106">Методы</span><span class="sxs-lookup"><span data-stu-id="44ec1-106">Methods</span></span>

| <span data-ttu-id="44ec1-107">Метод</span><span class="sxs-lookup"><span data-stu-id="44ec1-107">Method</span></span>                                                    | <span data-ttu-id="44ec1-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="44ec1-108">Return Type</span></span>                   | <span data-ttu-id="44ec1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="44ec1-109">Description</span></span> |
|:----------------------------------------------------------|:------------------------------|:--|
| [<span data-ttu-id="44ec1-110">Создание схемы</span><span class="sxs-lookup"><span data-stu-id="44ec1-110">Create schema</span></span>](../api/externalconnection-post-schema.md) | <span data-ttu-id="44ec1-111">Нет *или* [схема](schema.md)</span><span class="sxs-lookup"><span data-stu-id="44ec1-111">None *or* [schema](schema.md)</span></span> | <span data-ttu-id="44ec1-112">Регистрация схемы подключения.</span><span class="sxs-lookup"><span data-stu-id="44ec1-112">Register connection schema.</span></span> |
| [<span data-ttu-id="44ec1-113">Получение схемы</span><span class="sxs-lookup"><span data-stu-id="44ec1-113">Get schema</span></span>](../api/schema-get.md)                        | [<span data-ttu-id="44ec1-114">schema</span><span class="sxs-lookup"><span data-stu-id="44ec1-114">schema</span></span>](schema.md)           | <span data-ttu-id="44ec1-115">Чтение свойств объекта Schema.</span><span class="sxs-lookup"><span data-stu-id="44ec1-115">Read properties of a schema object.</span></span> |

## <a name="properties"></a><span data-ttu-id="44ec1-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="44ec1-116">Properties</span></span>

| <span data-ttu-id="44ec1-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="44ec1-117">Property</span></span>   | <span data-ttu-id="44ec1-118">Тип</span><span class="sxs-lookup"><span data-stu-id="44ec1-118">Type</span></span>                               | <span data-ttu-id="44ec1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="44ec1-119">Description</span></span>                |
|:-----------|:-----------------------------------|:---------------------------|
| <span data-ttu-id="44ec1-120">baseType</span><span class="sxs-lookup"><span data-stu-id="44ec1-120">baseType</span></span>   | <span data-ttu-id="44ec1-121">String</span><span class="sxs-lookup"><span data-stu-id="44ec1-121">String</span></span>                             | <span data-ttu-id="44ec1-122">Возможные значения: `microsoft.graph.externalItem` и `microsoft.graph.externalFile`.</span><span class="sxs-lookup"><span data-stu-id="44ec1-122">Possible values are `microsoft.graph.externalItem` and `microsoft.graph.externalFile`.</span></span> <span data-ttu-id="44ec1-123">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="44ec1-123">Required.</span></span> |
| <span data-ttu-id="44ec1-124">properties</span><span class="sxs-lookup"><span data-stu-id="44ec1-124">properties</span></span> | <span data-ttu-id="44ec1-125">Коллекция [свойств](property.md)</span><span class="sxs-lookup"><span data-stu-id="44ec1-125">[property](property.md) collection</span></span> | <span data-ttu-id="44ec1-126">Свойства, заданные для элементов в подключении.</span><span class="sxs-lookup"><span data-stu-id="44ec1-126">The properties defined for the items in the connection.</span></span> <span data-ttu-id="44ec1-127">Минимальное число свойств — 1, максимальное — 64.</span><span class="sxs-lookup"><span data-stu-id="44ec1-127">The minimum number of properties is one, the maximum is 64.</span></span> <span data-ttu-id="44ec1-128">Является обязательным `baseType` , если задано значение `microsoft.graph.externalItem`.</span><span class="sxs-lookup"><span data-stu-id="44ec1-128">Required when `baseType` is set to `microsoft.graph.externalItem`.</span></span> <span data-ttu-id="44ec1-129">Игнорируется `baseType` , если задано значение `microsoft.graph.externalFile`.</span><span class="sxs-lookup"><span data-stu-id="44ec1-129">Ignored when `baseType` is set to `microsoft.graph.externalFile`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="44ec1-130">Связи</span><span class="sxs-lookup"><span data-stu-id="44ec1-130">Relationships</span></span>

<span data-ttu-id="44ec1-131">Нет</span><span class="sxs-lookup"><span data-stu-id="44ec1-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44ec1-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44ec1-132">JSON representation</span></span>

<span data-ttu-id="44ec1-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44ec1-133">The following is a JSON representation of the resource.</span></span>

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
