---
title: Тип ресурса свойства
description: Определение свойства схемы для подключения поиска Майкрософт.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 465ad0824bf46949476304905bf0fea5c3ff6271
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38703772"
---
# <a name="property-resource-type"></a><span data-ttu-id="b735b-103">Тип ресурса свойства</span><span class="sxs-lookup"><span data-stu-id="b735b-103">property resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b735b-104">Определение свойства [схемы](schema.md) для [подключения](externalconnection.md)поиска Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="b735b-104">A [schema](schema.md) property definition for a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="b735b-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="b735b-105">Properties</span></span>

| <span data-ttu-id="b735b-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="b735b-106">Property</span></span>      | <span data-ttu-id="b735b-107">Тип</span><span class="sxs-lookup"><span data-stu-id="b735b-107">Type</span></span>    | <span data-ttu-id="b735b-108">Описание</span><span class="sxs-lookup"><span data-stu-id="b735b-108">Description</span></span>                                        |
|:--------------|:--------|:---------------------------------------------------|
| <span data-ttu-id="b735b-109">Queryable</span><span class="sxs-lookup"><span data-stu-id="b735b-109">isQueryable</span></span>   | <span data-ttu-id="b735b-110">Логическое</span><span class="sxs-lookup"><span data-stu-id="b735b-110">Boolean</span></span> | <span data-ttu-id="b735b-111">Указывает, является ли свойство подзапросом.</span><span class="sxs-lookup"><span data-stu-id="b735b-111">Specifies if the property is queryable.</span></span> <span data-ttu-id="b735b-112">Запрашиваемые свойства можно использовать в [запросах языка запросов по ключевым словам (KQL)](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span><span class="sxs-lookup"><span data-stu-id="b735b-112">Queryable properties can be used in [Keyword Query Language (KQL) queries](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span></span> <span data-ttu-id="b735b-113">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="b735b-113">Optional.</span></span>  |
| <span data-ttu-id="b735b-114">возможность извлечения</span><span class="sxs-lookup"><span data-stu-id="b735b-114">isRetrievable</span></span> | <span data-ttu-id="b735b-115">Логическое</span><span class="sxs-lookup"><span data-stu-id="b735b-115">Boolean</span></span> | <span data-ttu-id="b735b-116">Указывает, может ли свойство быть извлечено.</span><span class="sxs-lookup"><span data-stu-id="b735b-116">Specifies if the property is retrievable.</span></span> <span data-ttu-id="b735b-117">Извлекаемые свойства возвращаются в результирующем наборе при возвращении элементов с помощью API поиска.</span><span class="sxs-lookup"><span data-stu-id="b735b-117">Retrievable properties are returned in the result set when items are returned by the search API.</span></span> <span data-ttu-id="b735b-118">Доступные для извлечения свойства также можно добавить к шаблону отображения, используемому для отображения результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="b735b-118">Retrievable properties are also available to add to the display template used to render search results.</span></span> <span data-ttu-id="b735b-119">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="b735b-119">Optional.</span></span> |
| <span data-ttu-id="b735b-120">с возможностью поиска</span><span class="sxs-lookup"><span data-stu-id="b735b-120">isSearchable</span></span>  | <span data-ttu-id="b735b-121">Логическое</span><span class="sxs-lookup"><span data-stu-id="b735b-121">Boolean</span></span> | <span data-ttu-id="b735b-122">Указывает, доступно ли свойство для поиска.</span><span class="sxs-lookup"><span data-stu-id="b735b-122">Specifies if the property is searchable.</span></span> <span data-ttu-id="b735b-123">Только свойства типа `String` или `Collection(String)` могут быть доступны для поиска.</span><span class="sxs-lookup"><span data-stu-id="b735b-123">Only properties of type `String` or `Collection(String)` can be searchable.</span></span> <span data-ttu-id="b735b-124">Свойства, не включаемые в поиск, не добавляются в индекс поиска.</span><span class="sxs-lookup"><span data-stu-id="b735b-124">Non-searchable properties are not added to the search index.</span></span> <span data-ttu-id="b735b-125">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="b735b-125">Optional.</span></span> |
| <span data-ttu-id="b735b-126">name</span><span class="sxs-lookup"><span data-stu-id="b735b-126">name</span></span>          | <span data-ttu-id="b735b-127">String</span><span class="sxs-lookup"><span data-stu-id="b735b-127">String</span></span>  | <span data-ttu-id="b735b-128">Имя свойства.</span><span class="sxs-lookup"><span data-stu-id="b735b-128">The name of the property.</span></span> <span data-ttu-id="b735b-129">Максимальное число символов 32.</span><span class="sxs-lookup"><span data-stu-id="b735b-129">Maximum 32 characters.</span></span> <span data-ttu-id="b735b-130">Не должно содержать управляющие символы, пробелы или любые из следующих элементов `:`: `;`, `,`, `(`, `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"`,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,, `<` `>` `|` `` ` `` `^`</span><span class="sxs-lookup"><span data-stu-id="b735b-130">Must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="b735b-131">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="b735b-131">Required.</span></span>                |
| <span data-ttu-id="b735b-132">type</span><span class="sxs-lookup"><span data-stu-id="b735b-132">type</span></span>          | <span data-ttu-id="b735b-133">String</span><span class="sxs-lookup"><span data-stu-id="b735b-133">String</span></span>  | <span data-ttu-id="b735b-134">Тип данных указанного свойства.</span><span class="sxs-lookup"><span data-stu-id="b735b-134">The data type of the property.</span></span> <span data-ttu-id="b735b-135">Возможные значения: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `Collection(String)`, `Collection(Int64)`, `Collection(Double)`, `Collection(DateTime)`.</span><span class="sxs-lookup"><span data-stu-id="b735b-135">Possible values are: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `Collection(String)`, `Collection(Int64)`, `Collection(Double)`, `Collection(DateTime)`.</span></span> <span data-ttu-id="b735b-136">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="b735b-136">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b735b-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b735b-137">JSON representation</span></span>

<span data-ttu-id="b735b-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b735b-138">The following is a JSON representation of the resource.</span></span>

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
