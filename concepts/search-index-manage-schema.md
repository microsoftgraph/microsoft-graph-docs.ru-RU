---
title: Схема регистрации для связей Microsoft Graph
description: Узнайте, как с помощью Microsoft Graph зарегистрировать схему для связей Microsoft Graph
localization_priority: Priority
author: rsamai
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: 0e70f712b7965e97df7255cda3dcf94c69f73691
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193775"
---
# <a name="register-schema-for-the-microsoft-graph-connection"></a><span data-ttu-id="b1006-103">Схема регистрации для связей Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b1006-103">Register schema for the Microsoft Graph connection</span></span>

<span data-ttu-id="b1006-104">[Схема](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true) связей определяет, как ваше содержимое будет использоваться в различных интерфейсах Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b1006-104">The connection [schema](/graph/api/resources/schema?view=graph-rest-beta&preserve-view=true) determines how your content will be used in various Microsoft Graph experiences.</span></span> <span data-ttu-id="b1006-105">Схема — это плоский список всех свойств, которые вы планируете добавить в связь, а также их атрибуты, метки и псевдонимы.</span><span class="sxs-lookup"><span data-stu-id="b1006-105">Schema is a flat list of all the properties that you plan to add to the connection along with their attributes, labels, and aliases.</span></span> <span data-ttu-id="b1006-106">Перед добавлением элементов в связь вы должны зарегистрировать схему.</span><span class="sxs-lookup"><span data-stu-id="b1006-106">You must register the schema before adding items into the connection.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="example-schema"></a><span data-ttu-id="b1006-107">Пример схемы</span><span class="sxs-lookup"><span data-stu-id="b1006-107">Example schema</span></span>

<span data-ttu-id="b1006-108">В таблице ниже приведен пример возможной схемы для соединителя системы рабочих запросов.</span><span class="sxs-lookup"><span data-stu-id="b1006-108">The following table represents an example of a possible schema for a work ticket system connector.</span></span>

