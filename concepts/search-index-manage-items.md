---
title: Создание, обновление и удаление элементов, добавленных приложением в связь Microsoft Graph
description: Узнайте, как использовать Microsoft Graph для управления элементами, добавленными приложением в службу "Поиск (Майкрософт)".
localization_priority: Priority
author: rsamai
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: c2cae0ca25d55fd95a7b26c0175f7e5313d6e532
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962401"
---
# <a name="create-update-and-delete-items-added-by-your-application-in-the-microsoft-graph-connection"></a><span data-ttu-id="33444-103">Создание, обновление и удаление элементов, добавленных приложением в связь Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="33444-103">Create, update, and delete items added by your application in the Microsoft Graph connection</span></span>

<span data-ttu-id="33444-104">Элементы, добавленные приложением в службу "Поиск (Майкрософт)", представлены ресурсом [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="33444-104">Items added by your application to the Microsoft Search service are represented by the [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) resource in Microsoft Graph.</span></span>

<span data-ttu-id="33444-105">После создания связи вы можете добавить содержимое.</span><span class="sxs-lookup"><span data-stu-id="33444-105">Once you have created a connection, you can add your content.</span></span> <span data-ttu-id="33444-106">Каждый элемент из источника данных должен быть представлен в виде [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) в Microsoft Graph с уникальным идентификатором элемента. Этот идентификатор используется для создания, обновления или удаления элемента в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="33444-106">Each item from your data source must be represented as an [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) in Microsoft Graph with a unique item id. This id is used to create, update or delete the item from Microsoft Graph.</span></span> <span data-ttu-id="33444-107">Вы можете использовать первичный ключ из источника данных в качестве itemId или получить его из одного или нескольких полей.</span><span class="sxs-lookup"><span data-stu-id="33444-107">You can use the primary key from your data source as the itemId or derive it from one or more fields.</span></span> <span data-ttu-id="33444-108">[externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) содержит три основных компонента: список управления доступом, свойства и содержимое.</span><span class="sxs-lookup"><span data-stu-id="33444-108">An [externalItem](/graph/api/resources/externalitem?view=graph-rest-beta&preserve-view=true) has three key components: access control list, properties, and content.</span></span>

## <a name="access-control-list"></a><span data-ttu-id="33444-109">Список управления доступом</span><span class="sxs-lookup"><span data-stu-id="33444-109">Access control list</span></span>

<span data-ttu-id="33444-110">Список управления доступом используется для указания того, предоставляется ли определенным ролям доступ для просмотра элементов в интерфейсах Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="33444-110">The access control list is used to specify whether the given roles are granted or denied access to view items in Microsoft experiences.</span></span> <span data-ttu-id="33444-111">Это массив записей управления доступом, каждая из которых представляет пользователя или группу Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="33444-111">It is an array of access control entries, each representing an Azure Active Directory user or group.</span></span> <span data-ttu-id="33444-112">Существует третий тип записей управления доступом: `Everyone`, который представляет всех пользователей в клиенте.</span><span class="sxs-lookup"><span data-stu-id="33444-112">There is a third access control entry type `Everyone` that represents all the users in the tenant.</span></span>

![Пример списка управления доступом](./images/search-index-manage-items-acl.png)

<span data-ttu-id="33444-114">Значение accessType `deny` имеет приоритет над `grant`.</span><span class="sxs-lookup"><span data-stu-id="33444-114">The accessType value `deny` takes precedence over `grant`.</span></span> <span data-ttu-id="33444-115">Например, хотя в приведенном выше элементе доступ предоставлен с помощью параметра `Everyone`, а конкретному пользователю доступ запрещен, действующим разрешением для этого пользователя будет вариант `deny`.</span><span class="sxs-lookup"><span data-stu-id="33444-115">For example, in the item shown above, while `Everyone` is granted access and a specific user is denied access, the effective permission for this user is `deny`.</span></span>

<span data-ttu-id="33444-116">Если ваш источник данных не содержит групп Azure Active Directory, таких как группы в вашей службе поддержки, применяемых для настройки разрешений для элемента, вы можете создать внешние группы в Microsoft Graph, используя API синхронизации группы для репликации разрешений `allow` или `deny`.</span><span class="sxs-lookup"><span data-stu-id="33444-116">If your data source has non Azure Active Directory groups, such as teams within your helpdesk system, used to set permissions for the item, you can create external groups in Microsoft Graph using the group sync APIs to replicate the `allow` or `deny` permissions.</span></span> <span data-ttu-id="33444-117">Избегайте расширения участия ваших внешних групп непосредственно в списках управления доступом отдельных элементов, так как каждое обновление участия группы может привести к многочисленным обновлениям элементов.</span><span class="sxs-lookup"><span data-stu-id="33444-117">Avoid expanding the membership of your external groups directly into the access control lists of individual items since each group membership update could lead to a storm of item updates.</span></span>

<span data-ttu-id="33444-118">Внешние группы могут состоять из других внешних групп, пользователей Azure Active Directory и групп Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="33444-118">External groups can consist of another external group, Azure Active Directory users, and Azure Active Directory groups.</span></span> <span data-ttu-id="33444-119">Если у вас есть пользователи не из Azure Active Directory, вы должны преобразовать их в пользователей Azure Active Directory в своем списке управления доступом.</span><span class="sxs-lookup"><span data-stu-id="33444-119">If you have non-Azure Active Directory users, you must translate them to Azure Active Directory users in your access control list.</span></span>

## <a name="properties"></a><span data-ttu-id="33444-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="33444-120">Properties</span></span>

<span data-ttu-id="33444-121">С помощью компонента свойств можно добавлять метаданные элементов, которые удобно применять в интерфейсах Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="33444-121">The properties component is used to add item metadata that is useful in Microsoft Graph experiences.</span></span> <span data-ttu-id="33444-122">Вы должны [зарегистрировать схему](./search-index-manage-schema.md) для связи перед добавлением в нее элементов и преобразованием типов данных в [поддерживаемые типы данных](/graph/api/resources/property?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="33444-122">You must [register the schema](./search-index-manage-schema.md) for the connection before adding items into it and convert datatypes into [supported datatypes](/graph/api/resources/property?view=graph-rest-beta&preserve-view=true).</span></span>

![Пример компонента свойства](./images/search-index-manage-items-1.png)

## <a name="content"></a><span data-ttu-id="33444-124">Содержимое</span><span class="sxs-lookup"><span data-stu-id="33444-124">Content</span></span>

<span data-ttu-id="33444-125">Компонент содержимого используется для массового добавления элементов, которые должны быть полнотекстовым индексом.</span><span class="sxs-lookup"><span data-stu-id="33444-125">The content component is used to add the bulk of the item that needs to be full text indexed.</span></span> <span data-ttu-id="33444-126">Примеры включают описание запроса, проанализированный текст из файла или вики-страницы.</span><span class="sxs-lookup"><span data-stu-id="33444-126">Examples include ticket description, parsed text from a file body, or a wiki page body.</span></span>

<span data-ttu-id="33444-127">Содержимое — одно из ключевых полей, влияющих на [релевантность](./search-index-manage-schema.md#relevance) в интерфейсах Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="33444-127">Content is one of the key fields influencing [relevance](./search-index-manage-schema.md#relevance) across Microsoft experiences.</span></span> <span data-ttu-id="33444-128">Мы поддерживаем содержимое типа `text` и `HTML`.</span><span class="sxs-lookup"><span data-stu-id="33444-128">We support content of the type `text` and `HTML`.</span></span> <span data-ttu-id="33444-129">Если источник данных содержит двоичные файлы, вы можете проанализировать их в качестве текста перед добавлением в Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="33444-129">If your data source has binary files, you can parse them to text before adding them to Microsoft Graph.</span></span>

![Пример компонента содержимого](./images/search-index-manage-items-2.png)

<span data-ttu-id="33444-131">Содержимое нельзя непосредственно добавить в шаблон результатов поиска, но вы можете использовать созданный фрагмент результатов, являющийся динамически создаваемым предварительным просмотром соответствующих разделов в содержимом.</span><span class="sxs-lookup"><span data-stu-id="33444-131">Content cannot be directly added into a search result template, but you can use a generated result snippet which is a dynamically generated preview of the relevant sections within content.</span></span>

![Снимок экрана с шаблоном результатов поиска](./images/search-index-manage-items-3.svg)

<span data-ttu-id="33444-133">При изменении содержимого в источнике данных вы должны синхронизировать его с элементами связи.</span><span class="sxs-lookup"><span data-stu-id="33444-133">When content in your data source changes, you must sync it with your connection items.</span></span> <span data-ttu-id="33444-134">Вы можете обновить весь элемент или обновить один или несколько его компонентов.</span><span class="sxs-lookup"><span data-stu-id="33444-134">You can either update the entire item or update one or more of its components.</span></span> <span data-ttu-id="33444-135">После добавления содержимого в Microsoft Graph вы можете искать его с помощью интерфейса Поиска (Майкрософт), настроив [вертикали и типы результатов](/MicrosoftSearch/customize-search-page) или воспользовавшись [API поиска Microsoft Graph](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="33444-135">Once your content has been added to Microsoft Graph, you can search for it through the Microsoft Search experience after setting up [verticals and result types](/MicrosoftSearch/customize-search-page) or using the [Microsoft Graph Search API](/graph/api/resources/search-api-overview?view=graph-rest-beta&preserve-view=true).</span></span>

## <a name="add-an-item"></a><span data-ttu-id="33444-136">Добавление элемента</span><span class="sxs-lookup"><span data-stu-id="33444-136">Add an item</span></span>

<span data-ttu-id="33444-137">Вы можете добавить элемент в индекс, [создав объект externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="33444-137">You can add an item to the index by [creating an externalItem](/graph/api/externalconnection-put-items?view=graph-rest-beta&preserve-view=true).</span></span> <span data-ttu-id="33444-138">При создании элемента ему назначается уникальный идентификатор в URL-адресе.</span><span class="sxs-lookup"><span data-stu-id="33444-138">When you create an item, you assign a unique identifier in the URL.</span></span>

<span data-ttu-id="33444-139">Например, приложение может индексировать запросы в службу технической поддержки по их номерам.</span><span class="sxs-lookup"><span data-stu-id="33444-139">For example, your application may index helpdesk tickets using the ticket number.</span></span> <span data-ttu-id="33444-140">Если запросу назначен номер `SR00145`, он может выглядеть так:</span><span class="sxs-lookup"><span data-stu-id="33444-140">If a ticket has the ticket number `SR00145`, the request may look like the following.</span></span>

```http
PUT /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "title": "WiFi outage in Conference Room A",
  "status": "New",
  "assignee": "meganb@contoso.com"
}
```

> <span data-ttu-id="33444-141">![ПРИМЕЧАНИЕ] Перед поиском индексированных элементов в пользовательском интерфейсе "Поиск (Майкрософт)", администратор должен [настроить страницу результатов поиска](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page) для соответствующего подключения.</span><span class="sxs-lookup"><span data-stu-id="33444-141">![NOTE] Before indexed items can be found in the Microsoft Search UI, an administrator must [customize the search results page](/MicrosoftSearch/configure-connector#next-steps-customize-the-search-results-page) for the corresponding connection.</span></span>

## <a name="update-an-item"></a><span data-ttu-id="33444-142">Обновление элемента</span><span class="sxs-lookup"><span data-stu-id="33444-142">Update an item</span></span>

<span data-ttu-id="33444-143">При обновлении элемента во внешней службе (переназначении запросов в службу технической поддержки или обновлении описания продукта), вы можете обновить соответствующую запись в индексе, [обновив externalItem](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true) по уникальному идентификатору, назначенному элементу при его создании.</span><span class="sxs-lookup"><span data-stu-id="33444-143">When an item is updated in the external service (helpdesk ticket is reassigned, or a product description is updated), you can update its entry in the index by [updating the externalItem](/graph/api/externalitem-update?view=graph-rest-beta&preserve-view=true), using the unique identifier assigned to the item when you created it.</span></span>

```http
PATCH /external/connections/contosohelpdesk/items/SR00145
Content-Type: application/json

{
  "assignee": "alexw@contoso.com"
}
```

## <a name="delete-an-item"></a><span data-ttu-id="33444-144">Удаление элемента</span><span class="sxs-lookup"><span data-stu-id="33444-144">Delete an item</span></span>

<span data-ttu-id="33444-145">Вы можете удалить элементы из индекса, [удалив externalItem](/graph/api/externalitem-delete?view=graph-rest-beta&preserve-view=true) по уникальному идентификатору, назначенному при его создании.</span><span class="sxs-lookup"><span data-stu-id="33444-145">You can remove items from the index by [deleting the externalItem](/graph/api/externalitem-delete?view=graph-rest-beta&preserve-view=true), using the unique identifier assigned to the item when you created it.</span></span>

```http
DELETE /external/connections/contosohelpdesk/items/SR00145
```

## <a name="next-steps"></a><span data-ttu-id="33444-146">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="33444-146">Next steps</span></span>

- [<span data-ttu-id="33444-147">Запросы с использованием API Поиска (Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33444-147">Query using the Microsoft Search API</span></span>](search-concept-overview.md#why-use-the-microsoft-search-api)
- [<span data-ttu-id="33444-148">Обзор индексирования справочных материалов по API</span><span class="sxs-lookup"><span data-stu-id="33444-148">Review the Indexing API reference</span></span>](/graph/api/resources/indexing-api-overview?view=graph-rest-beta&preserve-view=true)
- [<span data-ttu-id="33444-149">Настройка страницы результатов поиска Microsoft</span><span class="sxs-lookup"><span data-stu-id="33444-149">Customize Microsoft Search results page</span></span>](/MicrosoftSearch/customize-search-page)
- [<span data-ttu-id="33444-150">Поиск объектов настраиваемого типа (externalItem)</span><span class="sxs-lookup"><span data-stu-id="33444-150">Search custom types (externalItem)</span></span>](search-concept-custom-types.md)
- <span data-ttu-id="33444-151">Скачайте [образец соединителя поиска](https://github.com/microsoftgraph/msgraph-search-connector-sample) с сайта GitHub.</span><span class="sxs-lookup"><span data-stu-id="33444-151">Download the [sample search connector](https://github.com/microsoftgraph/msgraph-search-connector-sample) from GitHub</span></span>