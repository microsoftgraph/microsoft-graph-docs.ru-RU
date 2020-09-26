---
title: Выполнение вызовов API с помощью пакетов SDK Microsoft Graph
description: Содержит инструкции по созданию HTTP-запросов Microsoft Graph с помощью пакетов SDK.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: 1338cbe7411a3643eaa5c1e1e58cf8d5b9b47c0a
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288335"
---
# <a name="make-api-calls-using-the-microsoft-graph-sdks"></a><span data-ttu-id="bd378-103">Выполнение вызовов API с помощью пакетов SDK Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bd378-103">Make API calls using the Microsoft Graph SDKs</span></span>

<span data-ttu-id="bd378-104">Библиотеки службы SDK Microsoft Graph предоставляют клиентский класс, который можно использовать в качестве отправной точки для создания всех запросов API.</span><span class="sxs-lookup"><span data-stu-id="bd378-104">The Microsoft Graph SDK service libraries provide a client class that you can use as the starting point for creating all API requests.</span></span> <span data-ttu-id="bd378-105">Существует два стиля клиентского класса: один использует интерфейс Fluent для создания запроса (например, `client.Users["user-id"].Manager` ), а другой принимает строку пути (например, `api("/users/user-id/manager")` ).</span><span class="sxs-lookup"><span data-stu-id="bd378-105">There are two styles of client class: one uses a fluent interface to create the request (for example, `client.Users["user-id"].Manager`) and the other accepts a path string (for example, `api("/users/user-id/manager")`).</span></span> <span data-ttu-id="bd378-106">Когда у вас есть объект Request, вы можете указать различные параметры, такие как фильтрация и сортировка, и, наконец, выбрать тип операции, которую необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="bd378-106">When you have a request object, you can specify a variety of options such as filtering and sorting, and finally, you select the type of operation you want to perform.</span></span>

<span data-ttu-id="bd378-107">Кроме того, существует [пакет SDK Microsoft Graph PowerShell](../powershell/get-started.md), в котором нет клиентского класса.</span><span class="sxs-lookup"><span data-stu-id="bd378-107">There is also the [Microsoft Graph PowerShell SDK](../powershell/get-started.md), which has no client class at all.</span></span> <span data-ttu-id="bd378-108">Вместо этого все запросы представлены в виде команд PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bd378-108">Instead, all requests are represented as PowerShell commands.</span></span> <span data-ttu-id="bd378-109">Например, для получения сведений о руководителе пользователя используется команда `Get-MgUserManager` .</span><span class="sxs-lookup"><span data-stu-id="bd378-109">For example, to get a user's manager, the command is `Get-MgUserManager`.</span></span> <span data-ttu-id="bd378-110">Дополнительные сведения о поиске команд для вызовов API приведены [в статье Навигация по пакету SDK для Microsoft Graph PowerShell](../powershell/navigating.md).</span><span class="sxs-lookup"><span data-stu-id="bd378-110">For more information on finding commands for API calls, see [Navigating the Microsoft Graph PowerShell SDK](../powershell/navigating.md).</span></span>

## <a name="read-information-from-microsoft-graph"></a><span data-ttu-id="bd378-111">Чтение информации из Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="bd378-111">Read information from Microsoft Graph</span></span>

<span data-ttu-id="bd378-112">Чтобы прочитать данные из Microsoft Graph, сначала необходимо создать объект Request, а затем выполнить `GET` метод для запроса.</span><span class="sxs-lookup"><span data-stu-id="bd378-112">To read information from Microsoft Graph, you first need to create a request object and then run the `GET` method on the request.</span></span>

# <a name="c"></a>[<span data-ttu-id="bd378-113">C#</span><span class="sxs-lookup"><span data-stu-id="bd378-113">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-read.md)]

# <a name="typescript"></a>[<span data-ttu-id="bd378-114">TypeScript</span><span class="sxs-lookup"><span data-stu-id="bd378-114">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-read.md)]

# <a name="java"></a>[<span data-ttu-id="bd378-115">Java</span><span class="sxs-lookup"><span data-stu-id="bd378-115">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-read.md)]