| <span data-ttu-id="b1006-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1006-109">Property</span></span>       | <span data-ttu-id="b1006-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b1006-110">Type</span></span>             | <span data-ttu-id="b1006-111">Возможность поиска</span><span class="sxs-lookup"><span data-stu-id="b1006-111">Searchable</span></span>         | <span data-ttu-id="b1006-112">Возможность запроса</span><span class="sxs-lookup"><span data-stu-id="b1006-112">Queryable</span></span>          | <span data-ttu-id="b1006-113">Возможность извлечения</span><span class="sxs-lookup"><span data-stu-id="b1006-113">Retrievable</span></span>        | <span data-ttu-id="b1006-114">Возможность уточнения</span><span class="sxs-lookup"><span data-stu-id="b1006-114">Refinable</span></span>          | <span data-ttu-id="b1006-115">Метки</span><span class="sxs-lookup"><span data-stu-id="b1006-115">Labels</span></span>               | <span data-ttu-id="b1006-116">Псевдонимы</span><span class="sxs-lookup"><span data-stu-id="b1006-116">Aliases</span></span>    |
|----------------|------------------|--------------------|--------------------|--------------------|--------------------|----------------------|------------|
| <span data-ttu-id="b1006-117">ticketId</span><span class="sxs-lookup"><span data-stu-id="b1006-117">ticketId</span></span>       | <span data-ttu-id="b1006-118">String</span><span class="sxs-lookup"><span data-stu-id="b1006-118">String</span></span>           |                    |                    |                    |                    |                      | <span data-ttu-id="b1006-119">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="b1006-119">ID</span></span>         |
| <span data-ttu-id="b1006-120">title</span><span class="sxs-lookup"><span data-stu-id="b1006-120">title</span></span>          | <span data-ttu-id="b1006-121">String</span><span class="sxs-lookup"><span data-stu-id="b1006-121">String</span></span>           | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |                    | <span data-ttu-id="b1006-125">title</span><span class="sxs-lookup"><span data-stu-id="b1006-125">title</span></span>                |            |
| <span data-ttu-id="b1006-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="b1006-126">createdBy</span></span>      | <span data-ttu-id="b1006-127">String</span><span class="sxs-lookup"><span data-stu-id="b1006-127">String</span></span>           | :heavy_check_mark: | :heavy_check_mark: |                    |                    | <span data-ttu-id="b1006-130">createdBy</span><span class="sxs-lookup"><span data-stu-id="b1006-130">createdBy</span></span>            | <span data-ttu-id="b1006-131">creator</span><span class="sxs-lookup"><span data-stu-id="b1006-131">creator</span></span>    |
| <span data-ttu-id="b1006-132">assignedTo</span><span class="sxs-lookup"><span data-stu-id="b1006-132">assignedTo</span></span>     | <span data-ttu-id="b1006-133">String</span><span class="sxs-lookup"><span data-stu-id="b1006-133">String</span></span>           | :heavy_check_mark: | :heavy_check_mark: |                    |                    |                      |            |
| <span data-ttu-id="b1006-136">lastEditedDate</span><span class="sxs-lookup"><span data-stu-id="b1006-136">lastEditedDate</span></span> | <span data-ttu-id="b1006-137">DateTime</span><span class="sxs-lookup"><span data-stu-id="b1006-137">DateTime</span></span>         |                    | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | <span data-ttu-id="b1006-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1006-141">lastModifiedDateTime</span></span> | <span data-ttu-id="b1006-142">editedDate</span><span class="sxs-lookup"><span data-stu-id="b1006-142">editedDate</span></span> |
| <span data-ttu-id="b1006-143">lastEditedBy</span><span class="sxs-lookup"><span data-stu-id="b1006-143">lastEditedBy</span></span>   | <span data-ttu-id="b1006-144">String</span><span class="sxs-lookup"><span data-stu-id="b1006-144">String</span></span>           | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |                    | <span data-ttu-id="b1006-148">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b1006-148">lastModifiedBy</span></span>       | <span data-ttu-id="b1006-149">edited</span><span class="sxs-lookup"><span data-stu-id="b1006-149">edited</span></span>     |
| <span data-ttu-id="b1006-150">workItemType</span><span class="sxs-lookup"><span data-stu-id="b1006-150">workItemType</span></span>   | <span data-ttu-id="b1006-151">String</span><span class="sxs-lookup"><span data-stu-id="b1006-151">String</span></span>           |                    | :heavy_check_mark: | :heavy_check_mark: |                    |                      | <span data-ttu-id="b1006-154">ticketType</span><span class="sxs-lookup"><span data-stu-id="b1006-154">ticketType</span></span> |
| <span data-ttu-id="b1006-155">priority</span><span class="sxs-lookup"><span data-stu-id="b1006-155">priority</span></span>       | <span data-ttu-id="b1006-156">Int64</span><span class="sxs-lookup"><span data-stu-id="b1006-156">Int64</span></span>            | :heavy_check_mark: |                    |                    |                    |                      |            |
| <span data-ttu-id="b1006-158">tags</span><span class="sxs-lookup"><span data-stu-id="b1006-158">tags</span></span>           | <span data-ttu-id="b1006-159">StringCollection</span><span class="sxs-lookup"><span data-stu-id="b1006-159">StringCollection</span></span> |                    | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |                      |            |
| <span data-ttu-id="b1006-163">status</span><span class="sxs-lookup"><span data-stu-id="b1006-163">status</span></span>         | <span data-ttu-id="b1006-164">String</span><span class="sxs-lookup"><span data-stu-id="b1006-164">String</span></span>           |                    | :heavy_check_mark: | :heavy_check_mark: |                    |                      |            |
| <span data-ttu-id="b1006-167">url</span><span class="sxs-lookup"><span data-stu-id="b1006-167">url</span></span>            | <span data-ttu-id="b1006-168">String</span><span class="sxs-lookup"><span data-stu-id="b1006-168">String</span></span>           |                    |                    |                    |                    | <span data-ttu-id="b1006-169">url</span><span class="sxs-lookup"><span data-stu-id="b1006-169">url</span></span>                  |            |
| <span data-ttu-id="b1006-170">resolved</span><span class="sxs-lookup"><span data-stu-id="b1006-170">resolved</span></span>       | <span data-ttu-id="b1006-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1006-171">Boolean</span></span>          |                    | :heavy_check_mark: | :heavy_check_mark: |                    |                      |            |

