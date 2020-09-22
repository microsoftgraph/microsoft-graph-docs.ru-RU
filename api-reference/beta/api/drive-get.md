---
author: JeremyKelley
description: Получение свойств и связей ресурса Drive.
ms.date: 09/10/2017
title: Получение ресурса Drive
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 579a0e59c3227056ade1587f83cbe69911ecd9fc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982278"
---
# <a name="get-drive"></a><span data-ttu-id="e6ed4-103">Получение ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="e6ed4-103">Get Drive</span></span>

<span data-ttu-id="e6ed4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6ed4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6ed4-105">В этой статье рассказывается, как получить свойства и связи ресурса [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="e6ed4-105">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="e6ed4-106">Drive — это контейнер верхнего уровня для файловой системы, например OneDrive или библиотек документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e6ed4-106">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6ed4-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6ed4-107">Permissions</span></span>

<span data-ttu-id="e6ed4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6ed4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6ed4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6ed4-110">Permission type</span></span>      | <span data-ttu-id="e6ed4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6ed4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6ed4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6ed4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e6ed4-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6ed4-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e6ed4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6ed4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6ed4-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6ed4-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e6ed4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6ed4-116">Application</span></span> | <span data-ttu-id="e6ed4-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6ed4-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="e6ed4-118">Получение хранилища OneDrive текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="e6ed4-118">Get current user's OneDrive</span></span>

<span data-ttu-id="e6ed4-119">Доступ к диску пользователя, выполнившего вход в систему (при использовании делегированной проверки подлинности), можно получить из одноэлементного множества `me`.</span><span class="sxs-lookup"><span data-stu-id="e6ed4-119">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="e6ed4-120">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="e6ed4-120">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="e6ed4-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6ed4-121">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="e6ed4-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6ed4-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive
```
# <a name="c"></a>[<span data-ttu-id="e6ed4-123">C#</span><span class="sxs-lookup"><span data-stu-id="e6ed4-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6ed4-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6ed4-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6ed4-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6ed4-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="e6ed4-126">Получение хранилища OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="e6ed4-126">Get a user's OneDrive</span></span>

<span data-ttu-id="e6ed4-127">Чтобы получить доступ к хранилищу OneDrive или OneDrive для бизнеса пользователя, ваше приложение должно запросить связь **drive** в ресурсе User.</span><span class="sxs-lookup"><span data-stu-id="e6ed4-127">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="e6ed4-128">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="e6ed4-128">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="e6ed4-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6ed4-129">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="e6ed4-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6ed4-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```msgraph-interactive
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="c"></a>[<span data-ttu-id="e6ed4-131">C#</span><span class="sxs-lookup"><span data-stu-id="e6ed4-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6ed4-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6ed4-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6ed4-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6ed4-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="e6ed4-134">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="e6ed4-134">Path parameters</span></span>

| <span data-ttu-id="e6ed4-135">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="e6ed4-135">Parameter name</span></span> | <span data-ttu-id="e6ed4-136">Значение</span><span class="sxs-lookup"><span data-stu-id="e6ed4-136">Value</span></span>  | <span data-ttu-id="e6ed4-137">Описание</span><span class="sxs-lookup"><span data-stu-id="e6ed4-137">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="e6ed4-138">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="e6ed4-138">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="e6ed4-139">строка</span><span class="sxs-lookup"><span data-stu-id="e6ed4-139">string</span></span> | <span data-ttu-id="e6ed4-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6ed4-140">Required.</span></span> <span data-ttu-id="e6ed4-141">Идентификатор объекта пользователя, которому принадлежит хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e6ed4-141">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="e6ed4-142">Получение библиотеки документов, связанной с группой</span><span class="sxs-lookup"><span data-stu-id="e6ed4-142">Get the document library associated with a group</span></span>

<span data-ttu-id="e6ed4-143">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для группы, ваше приложение должно запросить связь **drive** в объекте Group.</span><span class="sxs-lookup"><span data-stu-id="e6ed4-143">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="e6ed4-144">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6ed4-144">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="e6ed4-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6ed4-145">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```msgraph-interactive
GET /groups/{groupId}/drive
```
# <a name="c"></a>[<span data-ttu-id="e6ed4-146">C#</span><span class="sxs-lookup"><span data-stu-id="e6ed4-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6ed4-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6ed4-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6ed4-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6ed4-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="e6ed4-149">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="e6ed4-149">Path parameters</span></span>

| <span data-ttu-id="e6ed4-150">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="e6ed4-150">Parameter name</span></span> | <span data-ttu-id="e6ed4-151">Значение</span><span class="sxs-lookup"><span data-stu-id="e6ed4-151">Value</span></span>  | <span data-ttu-id="e6ed4-152">Описание</span><span class="sxs-lookup"><span data-stu-id="e6ed4-152">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="e6ed4-153">_groupId_</span><span class="sxs-lookup"><span data-stu-id="e6ed4-153">_groupId_</span></span>      | <span data-ttu-id="e6ed4-154">строка</span><span class="sxs-lookup"><span data-stu-id="e6ed4-154">string</span></span> | <span data-ttu-id="e6ed4-155">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6ed4-155">Required.</span></span> <span data-ttu-id="e6ed4-156">Идентификатор группы, которой принадлежит библиотека документов.</span><span class="sxs-lookup"><span data-stu-id="e6ed4-156">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="e6ed4-157">Получение библиотеки документов для сайта</span><span class="sxs-lookup"><span data-stu-id="e6ed4-157">Get the document library for a site</span></span>

<span data-ttu-id="e6ed4-158">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для [сайта](../resources/site.md), ваше приложение должно запросить связь **drive** в объекте Site.</span><span class="sxs-lookup"><span data-stu-id="e6ed4-158">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="e6ed4-159">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6ed4-159">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="e6ed4-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6ed4-160">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```msgraph-interactive
GET /sites/{siteId}/drive
```
# <a name="c"></a>[<span data-ttu-id="e6ed4-161">C#</span><span class="sxs-lookup"><span data-stu-id="e6ed4-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6ed4-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6ed4-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6ed4-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6ed4-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="e6ed4-164">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="e6ed4-164">Path parameters</span></span>

| <span data-ttu-id="e6ed4-165">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="e6ed4-165">Parameter name</span></span> | <span data-ttu-id="e6ed4-166">Значение</span><span class="sxs-lookup"><span data-stu-id="e6ed4-166">Value</span></span>  | <span data-ttu-id="e6ed4-167">Описание</span><span class="sxs-lookup"><span data-stu-id="e6ed4-167">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="e6ed4-168">_siteId_</span><span class="sxs-lookup"><span data-stu-id="e6ed4-168">_siteId_</span></span>       | <span data-ttu-id="e6ed4-169">строка</span><span class="sxs-lookup"><span data-stu-id="e6ed4-169">string</span></span> | <span data-ttu-id="e6ed4-170">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6ed4-170">Required.</span></span> <span data-ttu-id="e6ed4-171">Идентификатор для сайта, который содержит библиотеку документов.</span><span class="sxs-lookup"><span data-stu-id="e6ed4-171">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="e6ed4-172">Получение диска с использованием его идентификатора</span><span class="sxs-lookup"><span data-stu-id="e6ed4-172">Get a drive by ID</span></span>

<span data-ttu-id="e6ed4-173">Если у вас есть уникальный идентификатор диска, вы можете получить доступ к этому диску непосредственно из коллекции дисков верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="e6ed4-173">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="e6ed4-174">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6ed4-174">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="e6ed4-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="e6ed4-175">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```msgraph-interactive
GET /drives/{driveId}
```
# <a name="c"></a>[<span data-ttu-id="e6ed4-176">C#</span><span class="sxs-lookup"><span data-stu-id="e6ed4-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e6ed4-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e6ed4-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e6ed4-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e6ed4-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="e6ed4-179">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="e6ed4-179">Path parameters</span></span>

| <span data-ttu-id="e6ed4-180">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="e6ed4-180">Parameter name</span></span> | <span data-ttu-id="e6ed4-181">Значение</span><span class="sxs-lookup"><span data-stu-id="e6ed4-181">Value</span></span>  | <span data-ttu-id="e6ed4-182">Описание</span><span class="sxs-lookup"><span data-stu-id="e6ed4-182">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="e6ed4-183">_driveId_</span><span class="sxs-lookup"><span data-stu-id="e6ed4-183">_driveId_</span></span>      | <span data-ttu-id="e6ed4-184">string</span><span class="sxs-lookup"><span data-stu-id="e6ed4-184">string</span></span> | <span data-ttu-id="e6ed4-p105">Обязательный. Идентификатор запрошенного диска.</span><span class="sxs-lookup"><span data-stu-id="e6ed4-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="e6ed4-187">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e6ed4-187">Optional query parameters</span></span>

<span data-ttu-id="e6ed4-188">Эти методы поддерживают [параметр запроса $select][odata-query-parameters] для формирования ответа.</span><span class="sxs-lookup"><span data-stu-id="e6ed4-188">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="e6ed4-189">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6ed4-189">Response</span></span>

<span data-ttu-id="e6ed4-190">Каждый из этих методов возвращает [ресурс Drive][drive-resource] для соответствующего диска в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e6ed4-190">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="e6ed4-191">Коды ответов с ошибками</span><span class="sxs-lookup"><span data-stu-id="e6ed4-191">Error response codes</span></span>

<span data-ttu-id="e6ed4-192">Если диск не существует, и не удается подготовить его к работе автоматически (при использовании делегированной проверки подлинности), будет возвращен ответ `HTTP 404`.</span><span class="sxs-lookup"><span data-stu-id="e6ed4-192">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!--
{
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Microsoft 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "Drives/Get drive",
  "suppressions": [
  ]
}
-->