# <a name="powershell"></a>[<span data-ttu-id="bd378-116">PowerShell</span><span class="sxs-lookup"><span data-stu-id="bd378-116">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-read.md)]

---

## <a name="use-select-to-control-the-properties-returned"></a><span data-ttu-id="bd378-117">Использование $select для управления возвращаемыми свойствами</span><span class="sxs-lookup"><span data-stu-id="bd378-117">Use $select to control the properties returned</span></span>

<span data-ttu-id="bd378-118">При получении объекта автоматически извлекаются не все свойства; Иногда они должны быть явно выбраны.</span><span class="sxs-lookup"><span data-stu-id="bd378-118">When retrieving an entity, not all properties are automatically retrieved; sometimes they need to be explicitly selected.</span></span> <span data-ttu-id="bd378-119">Кроме того, в некоторых случаях не требуется возвращать набор свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bd378-119">Also, in some scenarios it isn't necessary to return the default set of properties.</span></span> <span data-ttu-id="bd378-120">Выбор только обязательных свойств может увеличить производительность запроса.</span><span class="sxs-lookup"><span data-stu-id="bd378-120">Selecting just the required properties can improve the performance of the request.</span></span> <span data-ttu-id="bd378-121">Вы можете настроить запрос на включение `$select` параметра запроса в список свойств.</span><span class="sxs-lookup"><span data-stu-id="bd378-121">You can customize the request to include the `$select` query parameter with a list of properties.</span></span>

<!-- markdownlint-disable MD024 -->
# <a name="c"></a>[<span data-ttu-id="bd378-122">C#</span><span class="sxs-lookup"><span data-stu-id="bd378-122">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-select.md)]

# <a name="typescript"></a>[<span data-ttu-id="bd378-123">TypeScript</span><span class="sxs-lookup"><span data-stu-id="bd378-123">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-select.md)]

# <a name="java"></a>[<span data-ttu-id="bd378-124">Java</span><span class="sxs-lookup"><span data-stu-id="bd378-124">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-select.md)]

# <a name="powershell"></a>[<span data-ttu-id="bd378-125">PowerShell</span><span class="sxs-lookup"><span data-stu-id="bd378-125">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-select.md)]

---

## <a name="retrieve-a-list-of-entities"></a><span data-ttu-id="bd378-126">Получение списка объектов</span><span class="sxs-lookup"><span data-stu-id="bd378-126">Retrieve a list of entities</span></span>

<span data-ttu-id="bd378-127">Получение списка сущностей аналогично получению одного объекта, за исключением ряда других вариантов настройки запроса.</span><span class="sxs-lookup"><span data-stu-id="bd378-127">Retrieving a list of entities is similar to retrieving a single entity except there a number of other options for configuring the request.</span></span> <span data-ttu-id="bd378-128">`$filter`Параметр Query можно использовать, чтобы уменьшить набор результатов до тех строк, которые соответствуют заданному условию.</span><span class="sxs-lookup"><span data-stu-id="bd378-128">The `$filter` query parameter can be used to reduce the result set to only those rows that match the provided condition.</span></span>  <span data-ttu-id="bd378-129">`$orderBy`Параметр запроса будет запрашивать, чтобы сервер предоставил список сущностей, отсортированных по указанным свойствам.</span><span class="sxs-lookup"><span data-stu-id="bd378-129">The `$orderBy` query parameter will request that the server provide the list of entities sorted by the specified properties.</span></span>

# <a name="c"></a>[<span data-ttu-id="bd378-130">C#</span><span class="sxs-lookup"><span data-stu-id="bd378-130">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-list.md)]

# <a name="typescript"></a>[<span data-ttu-id="bd378-131">TypeScript</span><span class="sxs-lookup"><span data-stu-id="bd378-131">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-list.md)]

# <a name="java"></a>[<span data-ttu-id="bd378-132">Java</span><span class="sxs-lookup"><span data-stu-id="bd378-132">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-list.md)]

# <a name="powershell"></a>[<span data-ttu-id="bd378-133">PowerShell</span><span class="sxs-lookup"><span data-stu-id="bd378-133">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-list.md)]

---

