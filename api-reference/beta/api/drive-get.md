---
author: JeremyKelley
description: В этой статье рассказывается, как получить свойства и связи ресурса Drive.
ms.date: 09/10/2017
title: Получение ресурса Drive
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4593959b5940df46d5a81dad95710aa6650511e4
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718179"
---
# <a name="get-drive"></a><span data-ttu-id="77e34-103">Получение ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="77e34-103">Get Drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77e34-104">В этой статье рассказывается, как получить свойства и связи ресурса [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="77e34-104">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="77e34-105">Drive — это контейнер верхнего уровня для файловой системы, например OneDrive или библиотек документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="77e34-105">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="77e34-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77e34-106">Permissions</span></span>

<span data-ttu-id="77e34-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77e34-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77e34-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77e34-109">Permission type</span></span>      | <span data-ttu-id="77e34-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77e34-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77e34-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77e34-111">Delegated (work or school account)</span></span> | <span data-ttu-id="77e34-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77e34-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="77e34-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77e34-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77e34-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77e34-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="77e34-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77e34-115">Application</span></span> | <span data-ttu-id="77e34-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77e34-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="77e34-117">Получение хранилища OneDrive текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="77e34-117">Get current user's OneDrive</span></span>

<span data-ttu-id="77e34-118">Доступ к диску пользователя, выполнившего вход в систему (при использовании делегированной проверки подлинности), можно получить из одноэлементного множества `me`.</span><span class="sxs-lookup"><span data-stu-id="77e34-118">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="77e34-119">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="77e34-119">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="77e34-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77e34-120">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="77e34-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="77e34-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="77e34-122">C#</span><span class="sxs-lookup"><span data-stu-id="77e34-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77e34-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77e34-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77e34-124">Цель — C</span><span class="sxs-lookup"><span data-stu-id="77e34-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="77e34-125">Получение хранилища OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="77e34-125">Get a user's OneDrive</span></span>

