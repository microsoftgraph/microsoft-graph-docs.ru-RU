---
title: Выполнение вызовов API с помощью пакетов SDK Microsoft Graph
description: Содержит инструкции по созданию HTTP-запросов Microsoft Graph с помощью пакетов SDK.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: f317b52393378231fb57f2c39c9b9701a9215cf4
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193025"
---
# <a name="make-api-calls-using-the-microsoft-graph-sdks"></a><span data-ttu-id="18a8f-103">Выполнение вызовов API с помощью пакетов SDK Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="18a8f-103">Make API calls using the Microsoft Graph SDKs</span></span>

<span data-ttu-id="18a8f-104">Библиотеки службы SDK Microsoft Graph предоставляют клиентский класс, который можно использовать в качестве отправной точки для создания всех запросов API.</span><span class="sxs-lookup"><span data-stu-id="18a8f-104">The Microsoft Graph SDK service libraries provide a client class that you can use as the starting point for creating all API requests.</span></span> <span data-ttu-id="18a8f-105">Существует два стиля клиентского класса: один использует интерфейс Fluent для создания запроса (например, `client.Users["user-id"].Manager` ), а другой принимает строку пути (например, `api("/users/user-id/manager")` ).</span><span class="sxs-lookup"><span data-stu-id="18a8f-105">There are two styles of client class: one uses a fluent interface to create the request (for example, `client.Users["user-id"].Manager`) and the other accepts a path string (for example, `api("/users/user-id/manager")`).</span></span> <span data-ttu-id="18a8f-106">Когда у вас есть объект Request, вы можете указать различные параметры, такие как фильтрация и сортировка, и, наконец, выбрать тип операции, которую необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="18a8f-106">When you have a request object, you can specify a variety of options such as filtering and sorting, and finally, you select the type of operation you want to perform.</span></span>

<span data-ttu-id="18a8f-107">Кроме того, существует [пакет SDK Microsoft Graph PowerShell](../powershell/get-started.md), в котором нет клиентского класса.</span><span class="sxs-lookup"><span data-stu-id="18a8f-107">There is also the [Microsoft Graph PowerShell SDK](../powershell/get-started.md), which has no client class at all.</span></span> <span data-ttu-id="18a8f-108">Вместо этого все запросы представлены в виде команд PowerShell.</span><span class="sxs-lookup"><span data-stu-id="18a8f-108">Instead, all requests are represented as PowerShell commands.</span></span> <span data-ttu-id="18a8f-109">Например, для получения сведений о руководителе пользователя используется команда `Get-MgUserManager` .</span><span class="sxs-lookup"><span data-stu-id="18a8f-109">For example, to get a user's manager, the command is `Get-MgUserManager`.</span></span> <span data-ttu-id="18a8f-110">Дополнительные сведения о поиске команд для вызовов API приведены [в статье Навигация по пакету SDK для Microsoft Graph PowerShell](../powershell/navigating.md).</span><span class="sxs-lookup"><span data-stu-id="18a8f-110">For more information on finding commands for API calls, see [Navigating the Microsoft Graph PowerShell SDK](../powershell/navigating.md).</span></span>

## <a name="read-information-from-microsoft-graph"></a><span data-ttu-id="18a8f-111">Чтение информации из Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="18a8f-111">Read information from Microsoft Graph</span></span>

<span data-ttu-id="18a8f-112">Чтобы прочитать данные из Microsoft Graph, сначала необходимо создать объект Request, а затем выполнить `GET` метод для запроса.</span><span class="sxs-lookup"><span data-stu-id="18a8f-112">To read information from Microsoft Graph, you first need to create a request object and then run the `GET` method on the request.</span></span>

# <a name="c"></a>[<span data-ttu-id="18a8f-113">C#</span><span class="sxs-lookup"><span data-stu-id="18a8f-113">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-read.md)]