<span data-ttu-id="bd378-134">Объект, возвращаемый при получении списка сущностей, скорее всего, является страничной коллекцией.</span><span class="sxs-lookup"><span data-stu-id="bd378-134">The object returned when retrieving a list of entities is likely to be a paged collection.</span></span> <span data-ttu-id="bd378-135">Сведения о том, как получить полный список сущностей, можно найти в разделе [paging a Collection](../paging.md).</span><span class="sxs-lookup"><span data-stu-id="bd378-135">For details about how to get the complete list of entities, see [paging through a collection](../paging.md).</span></span>

## <a name="access-an-item-of-a-collection"></a><span data-ttu-id="bd378-136">Доступ к элементу коллекции</span><span class="sxs-lookup"><span data-stu-id="bd378-136">Access an item of a collection</span></span>

<span data-ttu-id="bd378-137">Для пакетов SDK, поддерживающих стиль Fluent, доступ к коллекциям сущностей можно получить с помощью индекса массива.</span><span class="sxs-lookup"><span data-stu-id="bd378-137">For SDKs that support a fluent style, collections of entities can be accessed using an array index.</span></span> <span data-ttu-id="bd378-138">Для пакетов SDK на основе шаблонов достаточно внедрить идентификатор элемента в сегмент пути, следующий за коллекцией.</span><span class="sxs-lookup"><span data-stu-id="bd378-138">For template-based SDKs, it is sufficient to embed the item identifier in the path segment following the collection.</span></span> <span data-ttu-id="bd378-139">Для PowerShell идентификаторы передаются в качестве параметров.</span><span class="sxs-lookup"><span data-stu-id="bd378-139">For PowerShell, identifiers are passed as parameters.</span></span>

# <a name="c"></a>[<span data-ttu-id="bd378-140">C#</span><span class="sxs-lookup"><span data-stu-id="bd378-140">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-index.md)]

# <a name="typescript"></a>[<span data-ttu-id="bd378-141">TypeScript</span><span class="sxs-lookup"><span data-stu-id="bd378-141">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-index.md)]

# <a name="java"></a>[<span data-ttu-id="bd378-142">Java</span><span class="sxs-lookup"><span data-stu-id="bd378-142">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-index.md)]

# <a name="powershell"></a>[<span data-ttu-id="bd378-143">PowerShell</span><span class="sxs-lookup"><span data-stu-id="bd378-143">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-index.md)]

---

## <a name="use-expand-to-access-related-entities"></a><span data-ttu-id="bd378-144">Использование $expand для доступа к связанным сущностям</span><span class="sxs-lookup"><span data-stu-id="bd378-144">Use $expand to access related entities</span></span>

<span data-ttu-id="bd378-145">С помощью фильтра можно `$expand` запрашивать связанную сущность или коллекцию сущностей, которые запрашивают основной объект.</span><span class="sxs-lookup"><span data-stu-id="bd378-145">You can use the `$expand` filter to request a related entity, or collection of entities, at the same that you request the main entity.</span></span>

# <a name="c"></a>[<span data-ttu-id="bd378-146">C#</span><span class="sxs-lookup"><span data-stu-id="bd378-146">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-expand.md)]

# <a name="typescript"></a>[<span data-ttu-id="bd378-147">TypeScript</span><span class="sxs-lookup"><span data-stu-id="bd378-147">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-expand.md)]

# <a name="java"></a>[<span data-ttu-id="bd378-148">Java</span><span class="sxs-lookup"><span data-stu-id="bd378-148">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-expand.md)]

# <a name="powershell"></a>[<span data-ttu-id="bd378-149">PowerShell</span><span class="sxs-lookup"><span data-stu-id="bd378-149">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-expand.md)]

---

## <a name="delete-an-entity"></a><span data-ttu-id="bd378-150">Удаление объекта</span><span class="sxs-lookup"><span data-stu-id="bd378-150">Delete an entity</span></span>

<span data-ttu-id="bd378-151">Запросы DELETE создаются так же, как запросы на получение объекта, но `DELETE` вместо него используется запрос `GET` .</span><span class="sxs-lookup"><span data-stu-id="bd378-151">Delete requests are constructed in the same way as requests to retrieve an entity, but use a `DELETE` request instead of a `GET`.</span></span>

