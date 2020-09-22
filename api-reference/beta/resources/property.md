---
title: Тип ресурса свойства
description: Определение свойства схемы для подключения поиска Майкрософт.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ca2f9235a9a3a8f633976f0470326f06c9decf0a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078243"
---
# <a name="property-resource-type"></a><span data-ttu-id="65029-103">Тип ресурса свойства</span><span class="sxs-lookup"><span data-stu-id="65029-103">property resource type</span></span>

<span data-ttu-id="65029-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65029-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65029-105">Определение свойства [схемы](schema.md) для [подключения](externalconnection.md)поиска Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="65029-105">A [schema](schema.md) property definition for a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="properties"></a><span data-ttu-id="65029-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="65029-106">Properties</span></span>

| <span data-ttu-id="65029-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="65029-107">Property</span></span>      | <span data-ttu-id="65029-108">Тип</span><span class="sxs-lookup"><span data-stu-id="65029-108">Type</span></span>              | <span data-ttu-id="65029-109">Описание</span><span class="sxs-lookup"><span data-stu-id="65029-109">Description</span></span>                                        |
|:--------------|:------------------|:---------------------------------------------------|
| <span data-ttu-id="65029-110">псевдоним</span><span class="sxs-lookup"><span data-stu-id="65029-110">aliases</span></span>       | <span data-ttu-id="65029-111">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="65029-111">String collection</span></span> | <span data-ttu-id="65029-112">Набор псевдонимов или понятные имена для свойства.</span><span class="sxs-lookup"><span data-stu-id="65029-112">A set of aliases or a friendly names for the property.</span></span> <span data-ttu-id="65029-113">Максимальное число символов 32.</span><span class="sxs-lookup"><span data-stu-id="65029-113">Maximum 32 characters.</span></span> <span data-ttu-id="65029-114">Каждая строка не должна содержать управляющие символы, пробелы или любые из следующих элементов: `:` ,, `;` `,` ,, `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^` ,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,</span><span class="sxs-lookup"><span data-stu-id="65029-114">Each string must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="65029-115">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="65029-115">Optional.</span></span>  |
| <span data-ttu-id="65029-116">Queryable</span><span class="sxs-lookup"><span data-stu-id="65029-116">isQueryable</span></span>   | <span data-ttu-id="65029-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="65029-117">Boolean</span></span>           | <span data-ttu-id="65029-118">Указывает, является ли свойство подзапросом.</span><span class="sxs-lookup"><span data-stu-id="65029-118">Specifies if the property is queryable.</span></span> <span data-ttu-id="65029-119">Запрашиваемые свойства можно использовать в [запросах языка запросов по ключевым словам (KQL)](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span><span class="sxs-lookup"><span data-stu-id="65029-119">Queryable properties can be used in [Keyword Query Language (KQL) queries](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span></span> <span data-ttu-id="65029-120">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="65029-120">Optional.</span></span>  |
| <span data-ttu-id="65029-121">возможность уточнения</span><span class="sxs-lookup"><span data-stu-id="65029-121">isRefinable</span></span>   | <span data-ttu-id="65029-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="65029-122">Boolean</span></span>           | <span data-ttu-id="65029-123">Указывает, является ли свойство уточнением.</span><span class="sxs-lookup"><span data-stu-id="65029-123">Specifies if the property is refinable.</span></span>  <span data-ttu-id="65029-124">Свойства уточнения можно использовать для фильтрации результатов поиска в [API поиска](search-api-overview.md) и добавления уточнения в пользовательский интерфейс поиска Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="65029-124">Refinable properties can be used to filter search results in the [Search API](search-api-overview.md) and add a refiner control in the Microsoft Search user experience.</span></span> <span data-ttu-id="65029-125">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="65029-125">Optional.</span></span>  |
| <span data-ttu-id="65029-126">возможность извлечения</span><span class="sxs-lookup"><span data-stu-id="65029-126">isRetrievable</span></span> | <span data-ttu-id="65029-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="65029-127">Boolean</span></span>           | <span data-ttu-id="65029-128">Указывает, может ли свойство быть извлечено.</span><span class="sxs-lookup"><span data-stu-id="65029-128">Specifies if the property is retrievable.</span></span> <span data-ttu-id="65029-129">Извлекаемые свойства возвращаются в результирующем наборе при возвращении элементов с помощью API поиска.</span><span class="sxs-lookup"><span data-stu-id="65029-129">Retrievable properties are returned in the result set when items are returned by the search API.</span></span> <span data-ttu-id="65029-130">Доступные для извлечения свойства также можно добавить к шаблону отображения, используемому для отображения результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="65029-130">Retrievable properties are also available to add to the display template used to render search results.</span></span> <span data-ttu-id="65029-131">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="65029-131">Optional.</span></span> |
| <span data-ttu-id="65029-132">с возможностью поиска</span><span class="sxs-lookup"><span data-stu-id="65029-132">isSearchable</span></span>  | <span data-ttu-id="65029-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="65029-133">Boolean</span></span>           | <span data-ttu-id="65029-134">Указывает, доступно ли свойство для поиска.</span><span class="sxs-lookup"><span data-stu-id="65029-134">Specifies if the property is searchable.</span></span> <span data-ttu-id="65029-135">Только свойства типа `String` или `StringCollection` могут быть доступны для поиска.</span><span class="sxs-lookup"><span data-stu-id="65029-135">Only properties of type `String` or `StringCollection` can be searchable.</span></span> <span data-ttu-id="65029-136">Свойства, не включаемые в поиск, не добавляются в индекс поиска.</span><span class="sxs-lookup"><span data-stu-id="65029-136">Non-searchable properties are not added to the search index.</span></span> <span data-ttu-id="65029-137">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="65029-137">Optional.</span></span> |
| <span data-ttu-id="65029-138">Метка</span><span class="sxs-lookup"><span data-stu-id="65029-138">labels</span></span>        | <span data-ttu-id="65029-139">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="65029-139">String collection</span></span> | <span data-ttu-id="65029-140">Указывает один или несколько хорошо известных тегов, добавленных к свойству.</span><span class="sxs-lookup"><span data-stu-id="65029-140">Specifies one or more well-known tags added against a property.</span></span> <span data-ttu-id="65029-141">Метки помогают Microsoft Search распознавать семантику данных в подключении.</span><span class="sxs-lookup"><span data-stu-id="65029-141">Labels help Microsoft Search understand the semantics of the data in the connection.</span></span> <span data-ttu-id="65029-142">Добавление соответствующих меток приведет к расширению возможностей поиска (например, лучшей релевантности).</span><span class="sxs-lookup"><span data-stu-id="65029-142">Adding appropriate labels would result in an enhanced search experience (e.g. better relevance).</span></span> <span data-ttu-id="65029-143">Поддерживаемые Метки:,,,,,, `title` `url` `createdBy` `lastModifiedBy` `authors` `createdDateTime` `lastModifiedDateTime` `fileName` и `fileExtension` .</span><span class="sxs-lookup"><span data-stu-id="65029-143">Supported labels: `title`, `url`, `createdBy`, `lastModifiedBy`, `authors`, `createdDateTime`, `lastModifiedDateTime`, `fileName` and `fileExtension`.</span></span> <span data-ttu-id="65029-144">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="65029-144">Optional.</span></span> |
| <span data-ttu-id="65029-145">name</span><span class="sxs-lookup"><span data-stu-id="65029-145">name</span></span>          | <span data-ttu-id="65029-146">String</span><span class="sxs-lookup"><span data-stu-id="65029-146">String</span></span>            | <span data-ttu-id="65029-147">Имя свойства.</span><span class="sxs-lookup"><span data-stu-id="65029-147">The name of the property.</span></span> <span data-ttu-id="65029-148">Максимальное число символов 32.</span><span class="sxs-lookup"><span data-stu-id="65029-148">Maximum 32 characters.</span></span> <span data-ttu-id="65029-149">Не должно содержать управляющие символы, пробелы или любые из следующих элементов: `:` ,, `;` `,` ,, `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` ,,, `^` ,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,</span><span class="sxs-lookup"><span data-stu-id="65029-149">Must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="65029-150">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="65029-150">Required.</span></span>                |
| <span data-ttu-id="65029-151">type</span><span class="sxs-lookup"><span data-stu-id="65029-151">type</span></span>          | <span data-ttu-id="65029-152">String</span><span class="sxs-lookup"><span data-stu-id="65029-152">String</span></span>            | <span data-ttu-id="65029-153">Тип данных указанного свойства.</span><span class="sxs-lookup"><span data-stu-id="65029-153">The data type of the property.</span></span> <span data-ttu-id="65029-154">Возможные значения: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `StringCollection`, `Int64Collection`, `DoubleCollection`, `DateTimeCollection`.</span><span class="sxs-lookup"><span data-stu-id="65029-154">Possible values are: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `StringCollection`, `Int64Collection`, `DoubleCollection`, `DateTimeCollection`.</span></span> <span data-ttu-id="65029-155">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="65029-155">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="65029-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65029-156">JSON representation</span></span>

<span data-ttu-id="65029-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65029-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.property",
  "baseType": null
}-->

```json
{
  "aliases": [ "String" ],
  "isQueryable": true,
  "isRefinable": true,
  "isRetrievable": true,
  "isSearchable": true,
  "labels": [ "String" ],
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