# <a name="typescript"></a>[<span data-ttu-id="18a8f-114">TypeScript</span><span class="sxs-lookup"><span data-stu-id="18a8f-114">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-read.md)]

# <a name="powershell"></a>[<span data-ttu-id="18a8f-115">PowerShell</span><span class="sxs-lookup"><span data-stu-id="18a8f-115">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-read.md)]

---

## <a name="use-select-to-control-the-properties-returned"></a><span data-ttu-id="18a8f-116">Использование $select для управления возвращаемыми свойствами</span><span class="sxs-lookup"><span data-stu-id="18a8f-116">Use $select to control the properties returned</span></span>

<span data-ttu-id="18a8f-117">При получении объекта автоматически извлекаются не все свойства; Иногда они должны быть явно выбраны.</span><span class="sxs-lookup"><span data-stu-id="18a8f-117">When retrieving an entity, not all properties are automatically retrieved; sometimes they need to be explicitly selected.</span></span> <span data-ttu-id="18a8f-118">Кроме того, в некоторых случаях не требуется возвращать набор свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="18a8f-118">Also, in some scenarios it isn't necessary to return the default set of properties.</span></span> <span data-ttu-id="18a8f-119">Выбор только обязательных свойств может увеличить производительность запроса.</span><span class="sxs-lookup"><span data-stu-id="18a8f-119">Selecting just the required properties can improve the performance of the request.</span></span> <span data-ttu-id="18a8f-120">Вы можете настроить запрос на включение `$select` параметра запроса в список свойств.</span><span class="sxs-lookup"><span data-stu-id="18a8f-120">You can customize the request to include the `$select` query parameter with a list of properties.</span></span>

<!-- markdownlint-disable MD024 -->
# <a name="c"></a>[<span data-ttu-id="18a8f-121">C#</span><span class="sxs-lookup"><span data-stu-id="18a8f-121">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-select.md)]

# <a name="typescript"></a>[<span data-ttu-id="18a8f-122">TypeScript</span><span class="sxs-lookup"><span data-stu-id="18a8f-122">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-select.md)]

# <a name="powershell"></a>[<span data-ttu-id="18a8f-123">PowerShell</span><span class="sxs-lookup"><span data-stu-id="18a8f-123">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-select.md)]

---

## <a name="retrieve-a-list-of-entities"></a><span data-ttu-id="18a8f-124">Получение списка объектов</span><span class="sxs-lookup"><span data-stu-id="18a8f-124">Retrieve a list of entities</span></span>

<span data-ttu-id="18a8f-125">Получение списка сущностей аналогично получению одного объекта, за исключением ряда других вариантов настройки запроса.</span><span class="sxs-lookup"><span data-stu-id="18a8f-125">Retrieving a list of entities is similar to retrieving a single entity except there a number of other options for configuring the request.</span></span> <span data-ttu-id="18a8f-126">`$filter`Параметр Query можно использовать, чтобы уменьшить набор результатов до тех строк, которые соответствуют заданному условию.</span><span class="sxs-lookup"><span data-stu-id="18a8f-126">The `$filter` query parameter can be used to reduce the result set to only those rows that match the provided condition.</span></span>  <span data-ttu-id="18a8f-127">`$orderBy`Параметр запроса будет запрашивать, чтобы сервер предоставил список сущностей, отсортированных по указанным свойствам.</span><span class="sxs-lookup"><span data-stu-id="18a8f-127">The `$orderBy` query parameter will request that the server provide the list of entities sorted by the specified properties.</span></span>

# <a name="c"></a>[<span data-ttu-id="18a8f-128">C#</span><span class="sxs-lookup"><span data-stu-id="18a8f-128">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-list.md)]

# <a name="typescript"></a>[<span data-ttu-id="18a8f-129">TypeScript</span><span class="sxs-lookup"><span data-stu-id="18a8f-129">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-list.md)]