# <a name="c"></a>[<span data-ttu-id="bd378-152">C#</span><span class="sxs-lookup"><span data-stu-id="bd378-152">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-delete.md)]

# <a name="typescript"></a>[<span data-ttu-id="bd378-153">TypeScript</span><span class="sxs-lookup"><span data-stu-id="bd378-153">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-delete.md)]

# <a name="java"></a>[<span data-ttu-id="bd378-154">Java</span><span class="sxs-lookup"><span data-stu-id="bd378-154">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-delete.md)]

# <a name="powershell"></a>[<span data-ttu-id="bd378-155">PowerShell</span><span class="sxs-lookup"><span data-stu-id="bd378-155">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-delete.md)]

---

## <a name="make-a-post-request-to-create-a-new-entity"></a><span data-ttu-id="bd378-156">Создание запроса POST для создания нового объекта</span><span class="sxs-lookup"><span data-stu-id="bd378-156">Make a POST request to create a new entity</span></span>

<span data-ttu-id="bd378-157">Для пакетов SDK, поддерживающих стиль Fluent, новые элементы можно добавлять в коллекции с помощью `Add` метода.</span><span class="sxs-lookup"><span data-stu-id="bd378-157">For SDKs that support a fluent style, new items can be added to collections with an `Add` method.</span></span> <span data-ttu-id="bd378-158">В пакетах SDK на основе шаблонов объект Request предоставляет `post` метод.</span><span class="sxs-lookup"><span data-stu-id="bd378-158">For template-based SDKs, the request object exposes a `post` method.</span></span> <span data-ttu-id="bd378-159">Для PowerShell `New-*` доступна команда, принимающая параметры, сопоставленные с добавляемой сущностью.</span><span class="sxs-lookup"><span data-stu-id="bd378-159">For PowerShell, a `New-*` command is available that accepts parameters that map to the entity to add.</span></span> <span data-ttu-id="bd378-160">Созданная сущность обычно возвращается из вызова.</span><span class="sxs-lookup"><span data-stu-id="bd378-160">The created entity is usually returned from the call.</span></span>

# <a name="c"></a>[<span data-ttu-id="bd378-161">C#</span><span class="sxs-lookup"><span data-stu-id="bd378-161">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-create.md)]

# <a name="typescript"></a>[<span data-ttu-id="bd378-162">TypeScript</span><span class="sxs-lookup"><span data-stu-id="bd378-162">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-create.md)]

# <a name="java"></a>[<span data-ttu-id="bd378-163">Java</span><span class="sxs-lookup"><span data-stu-id="bd378-163">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-create.md)]

# <a name="powershell"></a>[<span data-ttu-id="bd378-164">PowerShell</span><span class="sxs-lookup"><span data-stu-id="bd378-164">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-create.md)]

---

## <a name="updating-an-existing-entity-with-patch"></a><span data-ttu-id="bd378-165">Обновление существующей сущности с помощью исправления</span><span class="sxs-lookup"><span data-stu-id="bd378-165">Updating an existing entity with PATCH</span></span>

<span data-ttu-id="bd378-166">Большинство обновлений в Microsoft Graph выполняются с помощью `PATCH` метода, поэтому необходимо включить в передаваемый объект только те свойства, которые нужно изменить.</span><span class="sxs-lookup"><span data-stu-id="bd378-166">Most updates in Microsoft Graph are performed using a `PATCH` method and therefore it is only necessary to include the properties that you want to change in the object you pass.</span></span>

# <a name="c"></a>[<span data-ttu-id="bd378-167">C#</span><span class="sxs-lookup"><span data-stu-id="bd378-167">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-update.md)]

# <a name="typescript"></a>[<span data-ttu-id="bd378-168">TypeScript</span><span class="sxs-lookup"><span data-stu-id="bd378-168">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-update.md)]

# <a name="java"></a>[<span data-ttu-id="bd378-169">Java</span><span class="sxs-lookup"><span data-stu-id="bd378-169">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-update.md)]

