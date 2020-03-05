---
title: Тип ресурса свойства
description: Определение свойства схемы для подключения поиска Майкрософт.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 48a61c9f26a7f5b90e41fc2cd36334d4061449dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521385"
---
# <a name="property-resource-type"></a><span data-ttu-id="b416c-103">Тип ресурса свойства</span><span class="sxs-lookup"><span data-stu-id="b416c-103">property resource type</span></span>

<span data-ttu-id="b416c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b416c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b416c-105">Определение свойства [схемы](schema.md) для [подключения](externalconnection.md)поиска Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="b416c-105">A [schema](schema.md) property definition for a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="b416c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b416c-106">Properties</span></span>

| <span data-ttu-id="b416c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b416c-107">Property</span></span>      | <span data-ttu-id="b416c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b416c-108">Type</span></span>    | <span data-ttu-id="b416c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b416c-109">Description</span></span>                                        |
|:--------------|:--------|:---------------------------------------------------|
| <span data-ttu-id="b416c-110">Queryable</span><span class="sxs-lookup"><span data-stu-id="b416c-110">isQueryable</span></span>   | <span data-ttu-id="b416c-111">Логический</span><span class="sxs-lookup"><span data-stu-id="b416c-111">Boolean</span></span> | <span data-ttu-id="b416c-112">Указывает, является ли свойство подзапросом.</span><span class="sxs-lookup"><span data-stu-id="b416c-112">Specifies if the property is queryable.</span></span> <span data-ttu-id="b416c-113">Запрашиваемые свойства можно использовать в [запросах языка запросов по ключевым словам (KQL)](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span><span class="sxs-lookup"><span data-stu-id="b416c-113">Queryable properties can be used in [Keyword Query Language (KQL) queries](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span></span> <span data-ttu-id="b416c-114">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="b416c-114">Optional.</span></span>  |
| <span data-ttu-id="b416c-115">возможность извлечения</span><span class="sxs-lookup"><span data-stu-id="b416c-115">isRetrievable</span></span> | <span data-ttu-id="b416c-116">Логический</span><span class="sxs-lookup"><span data-stu-id="b416c-116">Boolean</span></span> | <span data-ttu-id="b416c-117">Указывает, может ли свойство быть извлечено.</span><span class="sxs-lookup"><span data-stu-id="b416c-117">Specifies if the property is retrievable.</span></span> <span data-ttu-id="b416c-118">Извлекаемые свойства возвращаются в результирующем наборе при возвращении элементов с помощью API поиска.</span><span class="sxs-lookup"><span data-stu-id="b416c-118">Retrievable properties are returned in the result set when items are returned by the search API.</span></span> <span data-ttu-id="b416c-119">Доступные для извлечения свойства также можно добавить к шаблону отображения, используемому для отображения результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="b416c-119">Retrievable properties are also available to add to the display template used to render search results.</span></span> <span data-ttu-id="b416c-120">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="b416c-120">Optional.</span></span> |
| <span data-ttu-id="b416c-121">с возможностью поиска</span><span class="sxs-lookup"><span data-stu-id="b416c-121">isSearchable</span></span>  | <span data-ttu-id="b416c-122">Логический</span><span class="sxs-lookup"><span data-stu-id="b416c-122">Boolean</span></span> | <span data-ttu-id="b416c-123">Указывает, доступно ли свойство для поиска.</span><span class="sxs-lookup"><span data-stu-id="b416c-123">Specifies if the property is searchable.</span></span> <span data-ttu-id="b416c-124">Только свойства типа `String` или `StringCollection` могут быть доступны для поиска.</span><span class="sxs-lookup"><span data-stu-id="b416c-124">Only properties of type `String` or `StringCollection` can be searchable.</span></span> <span data-ttu-id="b416c-125">Свойства, не включаемые в поиск, не добавляются в индекс поиска.</span><span class="sxs-lookup"><span data-stu-id="b416c-125">Non-searchable properties are not added to the search index.</span></span> <span data-ttu-id="b416c-126">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="b416c-126">Optional.</span></span> |
| <span data-ttu-id="b416c-127">name</span><span class="sxs-lookup"><span data-stu-id="b416c-127">name</span></span>          | <span data-ttu-id="b416c-128">String</span><span class="sxs-lookup"><span data-stu-id="b416c-128">String</span></span>  | <span data-ttu-id="b416c-129">Имя свойства.</span><span class="sxs-lookup"><span data-stu-id="b416c-129">The name of the property.</span></span> <span data-ttu-id="b416c-130">Максимальное число символов 32.</span><span class="sxs-lookup"><span data-stu-id="b416c-130">Maximum 32 characters.</span></span> <span data-ttu-id="b416c-131">Не должно содержать управляющие символы, пробелы или любые из следующих элементов `:`: `;`, `,`, `(`, `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"`,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,, `<` `>` `|` `` ` `` `^`</span><span class="sxs-lookup"><span data-stu-id="b416c-131">Must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="b416c-132">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="b416c-132">Required.</span></span>                |
| <span data-ttu-id="b416c-133">type</span><span class="sxs-lookup"><span data-stu-id="b416c-133">type</span></span>          | <span data-ttu-id="b416c-134">String</span><span class="sxs-lookup"><span data-stu-id="b416c-134">String</span></span>  | <span data-ttu-id="b416c-135">Тип данных указанного свойства.</span><span class="sxs-lookup"><span data-stu-id="b416c-135">The data type of the property.</span></span> <span data-ttu-id="b416c-136">Возможные значения: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `StringCollection`, `Int64Collection`, `DoubleCollection`, `DateTimeCollection`.</span><span class="sxs-lookup"><span data-stu-id="b416c-136">Possible values are: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `StringCollection`, `Int64Collection`, `DoubleCollection`, `DateTimeCollection`.</span></span> <span data-ttu-id="b416c-137">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="b416c-137">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b416c-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b416c-138">JSON representation</span></span>

<span data-ttu-id="b416c-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b416c-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.property",
  "baseType": null
}-->

```json
{
  "isQueryable": true,
  "isRetrievable": true,
  "isSearchable": true,
  "name": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "property resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
