---
title: тип ресурса свойства
description: Определение свойства схемы для Поиск (Майкрософт) подключения.
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 68dfe94d81f4ae5347322ba17c02eb3dab5c15d7
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467852"
---
# <a name="property-resource-type"></a><span data-ttu-id="4a698-103">тип ресурса свойства</span><span class="sxs-lookup"><span data-stu-id="4a698-103">property resource type</span></span>

<span data-ttu-id="4a698-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="4a698-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a698-105">Определение [свойства схемы](externalconnectors-schema.md) для Поиск (Майкрософт) [подключения.](externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="4a698-105">A [schema](externalconnectors-schema.md) property definition for a Microsoft Search [connection](externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4a698-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="4a698-106">Properties</span></span>

| <span data-ttu-id="4a698-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="4a698-107">Property</span></span>      | <span data-ttu-id="4a698-108">Тип</span><span class="sxs-lookup"><span data-stu-id="4a698-108">Type</span></span>              | <span data-ttu-id="4a698-109">Описание</span><span class="sxs-lookup"><span data-stu-id="4a698-109">Description</span></span>                                        |
|:--------------|:------------------|:---------------------------------------------------|
| <span data-ttu-id="4a698-110">псевдонимы</span><span class="sxs-lookup"><span data-stu-id="4a698-110">aliases</span></span>       | <span data-ttu-id="4a698-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4a698-111">String collection</span></span> | <span data-ttu-id="4a698-112">Набор псевдонимов или дружественных имен для свойства.</span><span class="sxs-lookup"><span data-stu-id="4a698-112">A set of aliases or a friendly names for the property.</span></span> <span data-ttu-id="4a698-113">Максимум 32 символа.</span><span class="sxs-lookup"><span data-stu-id="4a698-113">Maximum 32 characters.</span></span> <span data-ttu-id="4a698-114">Каждая строка не должна содержать символов управления, whitespace или любого из следующих: , . `:` `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^`</span><span class="sxs-lookup"><span data-stu-id="4a698-114">Each string must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="4a698-115">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="4a698-115">Optional.</span></span>  |
| <span data-ttu-id="4a698-116">isQueryable</span><span class="sxs-lookup"><span data-stu-id="4a698-116">isQueryable</span></span>   | <span data-ttu-id="4a698-117">boolean</span><span class="sxs-lookup"><span data-stu-id="4a698-117">boolean</span></span>           | <span data-ttu-id="4a698-118">Указывает, запрашивается ли свойство.</span><span class="sxs-lookup"><span data-stu-id="4a698-118">Specifies if the property is queryable.</span></span> <span data-ttu-id="4a698-119">Запрашиваемые свойства можно использовать в запросах На языке запросов ключевых слов [(KQL).](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)</span><span class="sxs-lookup"><span data-stu-id="4a698-119">Queryable properties can be used in [Keyword Query Language (KQL) queries](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span></span> <span data-ttu-id="4a698-120">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="4a698-120">Optional.</span></span>  |
| <span data-ttu-id="4a698-121">isRefinable</span><span class="sxs-lookup"><span data-stu-id="4a698-121">isRefinable</span></span>   | <span data-ttu-id="4a698-122">boolean</span><span class="sxs-lookup"><span data-stu-id="4a698-122">boolean</span></span>           | <span data-ttu-id="4a698-123">Указывает, является ли свойство уточненным.</span><span class="sxs-lookup"><span data-stu-id="4a698-123">Specifies if the property is refinable.</span></span>  <span data-ttu-id="4a698-124">Уточненные свойства можно использовать для фильтрации результатов поиска в [API](search-api-overview.md) поиска и добавления управления Поиск (Майкрософт) пользователей.</span><span class="sxs-lookup"><span data-stu-id="4a698-124">Refinable properties can be used to filter search results in the [Search API](search-api-overview.md) and add a refiner control in the Microsoft Search user experience.</span></span> <span data-ttu-id="4a698-125">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="4a698-125">Optional.</span></span>  |
| <span data-ttu-id="4a698-126">isRetrievable</span><span class="sxs-lookup"><span data-stu-id="4a698-126">isRetrievable</span></span> | <span data-ttu-id="4a698-127">boolean</span><span class="sxs-lookup"><span data-stu-id="4a698-127">boolean</span></span>           | <span data-ttu-id="4a698-128">Указывает, является ли свойство искомым.</span><span class="sxs-lookup"><span data-stu-id="4a698-128">Specifies if the property is retrievable.</span></span> <span data-ttu-id="4a698-129">Возвращаемые свойства возвращаются в наборе результатов, когда элементы возвращаются API поиска.</span><span class="sxs-lookup"><span data-stu-id="4a698-129">Retrievable properties are returned in the result set when items are returned by the search API.</span></span> <span data-ttu-id="4a698-130">Свойства, которые можно получить, также доступны для добавления в шаблон отображения, используемый для отрисовки результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="4a698-130">Retrievable properties are also available to add to the display template used to render search results.</span></span> <span data-ttu-id="4a698-131">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="4a698-131">Optional.</span></span> |
| <span data-ttu-id="4a698-132">isSearchable</span><span class="sxs-lookup"><span data-stu-id="4a698-132">isSearchable</span></span>  | <span data-ttu-id="4a698-133">boolean</span><span class="sxs-lookup"><span data-stu-id="4a698-133">boolean</span></span>           | <span data-ttu-id="4a698-134">Указывает, можно ли найти свойство.</span><span class="sxs-lookup"><span data-stu-id="4a698-134">Specifies if the property is searchable.</span></span> <span data-ttu-id="4a698-135">Только свойства типа `string` или `stringCollection` можно искать.</span><span class="sxs-lookup"><span data-stu-id="4a698-135">Only properties of type `string` or `stringCollection` can be searchable.</span></span> <span data-ttu-id="4a698-136">Невыявимые свойства не добавляются в индекс поиска.</span><span class="sxs-lookup"><span data-stu-id="4a698-136">Non-searchable properties are not added to the search index.</span></span> <span data-ttu-id="4a698-137">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="4a698-137">Optional.</span></span> |
| <span data-ttu-id="4a698-138">метки</span><span class="sxs-lookup"><span data-stu-id="4a698-138">labels</span></span>        | <span data-ttu-id="4a698-139">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4a698-139">String collection</span></span> | <span data-ttu-id="4a698-140">Указывает один или несколько известных тегов, добавленных к свойству.</span><span class="sxs-lookup"><span data-stu-id="4a698-140">Specifies one or more well-known tags added against a property.</span></span> <span data-ttu-id="4a698-141">Метки помогают Поиск (Майкрософт) понять семантику данных в подключении.</span><span class="sxs-lookup"><span data-stu-id="4a698-141">Labels help Microsoft Search understand the semantics of the data in the connection.</span></span> <span data-ttu-id="4a698-142">Добавление соответствующих меток приведет к усилению поиска (например, повышению релевантности).</span><span class="sxs-lookup"><span data-stu-id="4a698-142">Adding appropriate labels would result in an enhanced search experience (e.g. better relevance).</span></span> <span data-ttu-id="4a698-143">Поддерживаемые метки: , , , , , , , , и `title` `url` `createdBy` `lastModifiedBy` `authors` `createdDateTime` `lastModifiedDateTime` `fileName` `fileExtension` `iconUrl` `containerName` `containerUrl` .</span><span class="sxs-lookup"><span data-stu-id="4a698-143">Supported labels: `title`, `url`, `createdBy`, `lastModifiedBy`, `authors`, `createdDateTime`, `lastModifiedDateTime`, `fileName`, `fileExtension`, `iconUrl`, `containerName`, and `containerUrl`.</span></span> <span data-ttu-id="4a698-144">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="4a698-144">Optional.</span></span> |
| <span data-ttu-id="4a698-145">name</span><span class="sxs-lookup"><span data-stu-id="4a698-145">name</span></span>          | <span data-ttu-id="4a698-146">String</span><span class="sxs-lookup"><span data-stu-id="4a698-146">String</span></span>            | <span data-ttu-id="4a698-147">Имя свойства.</span><span class="sxs-lookup"><span data-stu-id="4a698-147">The name of the property.</span></span> <span data-ttu-id="4a698-148">Максимум 32 символа.</span><span class="sxs-lookup"><span data-stu-id="4a698-148">Maximum 32 characters.</span></span> <span data-ttu-id="4a698-149">Не должен содержать символы управления, whitespace или любой из следующих: , . `:` `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^`</span><span class="sxs-lookup"><span data-stu-id="4a698-149">Must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="4a698-150">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="4a698-150">Required.</span></span>                |
| <span data-ttu-id="4a698-151">type</span><span class="sxs-lookup"><span data-stu-id="4a698-151">type</span></span>          | <span data-ttu-id="4a698-152">String</span><span class="sxs-lookup"><span data-stu-id="4a698-152">String</span></span>            | <span data-ttu-id="4a698-153">Тип данных указанного свойства.</span><span class="sxs-lookup"><span data-stu-id="4a698-153">The data type of the property.</span></span> <span data-ttu-id="4a698-154">Возможные значения: `string`, `int64`, `double`, `dateTime`, `boolean`, `stringCollection`, `int64Collection`, `doubleCollection`, `dateTimeCollection`.</span><span class="sxs-lookup"><span data-stu-id="4a698-154">Possible values are: `string`, `int64`, `double`, `dateTime`, `boolean`, `stringCollection`, `int64Collection`, `doubleCollection`, `dateTimeCollection`.</span></span> <span data-ttu-id="4a698-155">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="4a698-155">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4a698-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4a698-156">JSON representation</span></span>

<span data-ttu-id="4a698-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4a698-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.property",
  "baseType": null
}-->

```json
{
  "aliases": [ "String" ],
  "isQueryable": true,
  "isRefinable": true,
  "isRetrievable": true,
  "isSearchable": true,
  "labels": [ "string" ],
  "name": "string",
  "type": "string"
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