# <a name="powershell"></a>[<span data-ttu-id="bd378-170">PowerShell</span><span class="sxs-lookup"><span data-stu-id="bd378-170">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-update.md)]

---

## <a name="use-http-headers-to-control-request-behavior"></a><span data-ttu-id="bd378-171">Использование заголовков HTTP для управления поведением запроса</span><span class="sxs-lookup"><span data-stu-id="bd378-171">Use HTTP headers to control request behavior</span></span>

<span data-ttu-id="bd378-172">Вы можете использовать `Header()` функцию для присоединения пользовательских заголовков к запросу.</span><span class="sxs-lookup"><span data-stu-id="bd378-172">You can use a `Header()` function to attach custom headers to a request.</span></span> <span data-ttu-id="bd378-173">Для PowerShell Добавление заголовков возможно только в `Invoke-GraphRequest` методе.</span><span class="sxs-lookup"><span data-stu-id="bd378-173">For PowerShell, adding headers is only possible with the `Invoke-GraphRequest` method.</span></span> <span data-ttu-id="bd378-174">В некоторых сценариях Microsoft Graph для настройки поведения запроса используются настраиваемые заголовки.</span><span class="sxs-lookup"><span data-stu-id="bd378-174">A number of Microsoft Graph scenarios use custom headers to adjust the behavior of the request.</span></span>

# <a name="c"></a>[<span data-ttu-id="bd378-175">C#</span><span class="sxs-lookup"><span data-stu-id="bd378-175">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-headers.md)]

# <a name="typescript"></a>[<span data-ttu-id="bd378-176">TypeScript</span><span class="sxs-lookup"><span data-stu-id="bd378-176">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-headers.md)]

# <a name="java"></a>[<span data-ttu-id="bd378-177">Java</span><span class="sxs-lookup"><span data-stu-id="bd378-177">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-headers.md)]

# <a name="powershell"></a>[<span data-ttu-id="bd378-178">PowerShell</span><span class="sxs-lookup"><span data-stu-id="bd378-178">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-headers.md)]

---

## <a name="provide-custom-query-parameters"></a><span data-ttu-id="bd378-179">Предоставление настраиваемых параметров запроса</span><span class="sxs-lookup"><span data-stu-id="bd378-179">Provide custom query parameters</span></span>

<span data-ttu-id="bd378-180">Для пакетов SDK, поддерживающих стиль Fluent, можно указать настраиваемые значения параметров запроса с помощью списка `QueryOptions` объектов.</span><span class="sxs-lookup"><span data-stu-id="bd378-180">For SDKs that support a fluent style, you can provide custom query parameter values by using a list of `QueryOptions` objects.</span></span> <span data-ttu-id="bd378-181">Для пакетов SDK на основе шаблонов параметры кодируются в URL-адресе и добавляются в URI запроса.</span><span class="sxs-lookup"><span data-stu-id="bd378-181">For template-based SDKs, the parameters are URL-encoded and added to the request URI.</span></span> <span data-ttu-id="bd378-182">Для PowerShell определенные параметры запроса для данного API предоставляются в виде параметров для соответствующей команды.</span><span class="sxs-lookup"><span data-stu-id="bd378-182">For PowerShell, defined query parameters for a given API are exposed as parameters to the corresponding command.</span></span>

# <a name="c"></a>[<span data-ttu-id="bd378-183">C#</span><span class="sxs-lookup"><span data-stu-id="bd378-183">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-queryparams.md)]

# <a name="typescript"></a>[<span data-ttu-id="bd378-184">TypeScript</span><span class="sxs-lookup"><span data-stu-id="bd378-184">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-queryparams.md)]

# <a name="java"></a>[<span data-ttu-id="bd378-185">Java</span><span class="sxs-lookup"><span data-stu-id="bd378-185">Java</span></span>](#tab/java)

[!INCLUDE [sample-code](includes/snippets/java/create-requests-queryparams.md)]

# <a name="powershell"></a>[<span data-ttu-id="bd378-186">PowerShell</span><span class="sxs-lookup"><span data-stu-id="bd378-186">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-queryparams.md)]

---