# <a name="powershell"></a>[<span data-ttu-id="18a8f-130">PowerShell</span><span class="sxs-lookup"><span data-stu-id="18a8f-130">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-list.md)]

---

<span data-ttu-id="18a8f-131">Объект, возвращаемый при получении списка сущностей, скорее всего, является страничной коллекцией.</span><span class="sxs-lookup"><span data-stu-id="18a8f-131">The object returned when retrieving a list of entities is likely to be a paged collection.</span></span> <span data-ttu-id="18a8f-132">Сведения о том, как получить полный список сущностей, можно найти в разделе [paging a Collection](../paging.md).</span><span class="sxs-lookup"><span data-stu-id="18a8f-132">For details about how to get the complete list of entities, see [paging through a collection](../paging.md).</span></span>

## <a name="access-an-item-of-a-collection"></a><span data-ttu-id="18a8f-133">Доступ к элементу коллекции</span><span class="sxs-lookup"><span data-stu-id="18a8f-133">Access an item of a collection</span></span>

<span data-ttu-id="18a8f-134">Для пакетов SDK, поддерживающих стиль Fluent, доступ к коллекциям сущностей можно получить с помощью индекса массива.</span><span class="sxs-lookup"><span data-stu-id="18a8f-134">For SDKs that support a fluent style, collections of entities can be accessed using an array index.</span></span> <span data-ttu-id="18a8f-135">Для пакетов SDK на основе шаблонов достаточно внедрить идентификатор элемента в сегмент пути, следующий за коллекцией.</span><span class="sxs-lookup"><span data-stu-id="18a8f-135">For template-based SDKs, it is sufficient to embed the item identifier in the path segment following the collection.</span></span> <span data-ttu-id="18a8f-136">Для PowerShell идентификаторы передаются в качестве параметров.</span><span class="sxs-lookup"><span data-stu-id="18a8f-136">For PowerShell, identifiers are passed as parameters.</span></span>

# <a name="c"></a>[<span data-ttu-id="18a8f-137">C#</span><span class="sxs-lookup"><span data-stu-id="18a8f-137">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-index.md)]

# <a name="typescript"></a>[<span data-ttu-id="18a8f-138">TypeScript</span><span class="sxs-lookup"><span data-stu-id="18a8f-138">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-index.md)]

# <a name="powershell"></a>[<span data-ttu-id="18a8f-139">PowerShell</span><span class="sxs-lookup"><span data-stu-id="18a8f-139">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-index.md)]

---

## <a name="use-expand-to-access-related-entities"></a><span data-ttu-id="18a8f-140">Использование $expand для доступа к связанным сущностям</span><span class="sxs-lookup"><span data-stu-id="18a8f-140">Use $expand to access related entities</span></span>

<span data-ttu-id="18a8f-141">С помощью фильтра можно `$expand` запрашивать связанную сущность или коллекцию сущностей, которые запрашивают основной объект.</span><span class="sxs-lookup"><span data-stu-id="18a8f-141">You can use the `$expand` filter to request a related entity, or collection of entities, at the same that you request the main entity.</span></span>

# <a name="c"></a>[<span data-ttu-id="18a8f-142">C#</span><span class="sxs-lookup"><span data-stu-id="18a8f-142">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-expand.md)]

# <a name="typescript"></a>[<span data-ttu-id="18a8f-143">TypeScript</span><span class="sxs-lookup"><span data-stu-id="18a8f-143">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-expand.md)]

# <a name="powershell"></a>[<span data-ttu-id="18a8f-144">PowerShell</span><span class="sxs-lookup"><span data-stu-id="18a8f-144">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-expand.md)]

---

## <a name="delete-an-entity"></a><span data-ttu-id="18a8f-145">Удаление объекта</span><span class="sxs-lookup"><span data-stu-id="18a8f-145">Delete an entity</span></span>

