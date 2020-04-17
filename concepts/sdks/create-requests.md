---
title: Выполнение вызовов API с помощью пакетов SDK Microsoft Graph
description: Содержит инструкции по созданию HTTP-запросов Microsoft Graph с помощью пакетов SDK.
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: d4fdd5fc6c9a5b2fb0e8acd6d5484176ef179333
ms.sourcegitcommit: d189830649794365464e37539e02239f883011da
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2019
ms.locfileid: "37653519"
---
# <a name="make-api-calls-using-the-microsoft-graph-sdks"></a><span data-ttu-id="046b2-103">Выполнение вызовов API с помощью пакетов SDK Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="046b2-103">Make API calls using the Microsoft Graph SDKs</span></span>

<span data-ttu-id="046b2-104">Библиотеки службы SDK Microsoft Graph предоставляют клиентский класс, который можно использовать в качестве отправной точки для создания всех запросов API.</span><span class="sxs-lookup"><span data-stu-id="046b2-104">The Microsoft Graph SDK service libraries provide a client class that you can use as the starting point for creating all API requests.</span></span> <span data-ttu-id="046b2-105">Существует два стиля клиентского класса: один использует интерфейс Fluent для создания запроса (например, `client.Me.Manager`), а другой принимает строку пути (например, `api("/me/manager")`).</span><span class="sxs-lookup"><span data-stu-id="046b2-105">There are two styles of client class: one uses a fluent interface to create the request (for example, `client.Me.Manager`) and the other  accepts a path string (for example, `api("/me/manager")`).</span></span> <span data-ttu-id="046b2-106">Когда у вас есть объект Request, вы можете указать различные параметры, такие как фильтрация и сортировка, и, наконец, выбрать тип операции, которую необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="046b2-106">When you have a request object, you can specify a variety of options such as filtering and sorting, and finally, you select the type of operation you want to perform.</span></span>

## <a name="read-information-from-microsoft-graph"></a><span data-ttu-id="046b2-107">Чтение информации из Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="046b2-107">Read information from Microsoft Graph</span></span>

<span data-ttu-id="046b2-108">Чтобы прочитать данные из Microsoft Graph, сначала необходимо создать объект Request, а затем выполнить `GET` метод для запроса.</span><span class="sxs-lookup"><span data-stu-id="046b2-108">To read information from Microsoft Graph, you first need to create a request object and then run the `GET` method on the request.</span></span>

# <a name="c"></a>[<span data-ttu-id="046b2-109">C#</span><span class="sxs-lookup"><span data-stu-id="046b2-109">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-read.md)]
# <a name="typescript"></a>[<span data-ttu-id="046b2-110">TypeScript</span><span class="sxs-lookup"><span data-stu-id="046b2-110">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-read.md)]
---

## <a name="use-select-to-control-the-properties-returned"></a><span data-ttu-id="046b2-111">Использование $select для управления возвращаемыми свойствами</span><span class="sxs-lookup"><span data-stu-id="046b2-111">Use $select to control the properties returned</span></span>

<span data-ttu-id="046b2-112">При получении объекта автоматически извлекаются не все свойства; Иногда они должны быть явно выбраны.</span><span class="sxs-lookup"><span data-stu-id="046b2-112">When retrieving an entity, not all properties are automatically retrieved; sometimes they need to be explicitly selected.</span></span> <span data-ttu-id="046b2-113">Кроме того, в некоторых случаях не требуется возвращать набор свойств по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="046b2-113">Also, in some scenarios it isn't necessary to return the default set of properties.</span></span> <span data-ttu-id="046b2-114">Выбор только обязательных свойств может увеличить производительность запроса.</span><span class="sxs-lookup"><span data-stu-id="046b2-114">Selecting just the required properties can improve the performance of the request.</span></span> <span data-ttu-id="046b2-115">Вы можете настроить объект *request* так, чтобы он `$select` выдать параметр запроса с помощью списка свойств.</span><span class="sxs-lookup"><span data-stu-id="046b2-115">You can customize the *request* object to emit the `$select` query parameter with a list of properties.</span></span>

# <a name="c"></a>[<span data-ttu-id="046b2-116">C#</span><span class="sxs-lookup"><span data-stu-id="046b2-116">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-select.md)]
# <a name="typescript"></a>[<span data-ttu-id="046b2-117">TypeScript</span><span class="sxs-lookup"><span data-stu-id="046b2-117">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-select.md)]
---


## <a name="retrieve-a-list-of-entities"></a><span data-ttu-id="046b2-118">Получение списка объектов</span><span class="sxs-lookup"><span data-stu-id="046b2-118">Retrieve a list of entities</span></span>

