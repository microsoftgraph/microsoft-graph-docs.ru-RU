---
title: Создание, обновление и удаление элементов, добавленных приложением в индекс службы "Поиск (Майкрософт)"
description: Узнайте, как использовать Microsoft Graph для управления элементами, добавленными приложением в службу "Поиск (Майкрософт)".
localization_priority: Priority
author: snlraju-msft
ms.prod: ''
doc_type: conceptualPageType
ms.openlocfilehash: 5b969bd058b8c1e2790b0039a4369623287f641d
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892788"
---
# <a name="create-update-and-delete-items-added-by-your-application-in-the-microsoft-search-service-index"></a><span data-ttu-id="abcdb-103">Создание, обновление и удаление элементов, добавленных приложением в индекс службы "Поиск (Майкрософт)"</span><span class="sxs-lookup"><span data-stu-id="abcdb-103">Create, update, and delete items added by your application in the Microsoft Search service index</span></span>

<span data-ttu-id="abcdb-104">Элементы, добавленные приложением в службу "Поиск (Майкрософт)", представлены ресурсом [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="abcdb-104">Items added by your application to the Microsoft Search service are represented by the [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta) resource in Microsoft Graph.</span></span>

[!INCLUDE [search-api-preview-signup](../includes/search-api-preview-signup.md)]

## <a name="add-an-item"></a><span data-ttu-id="abcdb-105">Добавление элемента</span><span class="sxs-lookup"><span data-stu-id="abcdb-105">Add an item</span></span>

<span data-ttu-id="abcdb-106">Вы можете добавить элемент в индекс, [создав объект externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="abcdb-106">You can add an item to the index by [creating an externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta).</span></span> <span data-ttu-id="abcdb-107">При создании элемента ему назначается уникальный идентификатор в URL-адресе.</span><span class="sxs-lookup"><span data-stu-id="abcdb-107">When you create an item, you assign a unique identifier in the URL.</span></span>

<span data-ttu-id="abcdb-108">Например, приложение может индексировать запросы в службу технической поддержки по их номерам.</span><span class="sxs-lookup"><span data-stu-id="abcdb-108">For example, your application may index helpdesk tickets using the ticket number.</span></span> <span data-ttu-id="abcdb-109">Если запросу назначен номер `SR00145`, он может выглядеть так:</span><span class="sxs-lookup"><span data-stu-id="abcdb-109">If a ticket has the ticket number `SR00145`, the request may look like the following.</span></span>

```http
PUT /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "title": "WiFi outage in Conference Room A",
  "status": "New",
  "assignee": "meganb@contoso.com"
}
```

> <span data-ttu-id="abcdb-110">![ПРИМЕЧАНИЕ] Перед поиском индексированных элементов в пользовательском интерфейсе "Поиск (Майкрософт)", администратор должен [настроить страницу результатов поиска](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page) для соответствующего подключения.</span><span class="sxs-lookup"><span data-stu-id="abcdb-110">![NOTE] Before indexed items can be found in the Microsoft Search UI, an administrator must [customize the search results page](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page) for the corresponding connection.</span></span>

## <a name="update-an-item"></a><span data-ttu-id="abcdb-111">Обновление элемента</span><span class="sxs-lookup"><span data-stu-id="abcdb-111">Update an item</span></span>

<span data-ttu-id="abcdb-112">При обновлении элемента во внешней службе (переназначении запросов в службу технической поддержки или обновлении описания продукта), вы можете обновить соответствующую запись в индексе, [обновив externalItem](/graph/api/externalitem-update?view=graph-rest-beta) по уникальному идентификатору, назначенному элементу при его создании.</span><span class="sxs-lookup"><span data-stu-id="abcdb-112">When an item is updated in the external service (helpdesk ticket is reassigned, or a product description is updated), you can update its entry in the index by [updating the externalItem](/graph/api/externalitem-update?view=graph-rest-beta), using the unique identifier assigned to the item when you created it.</span></span>

```http
PATCH /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "assignee": "alexw@contoso.com"
}
```

## <a name="delete-an-item"></a><span data-ttu-id="abcdb-113">Удаление элемента</span><span class="sxs-lookup"><span data-stu-id="abcdb-113">Delete an item</span></span>

<span data-ttu-id="abcdb-114">Вы можете удалить элементы из индекса, [удалив externalItem](/graph/api/externalitem-delete?view=graph-rest-beta) по уникальному идентификатору, назначенному при его создании.</span><span class="sxs-lookup"><span data-stu-id="abcdb-114">You can remove items from the index by [deleting the externalItem](/graph/api/externalitem-delete?view=graph-rest-beta), using the unique identifier assigned to the item when you created it.</span></span>

```http
DELETE /external/connections/contosohelpdesk/items/SR00145
```

## <a name="next-steps"></a><span data-ttu-id="abcdb-115">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="abcdb-115">Next steps</span></span>

- [<span data-ttu-id="abcdb-116">Зачем использовать API Поиска (Майкрософт)?</span><span class="sxs-lookup"><span data-stu-id="abcdb-116">Why use the Microsoft Search API?</span></span>](search-concept-overview.md#why-use-the-microsoft-search-api)
- [<span data-ttu-id="abcdb-117">Обзор индексирования справочных материалов по API</span><span class="sxs-lookup"><span data-stu-id="abcdb-117">Review the Indexing API reference</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta)
- [<span data-ttu-id="abcdb-118">Настройка страницы результатов поиска Microsoft</span><span class="sxs-lookup"><span data-stu-id="abcdb-118">Customize Microsoft Search results page</span></span>](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page)
- [<span data-ttu-id="abcdb-119">Поиск объектов настраиваемого типа (externalItem)</span><span class="sxs-lookup"><span data-stu-id="abcdb-119">Search custom types (externalItem)</span></span>](search-concept-custom-types.md)
- <span data-ttu-id="abcdb-120">Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) с сайта GitHub.</span><span class="sxs-lookup"><span data-stu-id="abcdb-120">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub</span></span>
