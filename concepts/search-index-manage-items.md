---
title: Создание, обновление и удаление элементов, добавленных приложением в индекс службы "Поиск (Майкрософт)"
description: Узнайте, как использовать Microsoft Graph для управления элементами, добавленными приложением в службу "Поиск (Майкрософт)".
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: c5017943f966792e0246d3764a1c3e373718c63c
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/19/2019
ms.locfileid: "38704338"
---
# <a name="create-update-and-delete-items-added-by-your-application-in-the-microsoft-search-service-index"></a><span data-ttu-id="e0e67-103">Создание, обновление и удаление элементов, добавленных приложением в индекс службы "Поиск (Майкрософт)"</span><span class="sxs-lookup"><span data-stu-id="e0e67-103">Create, update, and delete items added by your application in the Microsoft Search service index</span></span>

<span data-ttu-id="e0e67-104">Элементы, добавленные приложением в службу "Поиск (Майкрософт)", представлены ресурсами [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) и [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e0e67-104">Items added by your application to the Microsoft Search service are represented by the [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) and [externalFile](/graph/api/resources/externalfile?view=graph-rest-beta) resources in Microsoft Graph.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

<span data-ttu-id="e0e67-105">Ресурс **externalItem** представляет настраиваемый тип.</span><span class="sxs-lookup"><span data-stu-id="e0e67-105">The **externalItem** resource represents a custom type.</span></span> <span data-ttu-id="e0e67-106">Его следует использовать, если элементы, добавленные в индекс, основаны на пользовательской схеме, не представленной ресурсом **externalFile**.</span><span class="sxs-lookup"><span data-stu-id="e0e67-106">It should be used when the items you add to the index use a custom schema not represented by the **externalFile** resource.</span></span> <span data-ttu-id="e0e67-107">Например, это могут быть запросы в службу технической поддержки или описания продуктов.</span><span class="sxs-lookup"><span data-stu-id="e0e67-107">For example, helpdesk tickets or product listings.</span></span>

<span data-ttu-id="e0e67-108">Ресурс **externalFile** представляет файл во внешней системе.</span><span class="sxs-lookup"><span data-stu-id="e0e67-108">The **externalFile** resource represents a file in an external system.</span></span>

> [!NOTE]
> <span data-ttu-id="e0e67-109">Схему **externalFile** невозможно расширить.</span><span class="sxs-lookup"><span data-stu-id="e0e67-109">The schema for **externalFile** cannot be extended.</span></span>

## <a name="add-an-item-or-file"></a><span data-ttu-id="e0e67-110">Добавление элемента или файла</span><span class="sxs-lookup"><span data-stu-id="e0e67-110">Add an item or file</span></span>

<span data-ttu-id="e0e67-111">Вы можете добавить элемент или файл в индекс, [создав объект externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="e0e67-111">You can add an item or file to the index by [creating an externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta).</span></span> <span data-ttu-id="e0e67-112">При создании элемента ему назначается уникальный идентификатор в URL-адресе.</span><span class="sxs-lookup"><span data-stu-id="e0e67-112">When you create an item, you assign a unique identifier in the URL.</span></span>

<span data-ttu-id="e0e67-113">Например, приложение может индексировать запросы в службу технической поддержки по их номерам.</span><span class="sxs-lookup"><span data-stu-id="e0e67-113">For example, your application may index helpdesk tickets using the ticket number.</span></span> <span data-ttu-id="e0e67-114">Если запросу назначен номер `SR00145`, он может выглядеть так:</span><span class="sxs-lookup"><span data-stu-id="e0e67-114">If a ticket has the ticket number `SR00145`, the request may look like the following.</span></span>

```http
PUT /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "title": "WiFi outage in Conference Room A",
  "status": "New",
  "assignee": "meganb@contoso.com"
}
```

## <a name="update-an-item-or-file"></a><span data-ttu-id="e0e67-115">Обновление элемента или файла</span><span class="sxs-lookup"><span data-stu-id="e0e67-115">Update an item or file</span></span>

<span data-ttu-id="e0e67-116">При обновлении элемента или файла во внешней службе (переназначении запросов в службу технической поддержки или обновлении описания продукта), вы можете обновить соответствующую запись в индексе, [обновив объект externalItem](/graph/api/externalitem-update?view=graph-rest-beta) по уникальному идентификатору, назначенному элементу при его создании.</span><span class="sxs-lookup"><span data-stu-id="e0e67-116">When an item or file is updated in the external service (helpdesk ticket is reassigned, or a product description is updated), you can update its entry in the index by [updating the externalItem](/graph/api/externalitem-update?view=graph-rest-beta), using the unique identifier assigned to the item when you created it.</span></span>

```http
PATCH /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "assignee": "alexw@contoso.com"
}
```

## <a name="delete-an-item-or-file"></a><span data-ttu-id="e0e67-117">Удаление элемента или файла</span><span class="sxs-lookup"><span data-stu-id="e0e67-117">Delete an item or file</span></span>

<span data-ttu-id="e0e67-118">Вы можете удалить элементы или файлы из индекса, [удалив объект externalItem](/graph/api/externalitem-delete?view=graph-rest-beta) по уникальному идентификатору, назначенному при его создании.</span><span class="sxs-lookup"><span data-stu-id="e0e67-118">You can remove items or files from the index by [deleting the externalItem](/graph/api/externalitem-delete?view=graph-rest-beta), using the unique identifier assigned to the item when you created it.</span></span>

```http
DELETE /external/connections/contosohelpdesk/items/SR00145
```

## <a name="next-steps"></a><span data-ttu-id="e0e67-119">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="e0e67-119">Next steps</span></span>

- [<span data-ttu-id="e0e67-120">Зачем использовать API Поиска (Майкрософт)?</span><span class="sxs-lookup"><span data-stu-id="e0e67-120">Why use the Microsoft Search API?</span></span>](search-concept-overview.md#why-use-the-microsoft-search-api)
- [<span data-ttu-id="e0e67-121">Использование API Поиска (Майкрософт) для индексирования данных</span><span class="sxs-lookup"><span data-stu-id="e0e67-121">Use the Microsoft Search API to index data</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [<span data-ttu-id="e0e67-122">Поиск объектов настраиваемого типа (externalItem)</span><span class="sxs-lookup"><span data-stu-id="e0e67-122">Search custom types (externalItem)</span></span>](search-concept-custom-types.md)
- [<span data-ttu-id="e0e67-123">Поиск файлов (включая externalFile)</span><span class="sxs-lookup"><span data-stu-id="e0e67-123">Search files (including externalFile)</span></span>](search-concept-files.md)
- <span data-ttu-id="e0e67-124">Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) с сайта GitHub.</span><span class="sxs-lookup"><span data-stu-id="e0e67-124">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub</span></span>