<span data-ttu-id="046b2-119">Получение списка сущностей аналогично получению одного объекта, за исключением ряда других вариантов настройки запроса.</span><span class="sxs-lookup"><span data-stu-id="046b2-119">Retrieving a list of entities is similar to retrieving a single entity except there a number of other options for configuring the request.</span></span> <span data-ttu-id="046b2-120">Параметр `$filter` Query можно использовать, чтобы уменьшить набор результатов до тех строк, которые соответствуют заданному условию.</span><span class="sxs-lookup"><span data-stu-id="046b2-120">The `$filter` query parameter can be used to reduce the result set to only those rows that match the provided condition.</span></span>  <span data-ttu-id="046b2-121">Параметр `$orderBy` запроса будет запрашивать, чтобы сервер предоставил список сущностей, отсортированных по указанным свойствам.</span><span class="sxs-lookup"><span data-stu-id="046b2-121">The `$orderBy` query parameter will request that the server provide the list of entities sorted by the specified properties.</span></span>

# <a name="c"></a>[<span data-ttu-id="046b2-122">C#</span><span class="sxs-lookup"><span data-stu-id="046b2-122">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-list.md)]
# <a name="typescript"></a>[<span data-ttu-id="046b2-123">TypeScript</span><span class="sxs-lookup"><span data-stu-id="046b2-123">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-list.md)]
---

<span data-ttu-id="046b2-124">Объект, возвращаемый при получении списка сущностей, скорее всего, является страничной коллекцией.</span><span class="sxs-lookup"><span data-stu-id="046b2-124">The object returned when retrieving a list of entities is likely to be a paged collection.</span></span> <span data-ttu-id="046b2-125">Сведения о том, как получить полный список сущностей, можно найти в разделе [paging a Collection](../paging.md).</span><span class="sxs-lookup"><span data-stu-id="046b2-125">For details about how to get the complete list of entities, see [paging through a collection](../paging.md).</span></span>

## <a name="access-an-item-of-a-collection"></a><span data-ttu-id="046b2-126">Доступ к элементу коллекции</span><span class="sxs-lookup"><span data-stu-id="046b2-126">Access an item of a collection</span></span>

<span data-ttu-id="046b2-127">Для пакетов SDK, поддерживающих стиль Fluent, доступ к коллекциям сущностей можно получить с помощью индекса массива.</span><span class="sxs-lookup"><span data-stu-id="046b2-127">For SDKs that support a fluent style, collections of entities can be accessed using an array index.</span></span> <span data-ttu-id="046b2-128">Для пакетов SDK на основе шаблонов достаточно внедрить идентификатор элемента в сегмент пути, следующий за коллекцией.</span><span class="sxs-lookup"><span data-stu-id="046b2-128">For template-based SDKs, it is sufficient to embed the item identifier in the path segment following the collection.</span></span>

# <a name="c"></a>[<span data-ttu-id="046b2-129">C#</span><span class="sxs-lookup"><span data-stu-id="046b2-129">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-index.md)]
# <a name="typescript"></a>[<span data-ttu-id="046b2-130">TypeScript</span><span class="sxs-lookup"><span data-stu-id="046b2-130">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-index.md)]
---

## <a name="use-expand-to-access-related-entities"></a><span data-ttu-id="046b2-131">Использование $expand для доступа к связанным сущностям</span><span class="sxs-lookup"><span data-stu-id="046b2-131">Use $expand to access related entities</span></span>

<span data-ttu-id="046b2-132">С помощью `$expand` фильтра можно запрашивать связанную сущность или коллекцию сущностей, которые запрашивают основной объект.</span><span class="sxs-lookup"><span data-stu-id="046b2-132">You can use the `$expand` filter to request a related entity, or collection of entities, at the same that you request the main entity.</span></span>  <span data-ttu-id="046b2-133">`Expand()` Функция в объекте *request* добавляет необходимый параметр запроса.</span><span class="sxs-lookup"><span data-stu-id="046b2-133">The `Expand()` function on the *request* object adds the necessary query parameter.</span></span>

# <a name="c"></a>[<span data-ttu-id="046b2-134">C#</span><span class="sxs-lookup"><span data-stu-id="046b2-134">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-expand.md)]
# <a name="typescript"></a>[<span data-ttu-id="046b2-135">TypeScript</span><span class="sxs-lookup"><span data-stu-id="046b2-135">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-expand.md)]
---


## <a name="delete-an-entity"></a><span data-ttu-id="046b2-136">Удаление объекта</span><span class="sxs-lookup"><span data-stu-id="046b2-136">Delete an entity</span></span>

<span data-ttu-id="046b2-137">Чтобы удалить сущность, создайте *запрос* так же, как и для получения объекта.</span><span class="sxs-lookup"><span data-stu-id="046b2-137">To delete an entity, construct the *request* in the same way that you do to retrieve an entity.</span></span> <span data-ttu-id="046b2-138">Метод *Delete* объекта *request* указывает на необходимость удаления объекта.</span><span class="sxs-lookup"><span data-stu-id="046b2-138">The *delete* method on the *request* object indicates the desire to delete the entity.</span></span>

