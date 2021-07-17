---
title: тип ресурса свойства
description: Определение свойства схемы для Поиск (Майкрософт) подключения.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 6159126581d2a95cc45596a29cddff8642c5838f
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467450"
---
# <a name="property-resource-type"></a><span data-ttu-id="34d92-103">тип ресурса свойства</span><span class="sxs-lookup"><span data-stu-id="34d92-103">property resource type</span></span>

<span data-ttu-id="34d92-104">Пространство имен: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="34d92-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="34d92-105">Определение [свойства схемы](externalconnectors-schema.md) для Поиск (Майкрософт) [подключения.](externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="34d92-105">A [schema](externalconnectors-schema.md) property definition for a Microsoft Search [connection](externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="34d92-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="34d92-106">Properties</span></span>
|<span data-ttu-id="34d92-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="34d92-107">Property</span></span>|<span data-ttu-id="34d92-108">Тип</span><span class="sxs-lookup"><span data-stu-id="34d92-108">Type</span></span>|<span data-ttu-id="34d92-109">Описание</span><span class="sxs-lookup"><span data-stu-id="34d92-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34d92-110">псевдонимы</span><span class="sxs-lookup"><span data-stu-id="34d92-110">aliases</span></span>|<span data-ttu-id="34d92-111">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="34d92-111">String collection</span></span>|<span data-ttu-id="34d92-112">Набор псевдонимов или дружественных имен для свойства.</span><span class="sxs-lookup"><span data-stu-id="34d92-112">A set of aliases or a friendly names for the property.</span></span> <span data-ttu-id="34d92-113">Максимум 32 символа.</span><span class="sxs-lookup"><span data-stu-id="34d92-113">Maximum 32 characters.</span></span> <span data-ttu-id="34d92-114">Каждая строка не должна содержать символов управления, whitespace или любого из следующих: , . `:` `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^`</span><span class="sxs-lookup"><span data-stu-id="34d92-114">Each string must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="34d92-115">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="34d92-115">Optional.</span></span>|
|<span data-ttu-id="34d92-116">isQueryable</span><span class="sxs-lookup"><span data-stu-id="34d92-116">isQueryable</span></span>|<span data-ttu-id="34d92-117">Логический</span><span class="sxs-lookup"><span data-stu-id="34d92-117">Boolean</span></span>|<span data-ttu-id="34d92-118">Указывает, запрашивается ли свойство.</span><span class="sxs-lookup"><span data-stu-id="34d92-118">Specifies if the property is queryable.</span></span> <span data-ttu-id="34d92-119">Запрашиваемые свойства можно использовать в запросах На языке запросов ключевых слов [(KQL).](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference)</span><span class="sxs-lookup"><span data-stu-id="34d92-119">Queryable properties can be used in [Keyword Query Language (KQL) queries](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span></span> <span data-ttu-id="34d92-120">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="34d92-120">Optional.</span></span>|
|<span data-ttu-id="34d92-121">isRefinable</span><span class="sxs-lookup"><span data-stu-id="34d92-121">isRefinable</span></span>|<span data-ttu-id="34d92-122">Логический</span><span class="sxs-lookup"><span data-stu-id="34d92-122">Boolean</span></span>|<span data-ttu-id="34d92-123">Указывает, является ли свойство уточненным.</span><span class="sxs-lookup"><span data-stu-id="34d92-123">Specifies if the property is refinable.</span></span>  <span data-ttu-id="34d92-124">Уточненные свойства можно использовать для фильтрации результатов поиска в [API](search-api-overview.md) поиска и добавления управления Поиск (Майкрософт) пользователей.</span><span class="sxs-lookup"><span data-stu-id="34d92-124">Refinable properties can be used to filter search results in the [Search API](search-api-overview.md) and add a refiner control in the Microsoft Search user experience.</span></span> <span data-ttu-id="34d92-125">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="34d92-125">Optional.</span></span>|
|<span data-ttu-id="34d92-126">isRetrievable</span><span class="sxs-lookup"><span data-stu-id="34d92-126">isRetrievable</span></span>|<span data-ttu-id="34d92-127">Логический</span><span class="sxs-lookup"><span data-stu-id="34d92-127">Boolean</span></span>|<span data-ttu-id="34d92-128">Указывает, является ли свойство искомым.</span><span class="sxs-lookup"><span data-stu-id="34d92-128">Specifies if the property is retrievable.</span></span> <span data-ttu-id="34d92-129">Возвращаемые свойства возвращаются в наборе результатов, когда элементы возвращаются API поиска.</span><span class="sxs-lookup"><span data-stu-id="34d92-129">Retrievable properties are returned in the result set when items are returned by the search API.</span></span> <span data-ttu-id="34d92-130">Свойства, которые можно получить, также доступны для добавления в шаблон отображения, используемый для отрисовки результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="34d92-130">Retrievable properties are also available to add to the display template used to render search results.</span></span> <span data-ttu-id="34d92-131">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="34d92-131">Optional.</span></span>|
|<span data-ttu-id="34d92-132">isSearchable</span><span class="sxs-lookup"><span data-stu-id="34d92-132">isSearchable</span></span>|<span data-ttu-id="34d92-133">Логический</span><span class="sxs-lookup"><span data-stu-id="34d92-133">Boolean</span></span>|<span data-ttu-id="34d92-134">Указывает, можно ли найти свойство.</span><span class="sxs-lookup"><span data-stu-id="34d92-134">Specifies if the property is searchable.</span></span> <span data-ttu-id="34d92-135">Только свойства типа `String` или `StringCollection` можно искать.</span><span class="sxs-lookup"><span data-stu-id="34d92-135">Only properties of type `String` or `StringCollection` can be searchable.</span></span> <span data-ttu-id="34d92-136">Невыявимые свойства не добавляются в индекс поиска.</span><span class="sxs-lookup"><span data-stu-id="34d92-136">Non-searchable properties are not added to the search index.</span></span> <span data-ttu-id="34d92-137">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="34d92-137">Optional.</span></span>|
|<span data-ttu-id="34d92-138">метки</span><span class="sxs-lookup"><span data-stu-id="34d92-138">labels</span></span>|<span data-ttu-id="34d92-139">коллекция microsoft.graph.externalConnectors.label</span><span class="sxs-lookup"><span data-stu-id="34d92-139">microsoft.graph.externalConnectors.label collection</span></span>|<span data-ttu-id="34d92-140">Указывает один или несколько известных тегов, добавленных к свойству.</span><span class="sxs-lookup"><span data-stu-id="34d92-140">Specifies one or more well-known tags added against a property.</span></span> <span data-ttu-id="34d92-141">Метки помогают Поиск (Майкрософт) понять семантику данных в подключении.</span><span class="sxs-lookup"><span data-stu-id="34d92-141">Labels help Microsoft Search understand the semantics of the data in the connection.</span></span> <span data-ttu-id="34d92-142">Добавление соответствующих меток приведет к усилению поиска (например, повышению релевантности).</span><span class="sxs-lookup"><span data-stu-id="34d92-142">Adding appropriate labels would result in an enhanced search experience (e.g. better relevance).</span></span> <span data-ttu-id="34d92-143">Поддерживаемые метки: `title` , , , , , , и `url` `createdBy` `lastModifiedBy` `authors` `createdDateTime` `lastModifiedDateTime` `fileName` `fileExtension` .</span><span class="sxs-lookup"><span data-stu-id="34d92-143">Supported labels: `title`, `url`, `createdBy`, `lastModifiedBy`, `authors`, `createdDateTime`, `lastModifiedDateTime`, `fileName` and `fileExtension`.</span></span> <span data-ttu-id="34d92-144">Необязательное.</span><span class="sxs-lookup"><span data-stu-id="34d92-144">Optional.</span></span>|
|<span data-ttu-id="34d92-145">name</span><span class="sxs-lookup"><span data-stu-id="34d92-145">name</span></span>|<span data-ttu-id="34d92-146">String</span><span class="sxs-lookup"><span data-stu-id="34d92-146">String</span></span>|<span data-ttu-id="34d92-147">Имя свойства.</span><span class="sxs-lookup"><span data-stu-id="34d92-147">The name of the property.</span></span> <span data-ttu-id="34d92-148">Максимум 32 символа.</span><span class="sxs-lookup"><span data-stu-id="34d92-148">Maximum 32 characters.</span></span> <span data-ttu-id="34d92-149">Не должен содержать символы управления, whitespace или любой из следующих: , . `:` `;` `,` `(` `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=` `&` `?` `@` `#` `\` `~` `'` `"` `<` `>` `|` `` ` `` `^`</span><span class="sxs-lookup"><span data-stu-id="34d92-149">Must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="34d92-150">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="34d92-150">Required.</span></span>|
|<span data-ttu-id="34d92-151">type</span><span class="sxs-lookup"><span data-stu-id="34d92-151">type</span></span>|<span data-ttu-id="34d92-152">microsoft.graph.externalConnectors.propertyType</span><span class="sxs-lookup"><span data-stu-id="34d92-152">microsoft.graph.externalConnectors.propertyType</span></span>|<span data-ttu-id="34d92-153">Тип данных указанного свойства.</span><span class="sxs-lookup"><span data-stu-id="34d92-153">The data type of the property.</span></span> <span data-ttu-id="34d92-154">Возможные значения: `string`, `int64`, `double`, `dateTime`, `boolean`, `stringCollection`, `int64Collection`, `doubleCollection`, `dateTimeCollection`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="34d92-154">Possible values are: `string`, `int64`, `double`, `dateTime`, `boolean`, `stringCollection`, `int64Collection`, `doubleCollection`, `dateTimeCollection`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34d92-155">Связи</span><span class="sxs-lookup"><span data-stu-id="34d92-155">Relationships</span></span>
<span data-ttu-id="34d92-156">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="34d92-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="34d92-157">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="34d92-157">JSON representation</span></span>
<span data-ttu-id="34d92-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34d92-158">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.property"
}
-->
``` json
{
  "name": "String",
  "type": "String",
  "isSearchable": "Boolean",
  "isRetrievable": "Boolean",
  "isQueryable": "Boolean",
  "isRefinable": "Boolean",
  "aliases": [
    "String"
  ],
  "labels": [
    "String"
  ]
}
```