<span data-ttu-id="18a8f-146">Запросы DELETE создаются так же, как запросы на получение объекта, но `DELETE` вместо него используется запрос `GET` .</span><span class="sxs-lookup"><span data-stu-id="18a8f-146">Delete requests are constructed in the same way as requests to retrieve an entity, but use a `DELETE` request instead of a `GET`.</span></span>

# <a name="c"></a>[<span data-ttu-id="18a8f-147">C#</span><span class="sxs-lookup"><span data-stu-id="18a8f-147">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-delete.md)]

# <a name="typescript"></a>[<span data-ttu-id="18a8f-148">TypeScript</span><span class="sxs-lookup"><span data-stu-id="18a8f-148">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-delete.md)]

# <a name="powershell"></a>[<span data-ttu-id="18a8f-149">PowerShell</span><span class="sxs-lookup"><span data-stu-id="18a8f-149">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-delete.md)]

---

## <a name="make-a-post-request-to-create-a-new-entity"></a><span data-ttu-id="18a8f-150">Создание запроса POST для создания нового объекта</span><span class="sxs-lookup"><span data-stu-id="18a8f-150">Make a POST request to create a new entity</span></span>

<span data-ttu-id="18a8f-151">Для пакетов SDK, поддерживающих стиль Fluent, новые элементы можно добавлять в коллекции с помощью `Add` метода.</span><span class="sxs-lookup"><span data-stu-id="18a8f-151">For SDKs that support a fluent style, new items can be added to collections with an `Add` method.</span></span> <span data-ttu-id="18a8f-152">В пакетах SDK на основе шаблонов объект Request предоставляет `post` метод.</span><span class="sxs-lookup"><span data-stu-id="18a8f-152">For template-based SDKs, the request object exposes a `post` method.</span></span> <span data-ttu-id="18a8f-153">Для PowerShell `New-*` доступна команда, принимающая параметры, сопоставленные с добавляемой сущностью.</span><span class="sxs-lookup"><span data-stu-id="18a8f-153">For PowerShell, a `New-*` command is available that accepts parameters that map to the entity to add.</span></span> <span data-ttu-id="18a8f-154">Созданная сущность обычно возвращается из вызова.</span><span class="sxs-lookup"><span data-stu-id="18a8f-154">The created entity is usually returned from the call.</span></span>

# <a name="c"></a>[<span data-ttu-id="18a8f-155">C#</span><span class="sxs-lookup"><span data-stu-id="18a8f-155">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-create.md)]

# <a name="typescript"></a>[<span data-ttu-id="18a8f-156">TypeScript</span><span class="sxs-lookup"><span data-stu-id="18a8f-156">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-create.md)]

# <a name="powershell"></a>[<span data-ttu-id="18a8f-157">PowerShell</span><span class="sxs-lookup"><span data-stu-id="18a8f-157">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-create.md)]

---

## <a name="updating-an-existing-entity-with-patch"></a><span data-ttu-id="18a8f-158">Обновление существующей сущности с помощью исправления</span><span class="sxs-lookup"><span data-stu-id="18a8f-158">Updating an existing entity with PATCH</span></span>

<span data-ttu-id="18a8f-159">Большинство обновлений в Microsoft Graph выполняются с помощью `PATCH` метода, поэтому необходимо включить в передаваемый объект только те свойства, которые нужно изменить.</span><span class="sxs-lookup"><span data-stu-id="18a8f-159">Most updates in Microsoft Graph are performed using a `PATCH` method and therefore it is only necessary to include the properties that you want to change in the object you pass.</span></span>

# <a name="c"></a>[<span data-ttu-id="18a8f-160">C#</span><span class="sxs-lookup"><span data-stu-id="18a8f-160">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-update.md)]

# <a name="typescript"></a>[<span data-ttu-id="18a8f-161">TypeScript</span><span class="sxs-lookup"><span data-stu-id="18a8f-161">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-update.md)]

