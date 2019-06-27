---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение доступа к ресурсу Drive
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 8e099f6ba8bef07cba3406e2deb2cbb8961aa227
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260356"
---
# <a name="get-drive"></a><span data-ttu-id="c36b6-102">Получение ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="c36b6-102">Get Drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c36b6-103">В этой статье рассказывается, как получить свойства и связи ресурса [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="c36b6-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="c36b6-104">Drive — это контейнер верхнего уровня для файловой системы, например OneDrive или библиотек документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c36b6-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="c36b6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c36b6-105">Permissions</span></span>

<span data-ttu-id="c36b6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c36b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c36b6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c36b6-108">Permission type</span></span>      | <span data-ttu-id="c36b6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c36b6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c36b6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c36b6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c36b6-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c36b6-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c36b6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c36b6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c36b6-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c36b6-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c36b6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c36b6-114">Application</span></span> | <span data-ttu-id="c36b6-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c36b6-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="c36b6-116">Получение хранилища OneDrive текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="c36b6-116">Get current user's OneDrive</span></span>

<span data-ttu-id="c36b6-117">Доступ к диску пользователя, выполнившего вход в систему (при использовании делегированной проверки подлинности), можно получить из одноэлементного множества `me`.</span><span class="sxs-lookup"><span data-stu-id="c36b6-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="c36b6-118">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="c36b6-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="c36b6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c36b6-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c36b6-120">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c36b6-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c36b6-121">C#</span><span class="sxs-lookup"><span data-stu-id="c36b6-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c36b6-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="c36b6-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-default-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c36b6-123">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c36b6-123">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-default-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="get-a-users-onedrive"></a><span data-ttu-id="c36b6-124">Получение хранилища OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="c36b6-124">Get a user's OneDrive</span></span>

<span data-ttu-id="c36b6-125">Чтобы получить доступ к хранилищу OneDrive или OneDrive для бизнеса пользователя, ваше приложение должно запросить связь **drive** в ресурсе User.</span><span class="sxs-lookup"><span data-stu-id="c36b6-125">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="c36b6-126">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="c36b6-126">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="c36b6-127">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c36b6-127">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c36b6-128">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c36b6-128">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c36b6-129">C#</span><span class="sxs-lookup"><span data-stu-id="c36b6-129">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c36b6-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="c36b6-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c36b6-131">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c36b6-131">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="c36b6-132">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="c36b6-132">Path parameters</span></span>

| <span data-ttu-id="c36b6-133">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="c36b6-133">Parameter name</span></span> | <span data-ttu-id="c36b6-134">Значение</span><span class="sxs-lookup"><span data-stu-id="c36b6-134">Value</span></span>  | <span data-ttu-id="c36b6-135">Описание</span><span class="sxs-lookup"><span data-stu-id="c36b6-135">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="c36b6-136">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="c36b6-136">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="c36b6-137">строка</span><span class="sxs-lookup"><span data-stu-id="c36b6-137">string</span></span> | <span data-ttu-id="c36b6-138">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c36b6-138">Required.</span></span> <span data-ttu-id="c36b6-139">Идентификатор объекта пользователя, которому принадлежит хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c36b6-139">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="c36b6-140">Получение библиотеки документов, связанной с группой</span><span class="sxs-lookup"><span data-stu-id="c36b6-140">Get the document library associated with a group</span></span>

<span data-ttu-id="c36b6-141">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для группы, ваше приложение должно запросить связь **drive** в объекте Group.</span><span class="sxs-lookup"><span data-stu-id="c36b6-141">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="c36b6-142">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c36b6-142">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c36b6-143">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c36b6-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c36b6-144">C#</span><span class="sxs-lookup"><span data-stu-id="c36b6-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c36b6-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="c36b6-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c36b6-146">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c36b6-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="c36b6-147">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="c36b6-147">Path parameters</span></span>

| <span data-ttu-id="c36b6-148">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="c36b6-148">Parameter name</span></span> | <span data-ttu-id="c36b6-149">Значение</span><span class="sxs-lookup"><span data-stu-id="c36b6-149">Value</span></span>  | <span data-ttu-id="c36b6-150">Описание</span><span class="sxs-lookup"><span data-stu-id="c36b6-150">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="c36b6-151">_groupId_</span><span class="sxs-lookup"><span data-stu-id="c36b6-151">_groupId_</span></span>      | <span data-ttu-id="c36b6-152">строка</span><span class="sxs-lookup"><span data-stu-id="c36b6-152">string</span></span> | <span data-ttu-id="c36b6-153">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c36b6-153">Required.</span></span> <span data-ttu-id="c36b6-154">Идентификатор группы, которой принадлежит библиотека документов.</span><span class="sxs-lookup"><span data-stu-id="c36b6-154">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="c36b6-155">Получение библиотеки документов для сайта</span><span class="sxs-lookup"><span data-stu-id="c36b6-155">Get the document library for a site</span></span>