<span data-ttu-id="77e34-126">Чтобы получить доступ к хранилищу OneDrive или OneDrive для бизнеса пользователя, ваше приложение должно запросить связь **drive** в ресурсе User.</span><span class="sxs-lookup"><span data-stu-id="77e34-126">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="77e34-127">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="77e34-127">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="77e34-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77e34-128">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="77e34-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="77e34-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```msgraph-interactive
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="77e34-130">C#</span><span class="sxs-lookup"><span data-stu-id="77e34-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77e34-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77e34-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77e34-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="77e34-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="77e34-133">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="77e34-133">Path parameters</span></span>

| <span data-ttu-id="77e34-134">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="77e34-134">Parameter name</span></span> | <span data-ttu-id="77e34-135">Значение</span><span class="sxs-lookup"><span data-stu-id="77e34-135">Value</span></span>  | <span data-ttu-id="77e34-136">Описание</span><span class="sxs-lookup"><span data-stu-id="77e34-136">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="77e34-137">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="77e34-137">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="77e34-138">строка</span><span class="sxs-lookup"><span data-stu-id="77e34-138">string</span></span> | <span data-ttu-id="77e34-139">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77e34-139">Required.</span></span> <span data-ttu-id="77e34-140">Идентификатор объекта пользователя, которому принадлежит хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="77e34-140">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="77e34-141">Получение библиотеки документов, связанной с группой</span><span class="sxs-lookup"><span data-stu-id="77e34-141">Get the document library associated with a group</span></span>

<span data-ttu-id="77e34-142">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для группы, ваше приложение должно запросить связь **drive** в объекте Group.</span><span class="sxs-lookup"><span data-stu-id="77e34-142">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="77e34-143">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77e34-143">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="77e34-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="77e34-144">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```msgraph-interactive
GET /groups/{groupId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="77e34-145">C#</span><span class="sxs-lookup"><span data-stu-id="77e34-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77e34-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77e34-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77e34-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="77e34-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="77e34-148">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="77e34-148">Path parameters</span></span>

| <span data-ttu-id="77e34-149">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="77e34-149">Parameter name</span></span> | <span data-ttu-id="77e34-150">Значение</span><span class="sxs-lookup"><span data-stu-id="77e34-150">Value</span></span>  | <span data-ttu-id="77e34-151">Описание</span><span class="sxs-lookup"><span data-stu-id="77e34-151">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="77e34-152">_groupId_</span><span class="sxs-lookup"><span data-stu-id="77e34-152">_groupId_</span></span>      | <span data-ttu-id="77e34-153">строка</span><span class="sxs-lookup"><span data-stu-id="77e34-153">string</span></span> | <span data-ttu-id="77e34-154">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77e34-154">Required.</span></span> <span data-ttu-id="77e34-155">Идентификатор группы, которой принадлежит библиотека документов.</span><span class="sxs-lookup"><span data-stu-id="77e34-155">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="77e34-156">Получение библиотеки документов для сайта</span><span class="sxs-lookup"><span data-stu-id="77e34-156">Get the document library for a site</span></span>

<span data-ttu-id="77e34-157">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для [сайта](../resources/site.md), ваше приложение должно запросить связь **drive** в объекте Site.</span><span class="sxs-lookup"><span data-stu-id="77e34-157">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="77e34-158">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77e34-158">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="77e34-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="77e34-159">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```msgraph-interactive
GET /sites/{siteId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="77e34-160">C#</span><span class="sxs-lookup"><span data-stu-id="77e34-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77e34-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77e34-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77e34-162">Цель — C</span><span class="sxs-lookup"><span data-stu-id="77e34-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="77e34-163">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="77e34-163">Path parameters</span></span>

| <span data-ttu-id="77e34-164">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="77e34-164">Parameter name</span></span> | <span data-ttu-id="77e34-165">Значение</span><span class="sxs-lookup"><span data-stu-id="77e34-165">Value</span></span>  | <span data-ttu-id="77e34-166">Описание</span><span class="sxs-lookup"><span data-stu-id="77e34-166">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="77e34-167">_siteId_</span><span class="sxs-lookup"><span data-stu-id="77e34-167">_siteId_</span></span>       | <span data-ttu-id="77e34-168">строка</span><span class="sxs-lookup"><span data-stu-id="77e34-168">string</span></span> | <span data-ttu-id="77e34-169">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="77e34-169">Required.</span></span> <span data-ttu-id="77e34-170">Идентификатор для сайта, который содержит библиотеку документов.</span><span class="sxs-lookup"><span data-stu-id="77e34-170">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="77e34-171">Получение диска с использованием его идентификатора</span><span class="sxs-lookup"><span data-stu-id="77e34-171">Get a drive by ID</span></span>

<span data-ttu-id="77e34-172">Если у вас есть уникальный идентификатор диска, вы можете получить доступ к этому диску непосредственно из коллекции дисков верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="77e34-172">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="77e34-173">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77e34-173">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="77e34-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="77e34-174">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```msgraph-interactive
GET /drives/{driveId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="77e34-175">C#</span><span class="sxs-lookup"><span data-stu-id="77e34-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="77e34-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="77e34-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="77e34-177">Цель — C</span><span class="sxs-lookup"><span data-stu-id="77e34-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="77e34-178">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="77e34-178">Path parameters</span></span>

| <span data-ttu-id="77e34-179">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="77e34-179">Parameter name</span></span> | <span data-ttu-id="77e34-180">Значение</span><span class="sxs-lookup"><span data-stu-id="77e34-180">Value</span></span>  | <span data-ttu-id="77e34-181">Описание</span><span class="sxs-lookup"><span data-stu-id="77e34-181">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="77e34-182">_driveId_</span><span class="sxs-lookup"><span data-stu-id="77e34-182">_driveId_</span></span>      | <span data-ttu-id="77e34-183">string</span><span class="sxs-lookup"><span data-stu-id="77e34-183">string</span></span> | <span data-ttu-id="77e34-p105">Обязательный. Идентификатор запрошенного диска.</span><span class="sxs-lookup"><span data-stu-id="77e34-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="77e34-186">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="77e34-186">Optional query parameters</span></span>

<span data-ttu-id="77e34-187">Эти методы поддерживают [параметр запроса $select][odata-query-parameters] для формирования ответа.</span><span class="sxs-lookup"><span data-stu-id="77e34-187">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="77e34-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="77e34-188">Response</span></span>

<span data-ttu-id="77e34-189">Каждый из этих методов возвращает [ресурс Drive][drive-resource] для соответствующего диска в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="77e34-189">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default" , "get-drive-by-site-id",] } -->

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

### <a name="error-response-codes"></a><span data-ttu-id="77e34-190">Коды ответов с ошибками</span><span class="sxs-lookup"><span data-stu-id="77e34-190">Error response codes</span></span>

<span data-ttu-id="77e34-191">Если диск не существует, и не удается подготовить его к работе автоматически (при использовании делегированной проверки подлинности), будет возвращен ответ `HTTP 404`.</span><span class="sxs-lookup"><span data-stu-id="77e34-191">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!--
{
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "Drives/Get drive",
  "suppressions": [
  ]
}
-->