# <a name="powershell"></a>[<span data-ttu-id="18a8f-162">PowerShell</span><span class="sxs-lookup"><span data-stu-id="18a8f-162">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-update.md)]

---

## <a name="use-http-headers-to-control-request-behavior"></a><span data-ttu-id="18a8f-163">Использование заголовков HTTP для управления поведением запроса</span><span class="sxs-lookup"><span data-stu-id="18a8f-163">Use HTTP headers to control request behavior</span></span>

<span data-ttu-id="18a8f-164">Вы можете использовать `Header()` функцию для присоединения пользовательских заголовков к запросу.</span><span class="sxs-lookup"><span data-stu-id="18a8f-164">You can use a `Header()` function to attach custom headers to a request.</span></span> <span data-ttu-id="18a8f-165">Для PowerShell Добавление заголовков возможно только в `Invoke-GraphRequest` методе.</span><span class="sxs-lookup"><span data-stu-id="18a8f-165">For PowerShell, adding headers is only possible with the `Invoke-GraphRequest` method.</span></span> <span data-ttu-id="18a8f-166">В некоторых сценариях Microsoft Graph для настройки поведения запроса используются настраиваемые заголовки.</span><span class="sxs-lookup"><span data-stu-id="18a8f-166">A number of Microsoft Graph scenarios use custom headers to adjust the behavior of the request.</span></span>

# <a name="c"></a>[<span data-ttu-id="18a8f-167">C#</span><span class="sxs-lookup"><span data-stu-id="18a8f-167">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-headers.md)]

# <a name="typescript"></a>[<span data-ttu-id="18a8f-168">TypeScript</span><span class="sxs-lookup"><span data-stu-id="18a8f-168">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-headers.md)]

# <a name="powershell"></a>[<span data-ttu-id="18a8f-169">PowerShell</span><span class="sxs-lookup"><span data-stu-id="18a8f-169">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-headers.md)]

---

## <a name="provide-custom-query-parameters"></a><span data-ttu-id="18a8f-170">Предоставление настраиваемых параметров запроса</span><span class="sxs-lookup"><span data-stu-id="18a8f-170">Provide custom query parameters</span></span>

<span data-ttu-id="18a8f-171">Для пакетов SDK, поддерживающих стиль Fluent, можно указать настраиваемые значения параметров запроса с помощью списка `QueryOptions` объектов.</span><span class="sxs-lookup"><span data-stu-id="18a8f-171">For SDKs that support a fluent style, you can provide custom query parameter values by using a list of `QueryOptions` objects.</span></span> <span data-ttu-id="18a8f-172">Для пакетов SDK на основе шаблонов параметры кодируются в URL-адресе и добавляются в URI запроса.</span><span class="sxs-lookup"><span data-stu-id="18a8f-172">For template-based SDKs, the parameters are URL-encoded and added to the request URI.</span></span> <span data-ttu-id="18a8f-173">Для PowerShell определенные параметры запроса для данного API предоставляются в виде параметров для соответствующей команды.</span><span class="sxs-lookup"><span data-stu-id="18a8f-173">For PowerShell, defined query parameters for a given API are exposed as parameters to the corresponding command.</span></span>

# <a name="c"></a>[<span data-ttu-id="18a8f-174">C#</span><span class="sxs-lookup"><span data-stu-id="18a8f-174">C#</span></span>](#tab/CS)

[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-queryparams.md)]

# <a name="typescript"></a>[<span data-ttu-id="18a8f-175">TypeScript</span><span class="sxs-lookup"><span data-stu-id="18a8f-175">TypeScript</span></span>](#tab/TypeScript)

[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-queryparams.md)]

# <a name="powershell"></a>[<span data-ttu-id="18a8f-176">PowerShell</span><span class="sxs-lookup"><span data-stu-id="18a8f-176">PowerShell</span></span>](#tab/PowerShell)

[!INCLUDE [sample-code](includes/snippets/powershell/create-requests-queryparams.md)]

---