<span data-ttu-id="c36b6-156">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для [сайта](../resources/site.md), ваше приложение должно запросить связь **drive** в объекте Site.</span><span class="sxs-lookup"><span data-stu-id="c36b6-156">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="c36b6-157">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c36b6-157">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c36b6-158">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c36b6-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c36b6-159">C#</span><span class="sxs-lookup"><span data-stu-id="c36b6-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c36b6-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="c36b6-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c36b6-161">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c36b6-161">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="c36b6-162">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="c36b6-162">Path parameters</span></span>

| <span data-ttu-id="c36b6-163">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="c36b6-163">Parameter name</span></span> | <span data-ttu-id="c36b6-164">Значение</span><span class="sxs-lookup"><span data-stu-id="c36b6-164">Value</span></span>  | <span data-ttu-id="c36b6-165">Описание</span><span class="sxs-lookup"><span data-stu-id="c36b6-165">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="c36b6-166">_siteId_</span><span class="sxs-lookup"><span data-stu-id="c36b6-166">_siteId_</span></span>       | <span data-ttu-id="c36b6-167">строка</span><span class="sxs-lookup"><span data-stu-id="c36b6-167">string</span></span> | <span data-ttu-id="c36b6-168">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c36b6-168">Required.</span></span> <span data-ttu-id="c36b6-169">Идентификатор для сайта, который содержит библиотеку документов.</span><span class="sxs-lookup"><span data-stu-id="c36b6-169">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="c36b6-170">Получение диска с использованием его идентификатора</span><span class="sxs-lookup"><span data-stu-id="c36b6-170">Get a drive by ID</span></span>

<span data-ttu-id="c36b6-171">Если у вас есть уникальный идентификатор диска, вы можете получить доступ к этому диску непосредственно из коллекции дисков верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="c36b6-171">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="c36b6-172">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c36b6-172">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```

### <a name="path-parameters"></a><span data-ttu-id="c36b6-173">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="c36b6-173">Path parameters</span></span>

| <span data-ttu-id="c36b6-174">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="c36b6-174">Parameter name</span></span> | <span data-ttu-id="c36b6-175">Значение</span><span class="sxs-lookup"><span data-stu-id="c36b6-175">Value</span></span>  | <span data-ttu-id="c36b6-176">Описание</span><span class="sxs-lookup"><span data-stu-id="c36b6-176">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="c36b6-177">_driveId_</span><span class="sxs-lookup"><span data-stu-id="c36b6-177">_driveId_</span></span>      | <span data-ttu-id="c36b6-178">string</span><span class="sxs-lookup"><span data-stu-id="c36b6-178">string</span></span> | <span data-ttu-id="c36b6-p105">Обязательный. Идентификатор запрошенного диска.</span><span class="sxs-lookup"><span data-stu-id="c36b6-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="c36b6-181">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c36b6-181">Optional query parameters</span></span>

<span data-ttu-id="c36b6-182">Эти методы поддерживают [параметр запроса $select][odata-query-parameters] для формирования ответа.</span><span class="sxs-lookup"><span data-stu-id="c36b6-182">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="c36b6-183">Отклик</span><span class="sxs-lookup"><span data-stu-id="c36b6-183">Response</span></span>

<span data-ttu-id="c36b6-184">Каждый из этих методов возвращает [ресурс Drive][drive-resource] для соответствующего диска в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c36b6-184">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c36b6-185">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c36b6-185">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c36b6-186">C#</span><span class="sxs-lookup"><span data-stu-id="c36b6-186">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c36b6-187">Javascript</span><span class="sxs-lookup"><span data-stu-id="c36b6-187">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c36b6-188">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c36b6-188">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="error-response-codes"></a><span data-ttu-id="c36b6-189">Коды ответов с ошибками</span><span class="sxs-lookup"><span data-stu-id="c36b6-189">Error response codes</span></span>

<span data-ttu-id="c36b6-190">Если диск не существует, и не удается подготовить его к работе автоматически (при использовании делегированной проверки подлинности), будет возвращен ответ `HTTP 404`.</span><span class="sxs-lookup"><span data-stu-id="c36b6-190">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

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
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
