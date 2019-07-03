---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение доступа к ресурсу Drive
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: f7d98e0f3b7963bc5d3ced3cd144b90b8f51f86c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35461199"
---
# <a name="get-drive"></a><span data-ttu-id="c7845-102">Получение ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="c7845-102">Get Drive</span></span>

<span data-ttu-id="c7845-103">В этой статье рассказывается, как получить свойства и связи ресурса [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="c7845-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="c7845-104">Drive — это контейнер верхнего уровня для файловой системы, например OneDrive или библиотек документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c7845-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7845-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7845-105">Permissions</span></span>

<span data-ttu-id="c7845-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7845-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c7845-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7845-108">Permission type</span></span>      | <span data-ttu-id="c7845-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7845-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c7845-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7845-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c7845-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7845-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c7845-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7845-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7845-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7845-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c7845-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7845-114">Application</span></span> | <span data-ttu-id="c7845-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c7845-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="c7845-116">Получение хранилища OneDrive текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="c7845-116">Get current user's OneDrive</span></span>

<span data-ttu-id="c7845-117">Доступ к диску пользователя, выполнившего вход в систему (при использовании делегированной проверки подлинности), можно получить из одноэлементного множества `me`.</span><span class="sxs-lookup"><span data-stu-id="c7845-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="c7845-118">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="c7845-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="c7845-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7845-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c7845-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7845-120">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c7845-121">C#</span><span class="sxs-lookup"><span data-stu-id="c7845-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c7845-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7845-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c7845-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7845-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="c7845-124">Получение хранилища OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="c7845-124">Get a user's OneDrive</span></span>

<span data-ttu-id="c7845-125">Чтобы получить доступ к хранилищу OneDrive или OneDrive для бизнеса пользователя, ваше приложение должно запросить связь **drive** в ресурсе User.</span><span class="sxs-lookup"><span data-stu-id="c7845-125">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="c7845-126">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="c7845-126">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="c7845-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7845-127">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c7845-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7845-128">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c7845-129">C#</span><span class="sxs-lookup"><span data-stu-id="c7845-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c7845-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7845-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c7845-131">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7845-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="c7845-132">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="c7845-132">Path parameters</span></span>

| <span data-ttu-id="c7845-133">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="c7845-133">Parameter name</span></span> | <span data-ttu-id="c7845-134">Значение</span><span class="sxs-lookup"><span data-stu-id="c7845-134">Value</span></span>  | <span data-ttu-id="c7845-135">Описание</span><span class="sxs-lookup"><span data-stu-id="c7845-135">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="c7845-136">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="c7845-136">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="c7845-137">строка</span><span class="sxs-lookup"><span data-stu-id="c7845-137">string</span></span> | <span data-ttu-id="c7845-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7845-138">Required.</span></span> <span data-ttu-id="c7845-139">Идентификатор объекта пользователя, которому принадлежит хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c7845-139">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="c7845-140">Получение библиотеки документов, связанной с группой</span><span class="sxs-lookup"><span data-stu-id="c7845-140">Get the document library associated with a group</span></span>

<span data-ttu-id="c7845-141">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для группы, ваше приложение должно запросить связь **drive** в объекте Group.</span><span class="sxs-lookup"><span data-stu-id="c7845-141">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="c7845-142">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7845-142">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c7845-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7845-143">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c7845-144">C#</span><span class="sxs-lookup"><span data-stu-id="c7845-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c7845-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7845-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c7845-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7845-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="c7845-147">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="c7845-147">Path parameters</span></span>

| <span data-ttu-id="c7845-148">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="c7845-148">Parameter name</span></span> | <span data-ttu-id="c7845-149">Значение</span><span class="sxs-lookup"><span data-stu-id="c7845-149">Value</span></span>  | <span data-ttu-id="c7845-150">Описание</span><span class="sxs-lookup"><span data-stu-id="c7845-150">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="c7845-151">_groupId_</span><span class="sxs-lookup"><span data-stu-id="c7845-151">_groupId_</span></span>      | <span data-ttu-id="c7845-152">строка</span><span class="sxs-lookup"><span data-stu-id="c7845-152">string</span></span> | <span data-ttu-id="c7845-153">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7845-153">Required.</span></span> <span data-ttu-id="c7845-154">Идентификатор группы, которой принадлежит библиотека документов.</span><span class="sxs-lookup"><span data-stu-id="c7845-154">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="c7845-155">Получение библиотеки документов для сайта</span><span class="sxs-lookup"><span data-stu-id="c7845-155">Get the document library for a site</span></span>

<span data-ttu-id="c7845-156">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для [сайта](../resources/site.md), ваше приложение должно запросить связь **drive** в объекте Site.</span><span class="sxs-lookup"><span data-stu-id="c7845-156">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="c7845-157">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7845-157">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c7845-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7845-158">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c7845-159">C#</span><span class="sxs-lookup"><span data-stu-id="c7845-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c7845-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7845-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c7845-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7845-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="c7845-162">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="c7845-162">Path parameters</span></span>

| <span data-ttu-id="c7845-163">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="c7845-163">Parameter name</span></span> | <span data-ttu-id="c7845-164">Значение</span><span class="sxs-lookup"><span data-stu-id="c7845-164">Value</span></span>  | <span data-ttu-id="c7845-165">Описание</span><span class="sxs-lookup"><span data-stu-id="c7845-165">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="c7845-166">_siteId_</span><span class="sxs-lookup"><span data-stu-id="c7845-166">_siteId_</span></span>       | <span data-ttu-id="c7845-167">строка</span><span class="sxs-lookup"><span data-stu-id="c7845-167">string</span></span> | <span data-ttu-id="c7845-168">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7845-168">Required.</span></span> <span data-ttu-id="c7845-169">Идентификатор для сайта, который содержит библиотеку документов.</span><span class="sxs-lookup"><span data-stu-id="c7845-169">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="c7845-170">Получение диска с использованием его идентификатора</span><span class="sxs-lookup"><span data-stu-id="c7845-170">Get a drive by ID</span></span>

<span data-ttu-id="c7845-171">Если у вас есть уникальный идентификатор диска, вы можете получить доступ к этому диску непосредственно из коллекции дисков верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="c7845-171">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="c7845-172">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7845-172">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c7845-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="c7845-173">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c7845-174">C#</span><span class="sxs-lookup"><span data-stu-id="c7845-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c7845-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c7845-175">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c7845-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c7845-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="c7845-177">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="c7845-177">Path parameters</span></span>

| <span data-ttu-id="c7845-178">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="c7845-178">Parameter name</span></span> | <span data-ttu-id="c7845-179">Значение</span><span class="sxs-lookup"><span data-stu-id="c7845-179">Value</span></span>  | <span data-ttu-id="c7845-180">Описание</span><span class="sxs-lookup"><span data-stu-id="c7845-180">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="c7845-181">_driveId_</span><span class="sxs-lookup"><span data-stu-id="c7845-181">_driveId_</span></span>      | <span data-ttu-id="c7845-182">string</span><span class="sxs-lookup"><span data-stu-id="c7845-182">string</span></span> | <span data-ttu-id="c7845-p105">Обязательный. Идентификатор запрошенного диска.</span><span class="sxs-lookup"><span data-stu-id="c7845-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="c7845-185">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c7845-185">Optional query parameters</span></span>

<span data-ttu-id="c7845-186">Эти методы поддерживают [параметр запроса $select][odata-query-parameters] для формирования ответа.</span><span class="sxs-lookup"><span data-stu-id="c7845-186">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="c7845-187">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7845-187">Response</span></span>

<span data-ttu-id="c7845-188">Каждый из этих методов возвращает [ресурс Drive][drive-resource] для соответствующего диска в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7845-188">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="c7845-189">Коды ответов с ошибками</span><span class="sxs-lookup"><span data-stu-id="c7845-189">Error response codes</span></span>

<span data-ttu-id="c7845-190">Если диск не существует, и не удается подготовить его к работе автоматически (при использовании делегированной проверки подлинности), будет возвращен ответ `HTTP 404`.</span><span class="sxs-lookup"><span data-stu-id="c7845-190">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

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
