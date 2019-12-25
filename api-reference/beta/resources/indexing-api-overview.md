---
title: Индексирование данных с помощью API Поиска (Майкрософт)
description: Используйте Microsoft Graph, чтобы индексировать пользовательские элементы или внешние файлы в службе Поиска (Майкрософт).
localization_priority: Priority
author: snlraju-msft
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: f1a39a42f94a072c501c288b55a6b665af0fc640
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870231"
---
# <a name="use-the-microsoft-search-api-to-index-data"></a><span data-ttu-id="967e0-103">Индексирование данных с помощью API Поиска (Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="967e0-103">Use the Microsoft Search API to index data</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="967e0-104">Вы можете использовать Microsoft Graph для добавления пользовательских элементов или внешних файлов в результаты поиска в интерфейсе [Поиска (Майкрософт)](/microsoftsearch/overview-microsoft-search).</span><span class="sxs-lookup"><span data-stu-id="967e0-104">Microsoft Graph lets your app add custom items or external files into search results in the [Microsoft Search](/microsoftsearch/overview-microsoft-search) experience.</span></span>

<span data-ttu-id="967e0-105">Запросы на индексирование данных выполняются от имени приложения без вошедшего пользователя, указываемого [маркером доступа с разрешением приложения](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="967e0-105">Requests to index data are performed on behalf of an application without the presence of a signed-in user, identified using an [access token with application permission](/graph/auth-v2-service).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="common-use-cases"></a><span data-ttu-id="967e0-106">Основные варианты использования</span><span class="sxs-lookup"><span data-stu-id="967e0-106">Common use cases</span></span>

<span data-ttu-id="967e0-107">Варианты использования интерфейсов API в этом разделе содержат создание [соединителей Microsoft Graph](/microsoftsearch/connectors-overview), включая следующие основные этапы:</span><span class="sxs-lookup"><span data-stu-id="967e0-107">The use cases for the APIs in this section center around building [Microsoft Graph connectors](/microsoftsearch/connectors-overview), which involves the main steps of:</span></span>

1. <span data-ttu-id="967e0-108">[Создание подключения](../api/external-post-connections.md) к внешнему источнику данных.</span><span class="sxs-lookup"><span data-stu-id="967e0-108">[Creating a connection](../api/external-post-connections.md) to an external data source</span></span>
2. <span data-ttu-id="967e0-109">[Создание и регистрация схемы](../api/externalconnection-post-schema.md), описывающей тип и способ индексирования внешних данных.</span><span class="sxs-lookup"><span data-stu-id="967e0-109">[Creating and registering a schema](../api/externalconnection-post-schema.md) that describes the type and how to index the external data</span></span>
3. <span data-ttu-id="967e0-110">[Индексирование данных](../api/externalconnection-put-items.md) в качестве внешнего элемента или файла.</span><span class="sxs-lookup"><span data-stu-id="967e0-110">[Indexing the data](../api/externalconnection-put-items.md) as an external item or external file</span></span>

| <span data-ttu-id="967e0-111">Варианты использования</span><span class="sxs-lookup"><span data-stu-id="967e0-111">Use cases</span></span>                                        | <span data-ttu-id="967e0-112">Ресурсы REST</span><span class="sxs-lookup"><span data-stu-id="967e0-112">REST resources</span></span>                              | <span data-ttu-id="967e0-113">См. также</span><span class="sxs-lookup"><span data-stu-id="967e0-113">See also</span></span> |
|:-------------------------------------------------|:--------------------------------------------|:--|
| <span data-ttu-id="967e0-114">**Действия для настройки**</span><span class="sxs-lookup"><span data-stu-id="967e0-114">**Configuration actions**</span></span>                        |                                             |   |
| <span data-ttu-id="967e0-115">Создание, обновление или удаление подключения</span><span class="sxs-lookup"><span data-stu-id="967e0-115">Create, update, or delete a connection</span></span>           | [<span data-ttu-id="967e0-116">externalConnection</span><span class="sxs-lookup"><span data-stu-id="967e0-116">externalConnection</span></span>](externalconnection.md) | [<span data-ttu-id="967e0-117">Методы externalConnection</span><span class="sxs-lookup"><span data-stu-id="967e0-117">externalConnection methods</span></span>](externalconnection.md#methods) |
| <span data-ttu-id="967e0-118">Регистрация схемы для внешних данных</span><span class="sxs-lookup"><span data-stu-id="967e0-118">Register a schema for the external data</span></span>          | [<span data-ttu-id="967e0-119">schema</span><span class="sxs-lookup"><span data-stu-id="967e0-119">schema</span></span>](schema.md)                         | [<span data-ttu-id="967e0-120">Методы schema</span><span class="sxs-lookup"><span data-stu-id="967e0-120">schema methods</span></span>](schema.md#methods) |
| <span data-ttu-id="967e0-121">**Действия для индексирования**</span><span class="sxs-lookup"><span data-stu-id="967e0-121">**Indexing actions**</span></span>                             |                                             |   |
| <span data-ttu-id="967e0-122">Добавление, обновление или удаление пользовательского элемента индекса</span><span class="sxs-lookup"><span data-stu-id="967e0-122">Add, update or delete a custom item in the index</span></span> | [<span data-ttu-id="967e0-123">externalItem</span><span class="sxs-lookup"><span data-stu-id="967e0-123">externalItem</span></span>](externalitem.md)             | [<span data-ttu-id="967e0-124">Методы externalItem</span><span class="sxs-lookup"><span data-stu-id="967e0-124">externalItem methods</span></span>](externalItem.md#methods) |
| <span data-ttu-id="967e0-125">Добавление, обновление или удаление файла в индексе</span><span class="sxs-lookup"><span data-stu-id="967e0-125">Add, update or delete a file in the index</span></span>        | [<span data-ttu-id="967e0-126">externalFile</span><span class="sxs-lookup"><span data-stu-id="967e0-126">externalFile</span></span>](externalfile.md)             | [<span data-ttu-id="967e0-127">Методы externalFile</span><span class="sxs-lookup"><span data-stu-id="967e0-127">externalFile methods</span></span>](externalfile.md#methods) |

## <a name="known-limitations"></a><span data-ttu-id="967e0-128">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="967e0-128">Known limitations</span></span>

<span data-ttu-id="967e0-129">Далее представлены известные ограничения:</span><span class="sxs-lookup"><span data-stu-id="967e0-129">The following are current knownlimitations:</span></span>

- <span data-ttu-id="967e0-130">Организациям доступно до 10 подключений.</span><span class="sxs-lookup"><span data-stu-id="967e0-130">Organizations are limited to a maximum of 10 connections.</span></span>
- <span data-ttu-id="967e0-131">Настраиваемые свойства не поддерживаются при индексировании файлов с помощью ресурса `externalFile`.</span><span class="sxs-lookup"><span data-stu-id="967e0-131">Custom properties are not supported when indexing files using the `externalFile` resource.</span></span>
- <span data-ttu-id="967e0-132">Поддерживаются только удостоверения Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="967e0-132">Only Azure Active Directory identities are supported.</span></span>
- <span data-ttu-id="967e0-133">В секунду можно создавать только четыре элемента ресурсов `externalItem` или `externalFile` в секунду.</span><span class="sxs-lookup"><span data-stu-id="967e0-133">You can create only four `externalItem` or `externalFile` resources items per second.</span></span>
- <span data-ttu-id="967e0-134">Приложение может выполнять до четырех одновременных операций с подключением.</span><span class="sxs-lookup"><span data-stu-id="967e0-134">An application is limited to 4 concurrent operations on a connection.</span></span>
- <span data-ttu-id="967e0-135">Емкость подключений ограничена до 700 000 элементов, или примерно 70 ГБ данных.</span><span class="sxs-lookup"><span data-stu-id="967e0-135">Connections have a capacity limit of 700,000 items or ~70 GB of data.</span></span>
- <span data-ttu-id="967e0-136">Максимальный размер объекта `externalItem` или `externalFile` составляет 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="967e0-136">Maximum size of an `externalItem` or `externalFile` entity is 4 MB.</span></span>
- <span data-ttu-id="967e0-137">Уточнение и сортировка результатов не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="967e0-137">Refining and sorting results is not supported.</span></span>
- <span data-ttu-id="967e0-138">Результаты ранжируются наилучшим возможным способом.</span><span class="sxs-lookup"><span data-stu-id="967e0-138">Result ranking is best effort.</span></span>

## <a name="next-steps"></a><span data-ttu-id="967e0-139">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="967e0-139">Next steps</span></span>

- <span data-ttu-id="967e0-140">См. статью [Обзор API Поиска (Майкрософт)](/graph/search-concept-overview).</span><span class="sxs-lookup"><span data-stu-id="967e0-140">See the [Microsoft Search API overview](/graph/search-concept-overview).</span></span>
- <span data-ttu-id="967e0-141">Подробное описание методов, свойств и связей ресурсов [externalConnection](externalconnection.md), [schema](schema.md), [externalItem](externalitem.md) и [externalFile](externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="967e0-141">Drill down on the methods, properties, and relationships of the [externalConnection](externalconnection.md), [schema](schema.md), [externalItem](externalitem.md), and [externalFile](externalfile.md) resources.</span></span>
- <span data-ttu-id="967e0-142">Ознакомьтесь с [примером соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="967e0-142">Check out the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>
