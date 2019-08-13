---
author: JeremyKelley
description: В этой статье рассказывается, как получить свойства и связи ресурса Drive.
ms.date: 09/10/2017
title: Получение ресурса Drive
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 0381e4cffc910c9169e57bdd0655041f4b9d3f0b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324456"
---
# <a name="get-drive"></a><span data-ttu-id="b1915-103">Получение ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="b1915-103">Get Drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1915-104">В этой статье рассказывается, как получить свойства и связи ресурса [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="b1915-104">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="b1915-105">Drive — это контейнер верхнего уровня для файловой системы, например OneDrive или библиотек документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="b1915-105">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1915-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b1915-106">Permissions</span></span>

<span data-ttu-id="b1915-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1915-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1915-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b1915-109">Permission type</span></span>      | <span data-ttu-id="b1915-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b1915-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1915-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b1915-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b1915-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1915-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b1915-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b1915-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1915-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1915-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b1915-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b1915-115">Application</span></span> | <span data-ttu-id="b1915-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1915-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="b1915-117">Получение хранилища OneDrive текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="b1915-117">Get current user's OneDrive</span></span>

<span data-ttu-id="b1915-118">Доступ к диску пользователя, выполнившего вход в систему (при использовании делегированной проверки подлинности), можно получить из одноэлементного множества `me`.</span><span class="sxs-lookup"><span data-stu-id="b1915-118">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="b1915-119">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="b1915-119">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="b1915-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1915-120">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b1915-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1915-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b1915-122">C#</span><span class="sxs-lookup"><span data-stu-id="b1915-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1915-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1915-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b1915-124">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b1915-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b1915-125">Java</span><span class="sxs-lookup"><span data-stu-id="b1915-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="b1915-126">Получение хранилища OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="b1915-126">Get a user's OneDrive</span></span>

<span data-ttu-id="b1915-127">Чтобы получить доступ к хранилищу OneDrive или OneDrive для бизнеса пользователя, ваше приложение должно запросить связь **drive** в ресурсе User.</span><span class="sxs-lookup"><span data-stu-id="b1915-127">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="b1915-128">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="b1915-128">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="b1915-129">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1915-129">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b1915-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1915-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b1915-131">C#</span><span class="sxs-lookup"><span data-stu-id="b1915-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1915-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1915-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b1915-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b1915-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b1915-134">Java</span><span class="sxs-lookup"><span data-stu-id="b1915-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="b1915-135">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="b1915-135">Path parameters</span></span>

| <span data-ttu-id="b1915-136">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="b1915-136">Parameter name</span></span> | <span data-ttu-id="b1915-137">Значение</span><span class="sxs-lookup"><span data-stu-id="b1915-137">Value</span></span>  | <span data-ttu-id="b1915-138">Описание</span><span class="sxs-lookup"><span data-stu-id="b1915-138">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="b1915-139">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="b1915-139">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="b1915-140">строка</span><span class="sxs-lookup"><span data-stu-id="b1915-140">string</span></span> | <span data-ttu-id="b1915-141">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1915-141">Required.</span></span> <span data-ttu-id="b1915-142">Идентификатор объекта пользователя, которому принадлежит хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="b1915-142">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="b1915-143">Получение библиотеки документов, связанной с группой</span><span class="sxs-lookup"><span data-stu-id="b1915-143">Get the document library associated with a group</span></span>

<span data-ttu-id="b1915-144">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для группы, ваше приложение должно запросить связь **drive** в объекте Group.</span><span class="sxs-lookup"><span data-stu-id="b1915-144">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="b1915-145">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1915-145">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b1915-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1915-146">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b1915-147">C#</span><span class="sxs-lookup"><span data-stu-id="b1915-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1915-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1915-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b1915-149">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b1915-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b1915-150">Java</span><span class="sxs-lookup"><span data-stu-id="b1915-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="b1915-151">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="b1915-151">Path parameters</span></span>

| <span data-ttu-id="b1915-152">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="b1915-152">Parameter name</span></span> | <span data-ttu-id="b1915-153">Значение</span><span class="sxs-lookup"><span data-stu-id="b1915-153">Value</span></span>  | <span data-ttu-id="b1915-154">Описание</span><span class="sxs-lookup"><span data-stu-id="b1915-154">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="b1915-155">_groupId_</span><span class="sxs-lookup"><span data-stu-id="b1915-155">_groupId_</span></span>      | <span data-ttu-id="b1915-156">строка</span><span class="sxs-lookup"><span data-stu-id="b1915-156">string</span></span> | <span data-ttu-id="b1915-157">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1915-157">Required.</span></span> <span data-ttu-id="b1915-158">Идентификатор группы, которой принадлежит библиотека документов.</span><span class="sxs-lookup"><span data-stu-id="b1915-158">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="b1915-159">Получение библиотеки документов для сайта</span><span class="sxs-lookup"><span data-stu-id="b1915-159">Get the document library for a site</span></span>

