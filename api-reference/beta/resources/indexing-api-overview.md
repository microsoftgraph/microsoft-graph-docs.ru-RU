---
title: Индексирование данных с помощью API Поиска (Майкрософт)
description: Microsoft Graph позволяет приложению индексировать пользовательские элементы или внешние файлы в службе "Поиск (Майкрософт)".
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: cac6d8e9d399e13554e9a9ef44fe8d869c0ad70d
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938950"
---
# <a name="use-the-microsoft-search-api-to-index-data"></a><span data-ttu-id="1dd7a-103">Индексирование данных с помощью API Поиска (Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dd7a-103">Use the Microsoft Search API to index data</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1dd7a-104">Microsoft Graph позволяет приложению добавлять настраиваемые элементы или внешние файлы в результаты поиска в службе [Поиск (Майкрософт)](/microsoftsearch/overview-microsoft-search).</span><span class="sxs-lookup"><span data-stu-id="1dd7a-104">Microsoft Graph lets your app add custom items or external files into search results in the [Microsoft Search](/microsoftsearch/overview-microsoft-search) experience.</span></span>

<span data-ttu-id="1dd7a-105">Запросы на индексирование данных выполняются от имени приложения без вошедшего пользователя, указываемого [маркером доступа с разрешением приложения](/graph/auth-v2-service).</span><span class="sxs-lookup"><span data-stu-id="1dd7a-105">Requests to index data are performed on behalf of an application without the presence of a signed-in user, identified using an [access token with application permission](/graph/auth-v2-service).</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="1dd7a-106">Распространенные варианты использования</span><span class="sxs-lookup"><span data-stu-id="1dd7a-106">Common use cases</span></span>

<span data-ttu-id="1dd7a-107">Варианты использования интерфейсов API в этом разделе сосредоточены на создании [соединителей Microsoft Graph](/microsoftsearch/connectors-overview), включающем следующие основные этапы:</span><span class="sxs-lookup"><span data-stu-id="1dd7a-107">The use cases for the APIs in this section center around building [Microsoft Graph connectors](/microsoftsearch/connectors-overview), which involves the main steps of:</span></span>

1. <span data-ttu-id="1dd7a-108">[создание подключения](../api/external-post-connections.md) к внешнему источнику данных;</span><span class="sxs-lookup"><span data-stu-id="1dd7a-108">[Creating a connection](../api/external-post-connections.md) to an external data source</span></span>
2. <span data-ttu-id="1dd7a-109">[создание и регистрация схемы](../api/externalconnection-post-schema.md), описывающей тип и способ индексирования внешних данных;</span><span class="sxs-lookup"><span data-stu-id="1dd7a-109">[Creating and registering a schema](../api/externalconnection-post-schema.md) that describes the type and how to index the external data</span></span>
3. <span data-ttu-id="1dd7a-110">[индексирование данных](../api/externalconnection-put-items.md) в качестве внешнего элемента или файла.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-110">[Indexing the data](../api/externalconnection-put-items.md) as an external item or external file</span></span>

