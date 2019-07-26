---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение доступа к ресурсу Drive
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: e9d0dcc53675650d93ebe00c88c020a266608e50
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887893"
---
# <a name="get-drive"></a><span data-ttu-id="72bfb-102">Получение ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="72bfb-102">Get Drive</span></span>

<span data-ttu-id="72bfb-103">В этой статье рассказывается, как получить свойства и связи ресурса [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="72bfb-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="72bfb-104">Drive — это контейнер верхнего уровня для файловой системы, например OneDrive или библиотек документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="72bfb-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="72bfb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="72bfb-105">Permissions</span></span>

<span data-ttu-id="72bfb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72bfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72bfb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="72bfb-108">Permission type</span></span>      | <span data-ttu-id="72bfb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="72bfb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="72bfb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="72bfb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="72bfb-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72bfb-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="72bfb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="72bfb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="72bfb-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72bfb-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="72bfb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="72bfb-114">Application</span></span> | <span data-ttu-id="72bfb-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72bfb-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="72bfb-116">Получение хранилища OneDrive текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="72bfb-116">Get current user's OneDrive</span></span>

<span data-ttu-id="72bfb-117">Доступ к диску пользователя, выполнившего вход в систему (при использовании делегированной проверки подлинности), можно получить из одноэлементного множества `me`.</span><span class="sxs-lookup"><span data-stu-id="72bfb-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="72bfb-118">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="72bfb-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="72bfb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72bfb-119">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="72bfb-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="72bfb-120">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="72bfb-121">C#</span><span class="sxs-lookup"><span data-stu-id="72bfb-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72bfb-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72bfb-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="72bfb-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72bfb-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="72bfb-124">Java</span><span class="sxs-lookup"><span data-stu-id="72bfb-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="72bfb-125">Получение хранилища OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="72bfb-125">Get a user's OneDrive</span></span>

<span data-ttu-id="72bfb-126">Чтобы получить доступ к хранилищу OneDrive или OneDrive для бизнеса пользователя, ваше приложение должно запросить связь **drive** в ресурсе User.</span><span class="sxs-lookup"><span data-stu-id="72bfb-126">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="72bfb-127">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="72bfb-127">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="72bfb-128">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72bfb-128">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="72bfb-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="72bfb-129">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="72bfb-130">C#</span><span class="sxs-lookup"><span data-stu-id="72bfb-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72bfb-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72bfb-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="72bfb-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72bfb-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="72bfb-133">Java</span><span class="sxs-lookup"><span data-stu-id="72bfb-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="72bfb-134">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="72bfb-134">Path parameters</span></span>

| <span data-ttu-id="72bfb-135">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="72bfb-135">Parameter name</span></span> | <span data-ttu-id="72bfb-136">Значение</span><span class="sxs-lookup"><span data-stu-id="72bfb-136">Value</span></span>  | <span data-ttu-id="72bfb-137">Описание</span><span class="sxs-lookup"><span data-stu-id="72bfb-137">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="72bfb-138">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="72bfb-138">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="72bfb-139">строка</span><span class="sxs-lookup"><span data-stu-id="72bfb-139">string</span></span> | <span data-ttu-id="72bfb-140">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72bfb-140">Required.</span></span> <span data-ttu-id="72bfb-141">Идентификатор объекта пользователя, которому принадлежит хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="72bfb-141">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="72bfb-142">Получение библиотеки документов, связанной с группой</span><span class="sxs-lookup"><span data-stu-id="72bfb-142">Get the document library associated with a group</span></span>

<span data-ttu-id="72bfb-143">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для группы, ваше приложение должно запросить связь **drive** в объекте Group.</span><span class="sxs-lookup"><span data-stu-id="72bfb-143">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="72bfb-144">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72bfb-144">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="72bfb-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="72bfb-145">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="72bfb-146">C#</span><span class="sxs-lookup"><span data-stu-id="72bfb-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72bfb-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72bfb-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="72bfb-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72bfb-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="72bfb-149">Java</span><span class="sxs-lookup"><span data-stu-id="72bfb-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="72bfb-150">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="72bfb-150">Path parameters</span></span>

| <span data-ttu-id="72bfb-151">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="72bfb-151">Parameter name</span></span> | <span data-ttu-id="72bfb-152">Значение</span><span class="sxs-lookup"><span data-stu-id="72bfb-152">Value</span></span>  | <span data-ttu-id="72bfb-153">Описание</span><span class="sxs-lookup"><span data-stu-id="72bfb-153">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="72bfb-154">_groupId_</span><span class="sxs-lookup"><span data-stu-id="72bfb-154">_groupId_</span></span>      | <span data-ttu-id="72bfb-155">строка</span><span class="sxs-lookup"><span data-stu-id="72bfb-155">string</span></span> | <span data-ttu-id="72bfb-156">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72bfb-156">Required.</span></span> <span data-ttu-id="72bfb-157">Идентификатор группы, которой принадлежит библиотека документов.</span><span class="sxs-lookup"><span data-stu-id="72bfb-157">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="72bfb-158">Получение библиотеки документов для сайта</span><span class="sxs-lookup"><span data-stu-id="72bfb-158">Get the document library for a site</span></span>

<span data-ttu-id="72bfb-159">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для [сайта](../resources/site.md), ваше приложение должно запросить связь **drive** в объекте Site.</span><span class="sxs-lookup"><span data-stu-id="72bfb-159">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="72bfb-160">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72bfb-160">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="72bfb-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="72bfb-161">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="72bfb-162">C#</span><span class="sxs-lookup"><span data-stu-id="72bfb-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72bfb-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72bfb-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="72bfb-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72bfb-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="72bfb-165">Java</span><span class="sxs-lookup"><span data-stu-id="72bfb-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-site-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="72bfb-166">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="72bfb-166">Path parameters</span></span>

| <span data-ttu-id="72bfb-167">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="72bfb-167">Parameter name</span></span> | <span data-ttu-id="72bfb-168">Значение</span><span class="sxs-lookup"><span data-stu-id="72bfb-168">Value</span></span>  | <span data-ttu-id="72bfb-169">Описание</span><span class="sxs-lookup"><span data-stu-id="72bfb-169">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="72bfb-170">_siteId_</span><span class="sxs-lookup"><span data-stu-id="72bfb-170">_siteId_</span></span>       | <span data-ttu-id="72bfb-171">строка</span><span class="sxs-lookup"><span data-stu-id="72bfb-171">string</span></span> | <span data-ttu-id="72bfb-172">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="72bfb-172">Required.</span></span> <span data-ttu-id="72bfb-173">Идентификатор для сайта, который содержит библиотеку документов.</span><span class="sxs-lookup"><span data-stu-id="72bfb-173">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="72bfb-174">Получение диска с использованием его идентификатора</span><span class="sxs-lookup"><span data-stu-id="72bfb-174">Get a drive by ID</span></span>

<span data-ttu-id="72bfb-175">Если у вас есть уникальный идентификатор диска, вы можете получить доступ к этому диску непосредственно из коллекции дисков верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="72bfb-175">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="72bfb-176">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="72bfb-176">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="72bfb-177">HTTP</span><span class="sxs-lookup"><span data-stu-id="72bfb-177">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="72bfb-178">C#</span><span class="sxs-lookup"><span data-stu-id="72bfb-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="72bfb-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="72bfb-179">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="72bfb-180">Objective-C</span><span class="sxs-lookup"><span data-stu-id="72bfb-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="72bfb-181">Java</span><span class="sxs-lookup"><span data-stu-id="72bfb-181">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="72bfb-182">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="72bfb-182">Path parameters</span></span>

| <span data-ttu-id="72bfb-183">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="72bfb-183">Parameter name</span></span> | <span data-ttu-id="72bfb-184">Значение</span><span class="sxs-lookup"><span data-stu-id="72bfb-184">Value</span></span>  | <span data-ttu-id="72bfb-185">Описание</span><span class="sxs-lookup"><span data-stu-id="72bfb-185">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="72bfb-186">_driveId_</span><span class="sxs-lookup"><span data-stu-id="72bfb-186">_driveId_</span></span>      | <span data-ttu-id="72bfb-187">string</span><span class="sxs-lookup"><span data-stu-id="72bfb-187">string</span></span> | <span data-ttu-id="72bfb-p105">Обязательный. Идентификатор запрошенного диска.</span><span class="sxs-lookup"><span data-stu-id="72bfb-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="72bfb-190">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="72bfb-190">Optional query parameters</span></span>

<span data-ttu-id="72bfb-191">Эти методы поддерживают [параметр запроса $select][odata-query-parameters] для формирования ответа.</span><span class="sxs-lookup"><span data-stu-id="72bfb-191">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="72bfb-192">Ответ</span><span class="sxs-lookup"><span data-stu-id="72bfb-192">Response</span></span>

<span data-ttu-id="72bfb-193">Каждый из этих методов возвращает [ресурс Drive][drive-resource] для соответствующего диска в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="72bfb-193">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="72bfb-194">Коды ответов с ошибками</span><span class="sxs-lookup"><span data-stu-id="72bfb-194">Error response codes</span></span>

<span data-ttu-id="72bfb-195">Если диск не существует, и не удается подготовить его к работе автоматически (при использовании делегированной проверки подлинности), будет возвращен ответ `HTTP 404`.</span><span class="sxs-lookup"><span data-stu-id="72bfb-195">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

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