<span data-ttu-id="b1915-160">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для [сайта](../resources/site.md), ваше приложение должно запросить связь **drive** в объекте Site.</span><span class="sxs-lookup"><span data-stu-id="b1915-160">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="b1915-161">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1915-161">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b1915-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1915-162">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b1915-163">C#</span><span class="sxs-lookup"><span data-stu-id="b1915-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1915-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1915-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b1915-165">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b1915-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b1915-166">Java</span><span class="sxs-lookup"><span data-stu-id="b1915-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-site-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="b1915-167">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="b1915-167">Path parameters</span></span>

| <span data-ttu-id="b1915-168">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="b1915-168">Parameter name</span></span> | <span data-ttu-id="b1915-169">Значение</span><span class="sxs-lookup"><span data-stu-id="b1915-169">Value</span></span>  | <span data-ttu-id="b1915-170">Описание</span><span class="sxs-lookup"><span data-stu-id="b1915-170">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="b1915-171">_siteId_</span><span class="sxs-lookup"><span data-stu-id="b1915-171">_siteId_</span></span>       | <span data-ttu-id="b1915-172">строка</span><span class="sxs-lookup"><span data-stu-id="b1915-172">string</span></span> | <span data-ttu-id="b1915-173">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b1915-173">Required.</span></span> <span data-ttu-id="b1915-174">Идентификатор для сайта, который содержит библиотеку документов.</span><span class="sxs-lookup"><span data-stu-id="b1915-174">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="b1915-175">Получение диска с использованием его идентификатора</span><span class="sxs-lookup"><span data-stu-id="b1915-175">Get a drive by ID</span></span>

<span data-ttu-id="b1915-176">Если у вас есть уникальный идентификатор диска, вы можете получить доступ к этому диску непосредственно из коллекции дисков верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="b1915-176">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="b1915-177">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b1915-177">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b1915-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1915-178">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b1915-179">C#</span><span class="sxs-lookup"><span data-stu-id="b1915-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b1915-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1915-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b1915-181">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b1915-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b1915-182">Java</span><span class="sxs-lookup"><span data-stu-id="b1915-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="b1915-183">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="b1915-183">Path parameters</span></span>

| <span data-ttu-id="b1915-184">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="b1915-184">Parameter name</span></span> | <span data-ttu-id="b1915-185">Значение</span><span class="sxs-lookup"><span data-stu-id="b1915-185">Value</span></span>  | <span data-ttu-id="b1915-186">Описание</span><span class="sxs-lookup"><span data-stu-id="b1915-186">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="b1915-187">_driveId_</span><span class="sxs-lookup"><span data-stu-id="b1915-187">_driveId_</span></span>      | <span data-ttu-id="b1915-188">string</span><span class="sxs-lookup"><span data-stu-id="b1915-188">string</span></span> | <span data-ttu-id="b1915-p105">Обязательный. Идентификатор запрошенного диска.</span><span class="sxs-lookup"><span data-stu-id="b1915-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="b1915-191">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b1915-191">Optional query parameters</span></span>

<span data-ttu-id="b1915-192">Эти методы поддерживают [параметр запроса $select][odata-query-parameters] для формирования ответа.</span><span class="sxs-lookup"><span data-stu-id="b1915-192">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="b1915-193">Отклик</span><span class="sxs-lookup"><span data-stu-id="b1915-193">Response</span></span>

<span data-ttu-id="b1915-194">Каждый из этих методов возвращает [ресурс Drive][drive-resource] для соответствующего диска в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b1915-194">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="b1915-195">Коды ответов с ошибками</span><span class="sxs-lookup"><span data-stu-id="b1915-195">Error response codes</span></span>

<span data-ttu-id="b1915-196">Если диск не существует, и не удается подготовить его к работе автоматически (при использовании делегированной проверки подлинности), будет возвращен ответ `HTTP 404`.</span><span class="sxs-lookup"><span data-stu-id="b1915-196">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

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
