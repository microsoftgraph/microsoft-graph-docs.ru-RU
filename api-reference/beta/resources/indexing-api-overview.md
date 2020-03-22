---
title: Индексирование данных с помощью API Поиска (Майкрософт)
description: Используйте Microsoft Graph для индексирования пользовательских элементов в службе поиска Microsoft.
localization_priority: Priority
author: snlraju-msft
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: 2d6c49fcdb0a25c0c15fce6c7f7ae0880a3968dd
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892627"
---
# <a name="use-the-microsoft-search-api-to-index-data"></a><span data-ttu-id="219d2-103">Индексирование данных с помощью API Поиска (Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="219d2-103">Use the Microsoft Search API to index data</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="219d2-104">Вы можете использовать Microsoft Graph для добавления пользовательских элементов в результаты поиска в режиме [поиска Microsoft](/microsoftsearch/overview-microsoft-search).</span><span class="sxs-lookup"><span data-stu-id="219d2-104">You can use Microsoft Graph to add custom items to search results in the [Microsoft Search](/microsoftsearch/overview-microsoft-search) experience.</span></span>

<span data-ttu-id="219d2-105">Запросы на индексирование данных выполняются от имени приложения без вошедшего пользователя, указываемого [маркером доступа с разрешением приложения](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="219d2-105">Requests to index data are performed on behalf of an application without the presence of a signed-in user, identified using an [access token with application permission](/graph/auth-v2-service).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="common-use-cases"></a><span data-ttu-id="219d2-106">Основные варианты использования</span><span class="sxs-lookup"><span data-stu-id="219d2-106">Common use cases</span></span>

<span data-ttu-id="219d2-107">Варианты использования интерфейсов API в этом разделе содержат создание [соединителей Microsoft Graph](/microsoftsearch/connectors-overview), включая следующие основные этапы:</span><span class="sxs-lookup"><span data-stu-id="219d2-107">The use cases for the APIs in this section involve building [Microsoft Graph connectors](/microsoftsearch/connectors-overview), which involves the following primary steps:</span></span>

1. <span data-ttu-id="219d2-108">[Создание подключения](../api/external-post-connections.md) к внешнему источнику данных.</span><span class="sxs-lookup"><span data-stu-id="219d2-108">[Create a connection](../api/external-post-connections.md) to an external data source.</span></span>
2. <span data-ttu-id="219d2-109">[Создание и регистрация схемы](../api/externalconnection-post-schema.md), описывающей тип и способ индексирования внешних данных.</span><span class="sxs-lookup"><span data-stu-id="219d2-109">[Create and register a schema](../api/externalconnection-post-schema.md) that describes the type and how to index the external data.</span></span>
3. <span data-ttu-id="219d2-110">[Индексируйте данные](../api/externalconnection-put-items.md) как внешний элемент.</span><span class="sxs-lookup"><span data-stu-id="219d2-110">[Index the data](../api/externalconnection-put-items.md) as an external item.</span></span>

| <span data-ttu-id="219d2-111">Варианты использования</span><span class="sxs-lookup"><span data-stu-id="219d2-111">Use cases</span></span>                                        | <span data-ttu-id="219d2-112">Ресурсы REST</span><span class="sxs-lookup"><span data-stu-id="219d2-112">REST resources</span></span>                              | <span data-ttu-id="219d2-113">См. также</span><span class="sxs-lookup"><span data-stu-id="219d2-113">See also</span></span> |
|:-------------------------------------------------|:--------------------------------------------|:--|
| <span data-ttu-id="219d2-114">**Действия для настройки**</span><span class="sxs-lookup"><span data-stu-id="219d2-114">**Configuration actions**</span></span>                        |                                             |   |
| <span data-ttu-id="219d2-115">Создание, обновление или удаление подключения</span><span class="sxs-lookup"><span data-stu-id="219d2-115">Create, update, or delete a connection</span></span>           | [<span data-ttu-id="219d2-116">externalConnection</span><span class="sxs-lookup"><span data-stu-id="219d2-116">externalConnection</span></span>](externalconnection.md) | [<span data-ttu-id="219d2-117">Методы externalConnection</span><span class="sxs-lookup"><span data-stu-id="219d2-117">externalConnection methods</span></span>](externalconnection.md#methods) |
| <span data-ttu-id="219d2-118">Регистрация схемы для внешних данных</span><span class="sxs-lookup"><span data-stu-id="219d2-118">Register a schema for the external data</span></span>          | [<span data-ttu-id="219d2-119">schema</span><span class="sxs-lookup"><span data-stu-id="219d2-119">schema</span></span>](schema.md)                         | [<span data-ttu-id="219d2-120">Методы schema</span><span class="sxs-lookup"><span data-stu-id="219d2-120">schema methods</span></span>](schema.md#methods) |
| <span data-ttu-id="219d2-121">**Действия для индексирования**</span><span class="sxs-lookup"><span data-stu-id="219d2-121">**Indexing actions**</span></span>                             |                                             |   |
| <span data-ttu-id="219d2-122">Добавление, обновление или удаление пользовательского элемента индекса</span><span class="sxs-lookup"><span data-stu-id="219d2-122">Add, update or delete a custom item in the index</span></span> | [<span data-ttu-id="219d2-123">externalItem</span><span class="sxs-lookup"><span data-stu-id="219d2-123">externalItem</span></span>](externalitem.md)             | [<span data-ttu-id="219d2-124">Методы externalItem</span><span class="sxs-lookup"><span data-stu-id="219d2-124">externalItem methods</span></span>](externalItem.md#methods) |

## <a name="known-limitations"></a><span data-ttu-id="219d2-125">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="219d2-125">Known limitations</span></span>

<span data-ttu-id="219d2-126">Далее представлены известные ограничения:</span><span class="sxs-lookup"><span data-stu-id="219d2-126">The following are current knownlimitations:</span></span>

- <span data-ttu-id="219d2-127">Организациям доступно до 10 подключений.</span><span class="sxs-lookup"><span data-stu-id="219d2-127">Organizations are limited to a maximum of 10 connections.</span></span>
- <span data-ttu-id="219d2-128">Поддерживаются только удостоверения Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="219d2-128">Only Azure Active Directory identities are supported.</span></span>
- <span data-ttu-id="219d2-129">Вы можете создавать только четыре `externalItem` элемента ресурсов в секунду.</span><span class="sxs-lookup"><span data-stu-id="219d2-129">You can create only four `externalItem` resources items per second.</span></span>
- <span data-ttu-id="219d2-130">Приложение может выполнять до четырех одновременных операций с подключением.</span><span class="sxs-lookup"><span data-stu-id="219d2-130">An application is limited to four concurrent operations on a connection.</span></span>
- <span data-ttu-id="219d2-131">Емкость подключений ограничена до 700 000 элементов, или примерно 70 ГБ данных.</span><span class="sxs-lookup"><span data-stu-id="219d2-131">Connections have a capacity limit of 700,000 items or ~70 GB of data.</span></span>
- <span data-ttu-id="219d2-132">Максимальный размер объекта `externalItem` составляет 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="219d2-132">Maximum size of an `externalItem` entity is 4 MB.</span></span>
- <span data-ttu-id="219d2-133">Уточнение и сортировка результатов не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="219d2-133">Refining and sorting results is not supported.</span></span>
- <span data-ttu-id="219d2-134">Результаты ранжируются наилучшим возможным способом.</span><span class="sxs-lookup"><span data-stu-id="219d2-134">Result ranking is best effort.</span></span>

## <a name="next-steps"></a><span data-ttu-id="219d2-135">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="219d2-135">Next steps</span></span>

- <span data-ttu-id="219d2-136">См. статью [Обзор API Поиска (Майкрософт)](/graph/search-concept-overview).</span><span class="sxs-lookup"><span data-stu-id="219d2-136">See the [Microsoft Search API overview](/graph/search-concept-overview).</span></span>
- <span data-ttu-id="219d2-137">Разверните методы, свойства и отношения ресурсов [externalConnection](externalconnection.md), [схемы](schema.md) и [externalItem](externalitem.md).</span><span class="sxs-lookup"><span data-stu-id="219d2-137">Drill down on the methods, properties, and relationships of the [externalConnection](externalconnection.md), [schema](schema.md), and [externalItem](externalitem.md) resources.</span></span>
- <span data-ttu-id="219d2-138">Ознакомьтесь с [примером соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="219d2-138">Check out the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>
