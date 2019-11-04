---
title: Тип ресурса свойства
description: Определение свойства схемы для подключения поиска Майкрософт.
localization_priority: Normal
author: snlraju-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: df535b89d238f31185ff187b207671337d05fd75
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939090"
---
# <a name="property-resource-type"></a><span data-ttu-id="2d9f0-103">Тип ресурса свойства</span><span class="sxs-lookup"><span data-stu-id="2d9f0-103">property resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d9f0-104">Определение свойства [схемы](schema.md) для [подключения](externalconnection.md)поиска Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="2d9f0-104">A [schema](schema.md) property definition for a Microsoft Search [connection](externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2d9f0-105">Свойства</span><span class="sxs-lookup"><span data-stu-id="2d9f0-105">Properties</span></span>

| <span data-ttu-id="2d9f0-106">Свойство</span><span class="sxs-lookup"><span data-stu-id="2d9f0-106">Property</span></span>      | <span data-ttu-id="2d9f0-107">Тип</span><span class="sxs-lookup"><span data-stu-id="2d9f0-107">Type</span></span>    | <span data-ttu-id="2d9f0-108">Описание</span><span class="sxs-lookup"><span data-stu-id="2d9f0-108">Description</span></span>                                        |
|:--------------|:--------|:---------------------------------------------------|
| <span data-ttu-id="2d9f0-109">Queryable</span><span class="sxs-lookup"><span data-stu-id="2d9f0-109">isQueryable</span></span>   | <span data-ttu-id="2d9f0-110">Логический</span><span class="sxs-lookup"><span data-stu-id="2d9f0-110">Boolean</span></span> | <span data-ttu-id="2d9f0-111">Указывает, является ли свойство подзапросом.</span><span class="sxs-lookup"><span data-stu-id="2d9f0-111">Specifies if the property is queryable.</span></span> <span data-ttu-id="2d9f0-112">Запрашиваемые свойства можно использовать в [запросах языка запросов по ключевым словам (KQL)](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span><span class="sxs-lookup"><span data-stu-id="2d9f0-112">Queryable properties can be used in [Keyword Query Language (KQL) queries](/sharepoint/dev/general-development/keyword-query-language-kql-syntax-reference).</span></span> <span data-ttu-id="2d9f0-113">Необязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="2d9f0-113">Optional.</span></span>  |
| <span data-ttu-id="2d9f0-114">возможность извлечения</span><span class="sxs-lookup"><span data-stu-id="2d9f0-114">isRetrievable</span></span> | <span data-ttu-id="2d9f0-115">Логический</span><span class="sxs-lookup"><span data-stu-id="2d9f0-115">Boolean</span></span> | <span data-ttu-id="2d9f0-116">Указывает, может ли свойство быть извлечено.</span><span class="sxs-lookup"><span data-stu-id="2d9f0-116">Specifies if the property is retrievable.</span></span> <span data-ttu-id="2d9f0-117">Извлекаемые свойства возвращаются в результирующем наборе при возвращении элементов с помощью API поиска.</span><span class="sxs-lookup"><span data-stu-id="2d9f0-117">Retrievable properties are returned in the result set when items are returned by the search API.</span></span> <span data-ttu-id="2d9f0-118">Доступные для извлечения свойства также можно добавить к шаблону отображения, используемому для отображения результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="2d9f0-118">Retrievable properties are also available to add to the display template used to render search results.</span></span> <span data-ttu-id="2d9f0-119">Необязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="2d9f0-119">Optional.</span></span> |
| <span data-ttu-id="2d9f0-120">с возможностью поиска</span><span class="sxs-lookup"><span data-stu-id="2d9f0-120">isSearchable</span></span>  | <span data-ttu-id="2d9f0-121">Логический</span><span class="sxs-lookup"><span data-stu-id="2d9f0-121">Boolean</span></span> | <span data-ttu-id="2d9f0-122">Указывает, доступно ли свойство для поиска.</span><span class="sxs-lookup"><span data-stu-id="2d9f0-122">Specifies if the property is searchable.</span></span> <span data-ttu-id="2d9f0-123">Только свойства типа `String` или `Collection(String)` могут быть доступны для поиска.</span><span class="sxs-lookup"><span data-stu-id="2d9f0-123">Only properties of type `String` or `Collection(String)` can be searchable.</span></span> <span data-ttu-id="2d9f0-124">Свойства, не включаемые в поиск, не добавляются в индекс поиска.</span><span class="sxs-lookup"><span data-stu-id="2d9f0-124">Non-searchable properties are not added to the search index.</span></span> <span data-ttu-id="2d9f0-125">Необязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="2d9f0-125">Optional.</span></span> |
| <span data-ttu-id="2d9f0-126">name</span><span class="sxs-lookup"><span data-stu-id="2d9f0-126">name</span></span>          | <span data-ttu-id="2d9f0-127">String</span><span class="sxs-lookup"><span data-stu-id="2d9f0-127">String</span></span>  | <span data-ttu-id="2d9f0-128">Имя свойства.</span><span class="sxs-lookup"><span data-stu-id="2d9f0-128">The name of the property.</span></span> <span data-ttu-id="2d9f0-129">Максимальное число символов 32.</span><span class="sxs-lookup"><span data-stu-id="2d9f0-129">Maximum 32 characters.</span></span> <span data-ttu-id="2d9f0-130">Не должно содержать управляющие символы, пробелы или любые из следующих элементов `:`: `;`, `,`, `(`, `)` `[` `]` `{` `}` `%` `$` `+` `!` `*` `=`,,,,,,,,,,, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span><span class="sxs-lookup"><span data-stu-id="2d9f0-130">Must not contain control characters, whitespace, or any of the following: `:`, `;`, `,`, `(`, `)`, `[`, `]`, `{`, `}`, `%`, `$`, `+`, `!`, `*`, `=`, `&`, `?`, `@`, `#`, `\`, `~`, `'`, `"`, `<`, `>`, `|`, `` ` ``, `^`.</span></span> <span data-ttu-id="2d9f0-131">Обязательное.</span><span class="sxs-lookup"><span data-stu-id="2d9f0-131">Required.</span></span>                |
| <span data-ttu-id="2d9f0-132">type</span><span class="sxs-lookup"><span data-stu-id="2d9f0-132">type</span></span>          | <span data-ttu-id="2d9f0-133">String</span><span class="sxs-lookup"><span data-stu-id="2d9f0-133">String</span></span>  | <span data-ttu-id="2d9f0-134">Тип данных указанного свойства.</span><span class="sxs-lookup"><span data-stu-id="2d9f0-134">The data type of the property.</span></span> <span data-ttu-id="2d9f0-135">Возможные значения: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `Collection(String)`, `Collection(Int64)`, `Collection(Double)`, `Collection(DateTime)`.</span><span class="sxs-lookup"><span data-stu-id="2d9f0-135">Possible values are: `String`, `Int64`, `Double`, `DateTime`, `Boolean`, `Collection(String)`, `Collection(Int64)`, `Collection(Double)`, `Collection(DateTime)`.</span></span> <span data-ttu-id="2d9f0-136">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="2d9f0-136">Required.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2d9f0-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2d9f0-137">JSON representation</span></span>

<span data-ttu-id="2d9f0-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2d9f0-138">The following is a JSON representation of the resource.</span></span>

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