# <a name="c"></a>[<span data-ttu-id="046b2-139">C#</span><span class="sxs-lookup"><span data-stu-id="046b2-139">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-delete.md)]
# <a name="typescript"></a>[<span data-ttu-id="046b2-140">TypeScript</span><span class="sxs-lookup"><span data-stu-id="046b2-140">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-delete.md)]
---

## <a name="make-a-post-request-to-create-a-new-entity"></a><span data-ttu-id="046b2-141">Создание запроса POST для создания нового объекта</span><span class="sxs-lookup"><span data-stu-id="046b2-141">Make a POST request to create a new entity</span></span>

<span data-ttu-id="046b2-142">Чтобы создать новый объект в коллекции, вызовите метод `add` или `post` и передайте объект, содержащий сведения, которые будут использоваться для создания нового объекта.</span><span class="sxs-lookup"><span data-stu-id="046b2-142">To create a new entity in a collection, call an `add` or `post` method and pass in an object that contains the information to be used to create the new entity.</span></span> <span data-ttu-id="046b2-143">Обновленная версия созданной сущности обычно возвращается при вызове.</span><span class="sxs-lookup"><span data-stu-id="046b2-143">An updated version of the created entity is usually returned from the call.</span></span>

# <a name="c"></a>[<span data-ttu-id="046b2-144">C#</span><span class="sxs-lookup"><span data-stu-id="046b2-144">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-create.md)]
# <a name="typescript"></a>[<span data-ttu-id="046b2-145">TypeScript</span><span class="sxs-lookup"><span data-stu-id="046b2-145">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-create.md)]
---

## <a name="updating-an-existing-entity-with-patch"></a><span data-ttu-id="046b2-146">Обновление существующей сущности с помощью исправления</span><span class="sxs-lookup"><span data-stu-id="046b2-146">Updating an existing entity with PATCH</span></span>

<span data-ttu-id="046b2-147">Большинство обновлений в Microsoft Graph выполняются с помощью `PATCH` метода, поэтому необходимо включить в передаваемый объект только те свойства, которые нужно изменить.</span><span class="sxs-lookup"><span data-stu-id="046b2-147">Most updates in Microsoft Graph are performed using a `PATCH` method and therefore it is only necessary to include the properties that you want to change in the object you pass.</span></span>  

# <a name="c"></a>[<span data-ttu-id="046b2-148">C#</span><span class="sxs-lookup"><span data-stu-id="046b2-148">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-update.md)]
# <a name="typescript"></a>[<span data-ttu-id="046b2-149">TypeScript</span><span class="sxs-lookup"><span data-stu-id="046b2-149">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-update.md)]
---


## <a name="use-http-headers-to-control-request-behavior"></a><span data-ttu-id="046b2-150">Использование заголовков HTTP для управления поведением запроса</span><span class="sxs-lookup"><span data-stu-id="046b2-150">Use HTTP headers to control request behavior</span></span>

<span data-ttu-id="046b2-151">Вы можете использовать `header()` функцию для присоединения пользовательских заголовков к запросу.</span><span class="sxs-lookup"><span data-stu-id="046b2-151">You can use a `header()` function to attach custom headers to a request.</span></span> <span data-ttu-id="046b2-152">В некоторых сценариях Microsoft Graph для настройки поведения запроса используются настраиваемые заголовки.</span><span class="sxs-lookup"><span data-stu-id="046b2-152">A number of Microsoft Graph scenarios use custom headers to adjust the behavior of the request.</span></span>
 
# <a name="c"></a>[<span data-ttu-id="046b2-153">C#</span><span class="sxs-lookup"><span data-stu-id="046b2-153">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-headers.md)]
# <a name="typescript"></a>[<span data-ttu-id="046b2-154">TypeScript</span><span class="sxs-lookup"><span data-stu-id="046b2-154">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-headers.md)]
---

## <a name="provide-custom-query-parameters"></a><span data-ttu-id="046b2-155">Предоставление настраиваемых параметров запроса</span><span class="sxs-lookup"><span data-stu-id="046b2-155">Provide custom query parameters</span></span>

<span data-ttu-id="046b2-156">В ситуациях, когда вызов API позволяет использовать пользовательские параметры запроса, можно предоставить эти значения параметров с помощью списка `QueryOptions` объектов.</span><span class="sxs-lookup"><span data-stu-id="046b2-156">In situations where an API call allows custom query parameters, you can provide those parameter values by using a list of `QueryOptions` objects.</span></span>

# <a name="c"></a>[<span data-ttu-id="046b2-157">C#</span><span class="sxs-lookup"><span data-stu-id="046b2-157">C#</span></span>](#tab/CS)
[!INCLUDE [sample-code](includes/snippets/csharp/create-requests-queryparams.md)]
# <a name="typescript"></a>[<span data-ttu-id="046b2-158">TypeScript</span><span class="sxs-lookup"><span data-stu-id="046b2-158">TypeScript</span></span>](#tab/TypeScript)
[!INCLUDE [sample-code](includes/snippets/typescript/create-requests-queryparams.md)]
---
