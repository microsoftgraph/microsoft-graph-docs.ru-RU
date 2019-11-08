---
title: Создание, обновление и удаление подключений к службе "Поиск (Майкрософт)"
description: Узнайте, как использовать Microsoft Graph для управления подключениями к службе "Поиск (Майкрософт)".
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: b1f599a4610ce4cb939c7733949eac4c0ddba371
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939532"
---
# <a name="create-update-and-delete-connections-to-the-microsoft-search-service"></a><span data-ttu-id="46b6e-103">Создание, обновление и удаление подключений к службе "Поиск (Майкрософт)"</span><span class="sxs-lookup"><span data-stu-id="46b6e-103">Create, update, and delete connections to the Microsoft Search service</span></span>

<span data-ttu-id="46b6e-104">Подключения внешних служб к службе "Поиск (Майкрософт)" представляются ресурсом [externalConnection](/graph/api/resources/externalconnection?view=graph-rest-beta) в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="46b6e-104">Connections from external services to the Microsoft Search service are represented by the [externalConnection](/graph/api/resources/externalconnection?view=graph-rest-beta) resource in Microsoft Graph.</span></span>

<span data-ttu-id="46b6e-105">Подключение позволяет приложению [определить схему](/graph/api/externalconnection-post-schema?view=graph-rest-beta) для индексируемых элементов, а также предоставляет службе конечную точку для [добавления, обновления и удаления элементов индекса](search-index-manage-items.md).</span><span class="sxs-lookup"><span data-stu-id="46b6e-105">A connection allows your application to [define a schema](/graph/api/externalconnection-post-schema?view=graph-rest-beta) for items that will be indexed, and provides an endpoint for your service to [add, update, or delete items from the index](search-index-manage-items.md).</span></span> <span data-ttu-id="46b6e-106">Создание подключения — первый шаг приложения к добавлению элементов в индекс поиска.</span><span class="sxs-lookup"><span data-stu-id="46b6e-106">Creating a connection is the first step for an application to add items to the search index.</span></span>

## <a name="create-a-connection"></a><span data-ttu-id="46b6e-107">Создание подключения</span><span class="sxs-lookup"><span data-stu-id="46b6e-107">Create a connection</span></span>

<span data-ttu-id="46b6e-108">Чтобы приложение могло добавлять элементы в индекс поиска, ему необходимо создать и настроить подключение, выполнив указанные ниже действия.</span><span class="sxs-lookup"><span data-stu-id="46b6e-108">Before an application can add items to the search index, it must create and configure a connection using the following steps.</span></span>

- <span data-ttu-id="46b6e-109">[Создание подключения](/graph/api/external-post-connections?view=graph-rest-beta) с уникальным идентификатором, отображаемым именем и описанием.</span><span class="sxs-lookup"><span data-stu-id="46b6e-109">[Create a connection](/graph/api/external-post-connections?view=graph-rest-beta) with a unique ID, display name, and description.</span></span>
- <span data-ttu-id="46b6e-110">[Регистрация схемы](/graph/api/externalconnection-post-schema?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="46b6e-110">[Registering a schema](/graph/api/externalconnection-post-schema?view=graph-rest-beta).</span></span>
  - <span data-ttu-id="46b6e-111">Для пользовательских элементов (например, обращений в службу технической поддержки, записей базы данных инвентаризации и т. д.) необходимо определить поля, включенные в индекс.</span><span class="sxs-lookup"><span data-stu-id="46b6e-111">For custom items (such as heldesk tickets or inventory database entries, etc.), define the fields that will be included in the index.</span></span>
  - <span data-ttu-id="46b6e-112">Для внешних файлов следует задать тип `microsoft.graph.externalFile`.</span><span class="sxs-lookup"><span data-stu-id="46b6e-112">For external files, specify the `microsoft.graph.externalFile` type.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="46b6e-113">После регистрации схемы ее невозможно изменить для существующего подключения.</span><span class="sxs-lookup"><span data-stu-id="46b6e-113">Once a schema has been registered, it cannot be changed for an existing connection.</span></span>

## <a name="update-a-connection"></a><span data-ttu-id="46b6e-114">Обновление подключения</span><span class="sxs-lookup"><span data-stu-id="46b6e-114">Update a connection</span></span>

<span data-ttu-id="46b6e-115">Вы можете изменить отображаемое имя или описание существующего подключения, [обновив подключение](/graph/api/externalconnection-update?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="46b6e-115">You can change the display name or description of an existing connection by [updating the connection](/graph/api/externalconnection-update?view=graph-rest-beta).</span></span>

## <a name="delete-a-connection"></a><span data-ttu-id="46b6e-116">Удаление подключения</span><span class="sxs-lookup"><span data-stu-id="46b6e-116">Delete a connection</span></span>

<span data-ttu-id="46b6e-117">Вы можете [удалить подключение](/graph/api/externalconnection-delete?view=graph-rest-beta) и удалить все элементы, индексированные через него.</span><span class="sxs-lookup"><span data-stu-id="46b6e-117">You can [delete a connection](/graph/api/externalconnection-delete?view=graph-rest-beta), and remove all items that were indexed via that connection.</span></span>

## <a name="next-steps"></a><span data-ttu-id="46b6e-118">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="46b6e-118">Next steps</span></span>

- [<span data-ttu-id="46b6e-119">Зачем использовать API Поиска (Майкрософт)?</span><span class="sxs-lookup"><span data-stu-id="46b6e-119">Why use the Microsoft Graph Security API?</span></span>](search-concept-overview.md#why-use-the-microsoft-search-api)
- [<span data-ttu-id="46b6e-120">Использование API Поиска (Майкрософт) для индексирования данных</span><span class="sxs-lookup"><span data-stu-id="46b6e-120">Use the Microsoft Search API to index data</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [<span data-ttu-id="46b6e-121">Обзор соединителей Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="46b6e-121">Overview for Microsoft Graph Connectors</span></span>](/microsoftsearch/connectors-overview)
- <span data-ttu-id="46b6e-122">Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) с сайта GitHub.</span><span class="sxs-lookup"><span data-stu-id="46b6e-122">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub</span></span>