## <a name="property-attributes"></a><span data-ttu-id="b1006-174">Атрибуты свойства</span><span class="sxs-lookup"><span data-stu-id="b1006-174">Property attributes</span></span>

### <a name="searchable"></a><span data-ttu-id="b1006-175">Возможность поиска</span><span class="sxs-lookup"><span data-stu-id="b1006-175">Searchable</span></span>

<span data-ttu-id="b1006-176">Если свойство доступно для поиска, его значение добавляется в полнотекстовый индекс.</span><span class="sxs-lookup"><span data-stu-id="b1006-176">If a property is searchable, its value is added to the full text index.</span></span> <span data-ttu-id="b1006-177">Когда пользователь выполняет поиск, результаты возвращаются в том случае, если поисковый запрос совпадает с одним из полей, доступных для поиска, или его [контентом](search-index-manage-items.md#content).</span><span class="sxs-lookup"><span data-stu-id="b1006-177">When a user performs a search, we return results if there is a search hit in one of the searchable fields or its [content](search-index-manage-items.md#content).</span></span>

<!-- markdownlint-disable MD036 -->
<span data-ttu-id="b1006-178">![Поиск по запросу "design" с отображением результатов, совпадающих со свойствами и контентом](./images/search-index-manage-items-schema-1.svg)</span><span class="sxs-lookup"><span data-stu-id="b1006-178">![A search for "design" displaying results for hits against properties and content](./images/search-index-manage-items-schema-1.svg)</span></span>

<span data-ttu-id="b1006-179">*Поиск по запросу "design" с отображением результатов, совпадающих со свойствами (`title`, `tags`) и контентом*</span><span class="sxs-lookup"><span data-stu-id="b1006-179">*A search for "design" displaying results for hits against properties (`title`, `tags`) and content*</span></span>

### <a name="queryable"></a><span data-ttu-id="b1006-180">Возможность запроса</span><span class="sxs-lookup"><span data-stu-id="b1006-180">Queryable</span></span>

<span data-ttu-id="b1006-181">Если свойство поддерживает запросы, вы можете запрашивать его с помощью языка KQL.</span><span class="sxs-lookup"><span data-stu-id="b1006-181">If a property is queryable, you can query against it using knowledge query language (KQL).</span></span> <span data-ttu-id="b1006-182">KQL содержит один или несколько ключевых слов в свободной текстовой форме (слова или фразы) или ограничения свойств.</span><span class="sxs-lookup"><span data-stu-id="b1006-182">KQL consists of 1 or more free text keywords (words or phrases) or property restrictions.</span></span> <span data-ttu-id="b1006-183">Имя свойства должно быть включено в запрос, будучи либо указанным в самом запросе, либо включаемым в запрос программно.</span><span class="sxs-lookup"><span data-stu-id="b1006-183">The property name must be included in the query, either specified in the query itself or included in the query programmatically.</span></span> <span data-ttu-id="b1006-184">Вы можете использовать сопоставление префиксов с помощью оператора подстановочного знака(\*).</span><span class="sxs-lookup"><span data-stu-id="b1006-184">You can use prefix matching with the wildcard operator(\*).</span></span>

> [!NOTE]
> <span data-ttu-id="b1006-185">Сопоставление суффиксов не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b1006-185">Suffix matching is not supported.</span></span>

![Поиск по запросу "search ba\*" с отображением результатов, соответствующих этому префиксу](./images/search-index-manage-items-schema-2.svg)

<span data-ttu-id="b1006-187">*Поиск по запросу "search ba*" с отображением результатов, соответствующих этому префиксу\*</span><span class="sxs-lookup"><span data-stu-id="b1006-187">*A search for "search ba*" displaying results that match this prefix\*</span></span>

![Поиск по запросу "tags:design" с областью результатов, соответствующих элементам с "design" в свойстве тегов](./images/search-index-manage-items-schema-3.svg)

<span data-ttu-id="b1006-189">*Поиск по запросу "tags:design" с областью результатов, соответствующих элементам с "design" в свойстве тегов*</span><span class="sxs-lookup"><span data-stu-id="b1006-189">*A search for "tags:design" scoping down results to items with "design" in the tags property*</span></span>

### <a name="retrievable"></a><span data-ttu-id="b1006-190">Возможность извлечения</span><span class="sxs-lookup"><span data-stu-id="b1006-190">Retrievable</span></span>

<span data-ttu-id="b1006-191">Если свойство можно извлечь, его значение может возвращаться в результатах поиска.</span><span class="sxs-lookup"><span data-stu-id="b1006-191">If a property is retrievable, its value can be returned in search results.</span></span> <span data-ttu-id="b1006-192">Любое свойство, которое вы хотите добавить в шаблон отображения или вернуть из запроса и показывать в результатах поиска, должно быть извлекаемым.</span><span class="sxs-lookup"><span data-stu-id="b1006-192">Any property that you want to add in the display template or be returned from the query and be relevant in search results must be retrievable.</span></span> <span data-ttu-id="b1006-193">Пометка больших свойств, например `editHistory`, или слишком большого количества свойств в качестве извлекаемых увеличит задержку поиска.</span><span class="sxs-lookup"><span data-stu-id="b1006-193">Marking large properties, such as `editHistory`, or too many properties as retrievable will increase search latency.</span></span> <span data-ttu-id="b1006-194">Будьте внимательны и выбирайте нужные свойства.</span><span class="sxs-lookup"><span data-stu-id="b1006-194">Be selective and choose relevant properties.</span></span>

![Набор свойств, доступных для извлечения, отображаемый в качестве результата](./images/search-index-manage-schema-4.svg)

<span data-ttu-id="b1006-196">*Набор свойств, доступных для извлечения (`title`, `lastEditedBy`и т. д.), отображаемый в качестве результата*</span><span class="sxs-lookup"><span data-stu-id="b1006-196">*A set of retrievable properties (`title`, `lastEditedBy` etc.) rendered as a result*</span></span>

### <a name="refinable"></a><span data-ttu-id="b1006-197">Возможность уточнения</span><span class="sxs-lookup"><span data-stu-id="b1006-197">Refinable</span></span>

<span data-ttu-id="b1006-198">Если свойство поддерживает уточнение, администратор может настроить его в качестве пользовательского фильтра на странице результатов Поиска (Майкрософт).</span><span class="sxs-lookup"><span data-stu-id="b1006-198">If a property is refinable, an admin can configure it as a custom filter in the Microsoft Search results page.</span></span>

![Уточнение результатов по тегам, свойство с возможностью уточнения](./images/search-index-manage-schema-5.svg)

<span data-ttu-id="b1006-200">*Уточнение результатов по `tags`, свойство с возможностью уточнения*</span><span class="sxs-lookup"><span data-stu-id="b1006-200">*Refine results by `tags`, a refinable property*</span></span>

## <a name="labels"></a><span data-ttu-id="b1006-201">Метки</span><span class="sxs-lookup"><span data-stu-id="b1006-201">Labels</span></span>

<span data-ttu-id="b1006-202">Метка — это известный тег, опубликованный корпорацией Майкрософт, который вы можете добавить для свойства в схему.</span><span class="sxs-lookup"><span data-stu-id="b1006-202">A label is a well known tag published by Microsoft that you can add against a property in your schema.</span></span> <span data-ttu-id="b1006-203">Добавление меток позволяет различным продуктам Майкрософт понимать свойство и обеспечивать более удобный интерфейс.</span><span class="sxs-lookup"><span data-stu-id="b1006-203">Adding a label helps various Microsoft products understand the property and provide a better experience.</span></span>

| <span data-ttu-id="b1006-204">Метка</span><span class="sxs-lookup"><span data-stu-id="b1006-204">Label</span></span>                 | <span data-ttu-id="b1006-205">Описание</span><span class="sxs-lookup"><span data-stu-id="b1006-205">Description</span></span>                                                                          |
|---------------------- |------------------------------------------------------------------------------------- |
| <span data-ttu-id="b1006-206">title</span><span class="sxs-lookup"><span data-stu-id="b1006-206">title</span></span>                 | <span data-ttu-id="b1006-207">Название элемента, который должен отображаться в поиске и других интерфейсах</span><span class="sxs-lookup"><span data-stu-id="b1006-207">The title of the item that you want shown in search & other experiences</span></span>              |
| <span data-ttu-id="b1006-208">url</span><span class="sxs-lookup"><span data-stu-id="b1006-208">url</span></span>                   | <span data-ttu-id="b1006-209">Целевой URL-адрес элемента в источнике данных</span><span class="sxs-lookup"><span data-stu-id="b1006-209">The target URL of the item in the data source</span></span>                                        |
| <span data-ttu-id="b1006-210">createdBy</span><span class="sxs-lookup"><span data-stu-id="b1006-210">createdBy</span></span>             | <span data-ttu-id="b1006-211">Имя пользователя, создавшего элемент в источнике данных</span><span class="sxs-lookup"><span data-stu-id="b1006-211">Name of the person who created the item in the data source</span></span>                           |
| <span data-ttu-id="b1006-212">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b1006-212">lastModifiedBy</span></span>        | <span data-ttu-id="b1006-213">Имя пользователя, который последним изменил элемент в источнике данных</span><span class="sxs-lookup"><span data-stu-id="b1006-213">Name of the person who most recently edited the item in the data source</span></span>              |
| <span data-ttu-id="b1006-214">authors</span><span class="sxs-lookup"><span data-stu-id="b1006-214">authors</span></span>               | <span data-ttu-id="b1006-215">Имена всех пользователей, которые участвовали и взаимодействовали в работе над элементом в источнике данных</span><span class="sxs-lookup"><span data-stu-id="b1006-215">Name of all the people who participated/collaborated on the item in the data source</span></span>  |
| <span data-ttu-id="b1006-216">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1006-216">createdDateTime</span></span>       | <span data-ttu-id="b1006-217">Время и дата создания элемента в источнике данных</span><span class="sxs-lookup"><span data-stu-id="b1006-217">Date & time that the item was created in the data source</span></span>                             |
| <span data-ttu-id="b1006-218">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1006-218">lastModifiedDateTime</span></span>  | <span data-ttu-id="b1006-219">Время и дата последнего изменения элемента в источнике данных</span><span class="sxs-lookup"><span data-stu-id="b1006-219">Date & time the item was last modified in the data source</span></span>                            |
| <span data-ttu-id="b1006-220">fileName</span><span class="sxs-lookup"><span data-stu-id="b1006-220">fileName</span></span>              | <span data-ttu-id="b1006-221">В случае с файлом — имя файла в источнике данных</span><span class="sxs-lookup"><span data-stu-id="b1006-221">In case of a file, the name of the file in the data source</span></span>                           |
| <span data-ttu-id="b1006-222">fileExtension</span><span class="sxs-lookup"><span data-stu-id="b1006-222">fileExtension</span></span>         | <span data-ttu-id="b1006-223">В случае с файлом — расширение файла в источнике данных</span><span class="sxs-lookup"><span data-stu-id="b1006-223">In case of a file, the extension of the file in the data source</span></span>                      |

<span data-ttu-id="b1006-224">Например, свойство связи *lastEditedBy* имеет то же значение, что и метка Майкрософт *lastModifiedBy*.</span><span class="sxs-lookup"><span data-stu-id="b1006-224">For example, the connection property *lastEditedBy* has the same meaning as the Microsoft label *lastModifiedBy*.</span></span>

<span data-ttu-id="b1006-225">Добавьте столько меток, сколько сможете, но убедитесь, что они точно соответствуют свойствам.</span><span class="sxs-lookup"><span data-stu-id="b1006-225">Add as many labels as you can, but ensure that they are accurately mapped to properties.</span></span> <span data-ttu-id="b1006-226">Не добавляйте метку к свойству, если она не имеет смысла.</span><span class="sxs-lookup"><span data-stu-id="b1006-226">Do not add a label to a property if it doesn't make sense.</span></span> <span data-ttu-id="b1006-227">Неправильные сопоставления ухудшат взаимодействие.</span><span class="sxs-lookup"><span data-stu-id="b1006-227">Incorrect mappings will deteriorate the experience.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="b1006-228">Все свойства, сопоставленные с метками, должны быть доступны для извлечения.</span><span class="sxs-lookup"><span data-stu-id="b1006-228">All properties that you map to labels must be retrievable.</span></span>

### <a name="relevance"></a><span data-ttu-id="b1006-229">Релевантность</span><span class="sxs-lookup"><span data-stu-id="b1006-229">Relevance</span></span>

<span data-ttu-id="b1006-230">Применяя как можно более точные сопоставленные метки, вы также можете улучшить обнаружение контента при поиске.</span><span class="sxs-lookup"><span data-stu-id="b1006-230">By applying as many accurately mapped labels as possible, you can also improve the discovery of your content through search.</span></span> <span data-ttu-id="b1006-231">Настоятельно рекомендуем определить как можно больше меток ниже, перечисленных по потенциальному влиянию на обнаружение в убывающем порядке:</span><span class="sxs-lookup"><span data-stu-id="b1006-231">We highly recommend defining as many of the below labels as possible, listed by potential impact on discovery in descending order:</span></span>

- <span data-ttu-id="b1006-232">title</span><span class="sxs-lookup"><span data-stu-id="b1006-232">title</span></span>
- <span data-ttu-id="b1006-233">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1006-233">lastModifiedDateTime</span></span>
- <span data-ttu-id="b1006-234">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b1006-234">lastModifiedBy</span></span>
- <span data-ttu-id="b1006-235">url</span><span class="sxs-lookup"><span data-stu-id="b1006-235">url</span></span>
- <span data-ttu-id="b1006-236">filename</span><span class="sxs-lookup"><span data-stu-id="b1006-236">filename</span></span>
- <span data-ttu-id="b1006-237">fileExtension</span><span class="sxs-lookup"><span data-stu-id="b1006-237">fileExtension</span></span>

<span data-ttu-id="b1006-238">Для обнаружения, т. е. сценариев поиска, обратите внимание на следующее:</span><span class="sxs-lookup"><span data-stu-id="b1006-238">For discovery, i.e. search scenarios, please note:</span></span>

- <span data-ttu-id="b1006-239">Используйте точные сопоставления.</span><span class="sxs-lookup"><span data-stu-id="b1006-239">Ensure that your mappings are accurate.</span></span>
- <span data-ttu-id="b1006-240">Когда вы используете свойство в качестве метки, содержащей много контента, вы можете увеличить задержку поиска, и вам придется ждать дольше, чтобы получить результаты.</span><span class="sxs-lookup"><span data-stu-id="b1006-240">When you use a property as label that contains large content, you might increase search latency and have to wait longer for search to return results.</span></span>
- <span data-ttu-id="b1006-241">В частности, в сценарии с настройкой пользовательской вертикали, позволяющей искать несколько связей, результаты поиска значительно выигрывают от назначения максимально большого количества меток.</span><span class="sxs-lookup"><span data-stu-id="b1006-241">Especially in the scenario where you configure a custom vertical that allows search over more than one connection, the search outcomes greatly benefit from appointing as many labels as possible.</span></span>

### <a name="default-result-types"></a><span data-ttu-id="b1006-242">Типы результатов по умолчанию</span><span class="sxs-lookup"><span data-stu-id="b1006-242">Default result types</span></span>

<span data-ttu-id="b1006-243">Метки также влияют на то, как создаются типы результатов, используемые по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b1006-243">Labels also affect how default result types are generated.</span></span> <span data-ttu-id="b1006-244">Добавление меток заголовка и контента как минимум обеспечит создание типа результатов для вашей связи.</span><span class="sxs-lookup"><span data-stu-id="b1006-244">Adding the title and content labels at a minimum will ensure that a result type is created for your connection.</span></span>

![Тип результатов, используемый по умолчанию, с заголовком и фрагментом результата](./images/search-index-manage-schema-6.svg)

<span data-ttu-id="b1006-246">*Тип результатов, используемый по умолчанию, с `title` и фрагментом результата*</span><span class="sxs-lookup"><span data-stu-id="b1006-246">*A default result type with `title` and a result snippet*</span></span>

<span data-ttu-id="b1006-247">Тип результатов, используемый по умолчанию, обеспечивает более эффективное взаимодействие, если вы определите (если применимо) следующие метки, перечисленные по возрастанию:</span><span class="sxs-lookup"><span data-stu-id="b1006-247">Your default result type will provide a better experience when you define these labels, when applicable, listed by ascending order:</span></span>

- <span data-ttu-id="b1006-248">title</span><span class="sxs-lookup"><span data-stu-id="b1006-248">title</span></span>
- <span data-ttu-id="b1006-249">url</span><span class="sxs-lookup"><span data-stu-id="b1006-249">url</span></span>
- <span data-ttu-id="b1006-250">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="b1006-250">lastModifiedBy</span></span>
- <span data-ttu-id="b1006-251">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1006-251">lastModifiedDateTime</span></span>
- <span data-ttu-id="b1006-252">fileName</span><span class="sxs-lookup"><span data-stu-id="b1006-252">fileName</span></span>
- <span data-ttu-id="b1006-253">fileExtension</span><span class="sxs-lookup"><span data-stu-id="b1006-253">fileExtension</span></span>

<span data-ttu-id="b1006-254">Наконец, назначая метки, убедитесь в следующем:</span><span class="sxs-lookup"><span data-stu-id="b1006-254">Finally, when assigning labels, ensure the following:</span></span>

- <span data-ttu-id="b1006-255">Свойства, выбранные в качестве меток, должны быть помечены как доступные для извлечения.</span><span class="sxs-lookup"><span data-stu-id="b1006-255">The properties that you select to function as labels need to be marked retrievable.</span></span>
- <span data-ttu-id="b1006-256">Свойства и назначенные им метки должны иметь одинаковый тип данных.</span><span class="sxs-lookup"><span data-stu-id="b1006-256">The properties and their assigned labels must have the same datatype.</span></span>
- <span data-ttu-id="b1006-257">Можно сопоставить только одну метку с одним свойством.</span><span class="sxs-lookup"><span data-stu-id="b1006-257">You can map exactly one label to exactly one property.</span></span>

## <a name="aliases"></a><span data-ttu-id="b1006-258">Псевдонимы</span><span class="sxs-lookup"><span data-stu-id="b1006-258">Aliases</span></span>

<span data-ttu-id="b1006-259">Псевдонимы — это понятные имена свойств, которые вы назначаете.</span><span class="sxs-lookup"><span data-stu-id="b1006-259">Aliases are friendly names for properties that you assign.</span></span> <span data-ttu-id="b1006-260">Они будут использоваться в запросах и при выборе фильтров уточняемых свойств.</span><span class="sxs-lookup"><span data-stu-id="b1006-260">These will be used in queries and selections in refinable property filters.</span></span>

## <a name="next-steps"></a><span data-ttu-id="b1006-261">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="b1006-261">Next steps</span></span>

- [<span data-ttu-id="b1006-262">Добавление элементов в связь</span><span class="sxs-lookup"><span data-stu-id="b1006-262">Add items to the connection</span></span>](/graph/concepts/search-index-manage-items.md)
- [<span data-ttu-id="b1006-263">Обзор справочника API соединителей Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b1006-263">Review the Microsoft Graph connectors API reference</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)
- [<span data-ttu-id="b1006-264">Настройка страницы результатов поиска Microsoft</span><span class="sxs-lookup"><span data-stu-id="b1006-264">Customize Microsoft Search results page</span></span>](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page)
- [<span data-ttu-id="b1006-265">Поиск объектов настраиваемого типа (externalItem)</span><span class="sxs-lookup"><span data-stu-id="b1006-265">Search custom types (externalItem)</span></span>](search-concept-custom-types.md)
- <span data-ttu-id="b1006-266">Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) с сайта GitHub.</span><span class="sxs-lookup"><span data-stu-id="b1006-266">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub</span></span>
