---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение ресурса Drive
localization_priority: Priority
ms.prod: sharepoint
description: Получение свойств и связей ресурса Drive.
doc_type: apiPageType
ms.openlocfilehash: d3513714ecc20ba4e2036dab2c61d91250cea73e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517827"
---
# <a name="get-drive"></a><span data-ttu-id="3cfea-103">Получение ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="3cfea-103">Get Drive</span></span>

<span data-ttu-id="3cfea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cfea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3cfea-105">В этой статье рассказывается, как получить свойства и связи ресурса [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="3cfea-105">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="3cfea-106">Drive — это контейнер верхнего уровня для файловой системы, например OneDrive или библиотек документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3cfea-106">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cfea-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3cfea-107">Permissions</span></span>

<span data-ttu-id="3cfea-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3cfea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cfea-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3cfea-110">Permission type</span></span>      | <span data-ttu-id="3cfea-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3cfea-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3cfea-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3cfea-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3cfea-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cfea-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3cfea-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3cfea-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3cfea-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cfea-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="3cfea-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3cfea-116">Application</span></span> | <span data-ttu-id="3cfea-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cfea-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="3cfea-118">Получение хранилища OneDrive текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="3cfea-118">Get current user's OneDrive</span></span>

<span data-ttu-id="3cfea-119">Доступ к диску пользователя, выполнившего вход в систему (при использовании делегированной проверки подлинности), можно получить из одноэлементного множества `me`.</span><span class="sxs-lookup"><span data-stu-id="3cfea-119">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="3cfea-120">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="3cfea-120">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="3cfea-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cfea-121">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="3cfea-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cfea-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive
```
# <a name="c"></a>[<span data-ttu-id="3cfea-123">C#</span><span class="sxs-lookup"><span data-stu-id="3cfea-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cfea-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cfea-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cfea-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cfea-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cfea-126">Java</span><span class="sxs-lookup"><span data-stu-id="3cfea-126">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="3cfea-127">Получение хранилища OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="3cfea-127">Get a user's OneDrive</span></span>

<span data-ttu-id="3cfea-128">Чтобы получить доступ к хранилищу OneDrive или OneDrive для бизнеса пользователя, ваше приложение должно запросить связь **drive** в ресурсе User.</span><span class="sxs-lookup"><span data-stu-id="3cfea-128">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="3cfea-129">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="3cfea-129">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="3cfea-130">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cfea-130">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="3cfea-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cfea-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```msgraph-interactive
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="c"></a>[<span data-ttu-id="3cfea-132">C#</span><span class="sxs-lookup"><span data-stu-id="3cfea-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cfea-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cfea-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cfea-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cfea-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cfea-135">Java</span><span class="sxs-lookup"><span data-stu-id="3cfea-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="3cfea-136">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="3cfea-136">Path parameters</span></span>

| <span data-ttu-id="3cfea-137">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="3cfea-137">Parameter name</span></span> | <span data-ttu-id="3cfea-138">Значение</span><span class="sxs-lookup"><span data-stu-id="3cfea-138">Value</span></span>  | <span data-ttu-id="3cfea-139">Описание</span><span class="sxs-lookup"><span data-stu-id="3cfea-139">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="3cfea-140">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="3cfea-140">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="3cfea-141">строка</span><span class="sxs-lookup"><span data-stu-id="3cfea-141">string</span></span> | <span data-ttu-id="3cfea-142">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3cfea-142">Required.</span></span> <span data-ttu-id="3cfea-143">Идентификатор объекта пользователя, которому принадлежит хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="3cfea-143">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="3cfea-144">Получение библиотеки документов, связанной с группой</span><span class="sxs-lookup"><span data-stu-id="3cfea-144">Get the document library associated with a group</span></span>

<span data-ttu-id="3cfea-145">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для группы, ваше приложение должно запросить связь **drive** в объекте Group.</span><span class="sxs-lookup"><span data-stu-id="3cfea-145">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="3cfea-146">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cfea-146">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="3cfea-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cfea-147">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```msgraph-interactive
GET /groups/{groupId}/drive
```
# <a name="c"></a>[<span data-ttu-id="3cfea-148">C#</span><span class="sxs-lookup"><span data-stu-id="3cfea-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cfea-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cfea-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cfea-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cfea-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cfea-151">Java</span><span class="sxs-lookup"><span data-stu-id="3cfea-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="3cfea-152">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="3cfea-152">Path parameters</span></span>

| <span data-ttu-id="3cfea-153">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="3cfea-153">Parameter name</span></span> | <span data-ttu-id="3cfea-154">Значение</span><span class="sxs-lookup"><span data-stu-id="3cfea-154">Value</span></span>  | <span data-ttu-id="3cfea-155">Описание</span><span class="sxs-lookup"><span data-stu-id="3cfea-155">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="3cfea-156">_groupId_</span><span class="sxs-lookup"><span data-stu-id="3cfea-156">_groupId_</span></span>      | <span data-ttu-id="3cfea-157">строка</span><span class="sxs-lookup"><span data-stu-id="3cfea-157">string</span></span> | <span data-ttu-id="3cfea-158">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3cfea-158">Required.</span></span> <span data-ttu-id="3cfea-159">Идентификатор группы, которой принадлежит библиотека документов.</span><span class="sxs-lookup"><span data-stu-id="3cfea-159">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="3cfea-160">Получение библиотеки документов для сайта</span><span class="sxs-lookup"><span data-stu-id="3cfea-160">Get the document library for a site</span></span>

<span data-ttu-id="3cfea-161">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для [сайта](../resources/site.md), ваше приложение должно запросить связь **drive** в объекте Site.</span><span class="sxs-lookup"><span data-stu-id="3cfea-161">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="3cfea-162">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cfea-162">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="3cfea-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cfea-163">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```msgraph-interactive
GET /sites/{siteId}/drive
```
# <a name="c"></a>[<span data-ttu-id="3cfea-164">C#</span><span class="sxs-lookup"><span data-stu-id="3cfea-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cfea-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cfea-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cfea-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cfea-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cfea-167">Java</span><span class="sxs-lookup"><span data-stu-id="3cfea-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-site-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="3cfea-168">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="3cfea-168">Path parameters</span></span>

| <span data-ttu-id="3cfea-169">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="3cfea-169">Parameter name</span></span> | <span data-ttu-id="3cfea-170">Значение</span><span class="sxs-lookup"><span data-stu-id="3cfea-170">Value</span></span>  | <span data-ttu-id="3cfea-171">Описание</span><span class="sxs-lookup"><span data-stu-id="3cfea-171">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="3cfea-172">_siteId_</span><span class="sxs-lookup"><span data-stu-id="3cfea-172">_siteId_</span></span>       | <span data-ttu-id="3cfea-173">строка</span><span class="sxs-lookup"><span data-stu-id="3cfea-173">string</span></span> | <span data-ttu-id="3cfea-174">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3cfea-174">Required.</span></span> <span data-ttu-id="3cfea-175">Идентификатор для сайта, который содержит библиотеку документов.</span><span class="sxs-lookup"><span data-stu-id="3cfea-175">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="3cfea-176">Получение диска с использованием его идентификатора</span><span class="sxs-lookup"><span data-stu-id="3cfea-176">Get a drive by ID</span></span>

<span data-ttu-id="3cfea-177">Если у вас есть уникальный идентификатор диска, вы можете получить доступ к этому диску непосредственно из коллекции дисков верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="3cfea-177">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="3cfea-178">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3cfea-178">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="3cfea-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cfea-179">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```msgraph-interactive
GET /drives/{drive-id}
```
# <a name="c"></a>[<span data-ttu-id="3cfea-180">C#</span><span class="sxs-lookup"><span data-stu-id="3cfea-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cfea-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cfea-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cfea-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cfea-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cfea-183">Java</span><span class="sxs-lookup"><span data-stu-id="3cfea-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="3cfea-184">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="3cfea-184">Path parameters</span></span>

| <span data-ttu-id="3cfea-185">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="3cfea-185">Parameter name</span></span> | <span data-ttu-id="3cfea-186">Значение</span><span class="sxs-lookup"><span data-stu-id="3cfea-186">Value</span></span>  | <span data-ttu-id="3cfea-187">Описание</span><span class="sxs-lookup"><span data-stu-id="3cfea-187">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="3cfea-188">_driveId_</span><span class="sxs-lookup"><span data-stu-id="3cfea-188">_driveId_</span></span>      | <span data-ttu-id="3cfea-189">string</span><span class="sxs-lookup"><span data-stu-id="3cfea-189">string</span></span> | <span data-ttu-id="3cfea-p105">Обязательный. Идентификатор запрошенного диска.</span><span class="sxs-lookup"><span data-stu-id="3cfea-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="3cfea-192">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3cfea-192">Optional query parameters</span></span>

<span data-ttu-id="3cfea-193">Эти методы поддерживают [параметр запроса $select][odata-query-parameters] для формирования ответа.</span><span class="sxs-lookup"><span data-stu-id="3cfea-193">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="3cfea-194">Ответ</span><span class="sxs-lookup"><span data-stu-id="3cfea-194">Response</span></span>

<span data-ttu-id="3cfea-195">Каждый из этих методов возвращает [ресурс Drive][drive-resource] для соответствующего диска в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3cfea-195">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default" , "get-drive-by-site-id"] } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
    "driveType": "business",
    "owner": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Ryan Gregg"
        }
    },
    "quota": {
        "deleted": 256938,
        "remaining": 1099447353539,
        "state": "normal",
        "total": 1099511627776
    }
}
```

### <a name="error-response-codes"></a><span data-ttu-id="3cfea-196">Коды ответов с ошибками</span><span class="sxs-lookup"><span data-stu-id="3cfea-196">Error response codes</span></span>

<span data-ttu-id="3cfea-197">Если диск не существует, и не удается подготовить его к работе автоматически (при использовании делегированной проверки подлинности), будет возвращен ответ `HTTP 404`.</span><span class="sxs-lookup"><span data-stu-id="3cfea-197">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/api/drive-get.md:
        Unable to map some markdown elements into schema.
            Unmapped methods:
        get-drive-default, get-drive-by-user, get-drive-by-group, get-drive-by-id
            Unmapped tables:
        Permissions - AuthScopes, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters"
  ],
  "tocPath": "Drives/Get drive"
} -->