| <span data-ttu-id="1dd7a-111">Варианты использования</span><span class="sxs-lookup"><span data-stu-id="1dd7a-111">Use cases</span></span>                                        | <span data-ttu-id="1dd7a-112">Ресурсы REST</span><span class="sxs-lookup"><span data-stu-id="1dd7a-112">REST resources</span></span>                              | <span data-ttu-id="1dd7a-113">См. также</span><span class="sxs-lookup"><span data-stu-id="1dd7a-113">See also</span></span> |
|:-------------------------------------------------|:--------------------------------------------|:--|
| <span data-ttu-id="1dd7a-114">**Действия для настройки**</span><span class="sxs-lookup"><span data-stu-id="1dd7a-114">**Configuration actions**</span></span>                        |                                             |   |
| <span data-ttu-id="1dd7a-115">Создание, обновление или удаление подключения</span><span class="sxs-lookup"><span data-stu-id="1dd7a-115">Create, get, update, or delete a business</span></span>           | [<span data-ttu-id="1dd7a-116">externalConnection</span><span class="sxs-lookup"><span data-stu-id="1dd7a-116">externalConnection</span></span>](externalconnection.md) | [<span data-ttu-id="1dd7a-117">Методы объекта externalConnection</span><span class="sxs-lookup"><span data-stu-id="1dd7a-117">Methods of externalConnection</span></span>](externalconnection.md#methods) |
| <span data-ttu-id="1dd7a-118">Регистрация схемы для внешних данных</span><span class="sxs-lookup"><span data-stu-id="1dd7a-118">Register a schema for the external data</span></span>          | [<span data-ttu-id="1dd7a-119">schema</span><span class="sxs-lookup"><span data-stu-id="1dd7a-119">SCHEMA</span></span>](schema.md)                         | [<span data-ttu-id="1dd7a-120">Методы объекта schema</span><span class="sxs-lookup"><span data-stu-id="1dd7a-120">Methods of schema</span></span>](schema.md#methods) |
| <span data-ttu-id="1dd7a-121">**Действия для индексирования**</span><span class="sxs-lookup"><span data-stu-id="1dd7a-121">**Indexing actions**</span></span>                             |                                             |   |
| <span data-ttu-id="1dd7a-122">Добавление, обновление или удаление пользовательского элемента индекса</span><span class="sxs-lookup"><span data-stu-id="1dd7a-122">Add, update or delete a custom item in the index</span></span> | [<span data-ttu-id="1dd7a-123">externalItem</span><span class="sxs-lookup"><span data-stu-id="1dd7a-123">externalItem</span></span>](externalitem.md)             | [<span data-ttu-id="1dd7a-124">Методы объекта externalItem</span><span class="sxs-lookup"><span data-stu-id="1dd7a-124">Methods of externalItem</span></span>](externalItem.md#methods) |
| <span data-ttu-id="1dd7a-125">Добавление, обновление или удаление файла в индексе</span><span class="sxs-lookup"><span data-stu-id="1dd7a-125">Add, update or delete a file in the index</span></span>        | [<span data-ttu-id="1dd7a-126">externalFile</span><span class="sxs-lookup"><span data-stu-id="1dd7a-126">externalFile</span></span>](externalfile.md)             | [<span data-ttu-id="1dd7a-127">Методы объекта externalFile</span><span class="sxs-lookup"><span data-stu-id="1dd7a-127">Methods of externalFile</span></span>](externalfile.md#methods) |

## <a name="known-limitations"></a><span data-ttu-id="1dd7a-128">Известные ограничения</span><span class="sxs-lookup"><span data-stu-id="1dd7a-128">Known limitations</span></span>

<span data-ttu-id="1dd7a-129">Работая с предварительной версией, учитывайте описанные ниже факторы.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-129">Note the following limitations during preview.</span></span>

- <span data-ttu-id="1dd7a-130">Организациям доступно до 10 подключений.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-130">Organizations are limited to a maximum of 10 connections.</span></span>
- <span data-ttu-id="1dd7a-131">Настраиваемые свойства не поддерживаются при индексировании файлов с помощью ресурса `externalFile`.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-131">No support for custom properties when indexing files using the `externalFile` resource.</span></span>
- <span data-ttu-id="1dd7a-132">Поддерживаются только удостоверения Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-132">Only Azure Active Directory identities are supported.</span></span>
- <span data-ttu-id="1dd7a-133">Создание ресурсов `externalItem` или `externalFile` ограничено до 4 элементов в секунду.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-133">Creating `externalItem` or `externalFile` resources is limited to 4 items per second.</span></span>
- <span data-ttu-id="1dd7a-134">Приложение может выполнять до 4 одновременных операций с подключением.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-134">An application is limited to 4 concurrent operations on a connection.</span></span>
- <span data-ttu-id="1dd7a-135">Емкость подключений ограничена до 700 000 элементов, или примерно 70 ГБ данных.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-135">Connections have a capacity limit of 700,000 items or ~70 GB of data.</span></span>
- <span data-ttu-id="1dd7a-136">Максимальный размер объекта `externalItem` или `externalFile` составляет 4 МБ.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-136">Maximum size of an `externalItem` or `externalFile` entity is 4 MB.</span></span>
- <span data-ttu-id="1dd7a-137">Уточнение и сортировка результатов не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-137">No support for refining and sorting results.</span></span>
- <span data-ttu-id="1dd7a-138">Результаты ранжируются наилучшим возможным способом.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-138">Result ranking is best effort.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1dd7a-139">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="1dd7a-139">Next steps</span></span>

- [<span data-ttu-id="1dd7a-140">Обзор API Поиска (Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1dd7a-140">Microsoft Bookings API overview</span></span>](/graph/search-concept-overview)
- <span data-ttu-id="1dd7a-141">Подробное описание методов, свойств и связей ресурсов [externalConnection](externalconnection.md), [schema](schema.md), [externalItem](externalitem.md) и [externalFile](externalfile.md).</span><span class="sxs-lookup"><span data-stu-id="1dd7a-141">Drill down on the [methods](externalconnection.md), [properties](schema.md), and [relationships](externalitem.md) of the [message](externalfile.md) and mailFolder resources.</span></span>
- <span data-ttu-id="1dd7a-142">Ознакомьтесь с [примером соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) на сайте GitHub.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-142">Check out the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub.</span></span>
