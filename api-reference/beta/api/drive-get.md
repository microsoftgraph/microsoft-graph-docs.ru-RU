---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение доступа к ресурсу Drive
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 34a3b2a772f225a4b4806f0e8b305bd036bd03f7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434280"
---
# <a name="get-drive"></a><span data-ttu-id="98642-102">Получение ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="98642-102">Get Drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98642-103">В этой статье рассказывается, как получить свойства и связи ресурса [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="98642-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="98642-104">Drive — это контейнер верхнего уровня для файловой системы, например OneDrive или библиотек документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="98642-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="98642-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98642-105">Permissions</span></span>

<span data-ttu-id="98642-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98642-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98642-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98642-108">Permission type</span></span>      | <span data-ttu-id="98642-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98642-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98642-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98642-110">Delegated (work or school account)</span></span> | <span data-ttu-id="98642-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98642-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="98642-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98642-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98642-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98642-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="98642-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98642-114">Application</span></span> | <span data-ttu-id="98642-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98642-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="98642-116">Получение хранилища OneDrive текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="98642-116">Get current user's OneDrive</span></span>

<span data-ttu-id="98642-117">Доступ к диску пользователя, выполнившего вход в систему (при использовании делегированной проверки подлинности), можно получить из одноэлементного множества `me`.</span><span class="sxs-lookup"><span data-stu-id="98642-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="98642-118">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="98642-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="98642-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98642-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="98642-120">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="98642-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="98642-121">C#</span><span class="sxs-lookup"><span data-stu-id="98642-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="98642-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="98642-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-default-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="get-a-users-onedrive"></a><span data-ttu-id="98642-123">Получение хранилища OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="98642-123">Get a user's OneDrive</span></span>

<span data-ttu-id="98642-124">Чтобы получить доступ к хранилищу OneDrive или OneDrive для бизнеса пользователя, ваше приложение должно запросить связь **drive** в ресурсе User.</span><span class="sxs-lookup"><span data-stu-id="98642-124">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="98642-125">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="98642-125">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="98642-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98642-126">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="98642-127">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="98642-127">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="98642-128">C#</span><span class="sxs-lookup"><span data-stu-id="98642-128">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="98642-129">Javascript</span><span class="sxs-lookup"><span data-stu-id="98642-129">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="98642-130">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="98642-130">Path parameters</span></span>

| <span data-ttu-id="98642-131">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="98642-131">Parameter name</span></span> | <span data-ttu-id="98642-132">Значение</span><span class="sxs-lookup"><span data-stu-id="98642-132">Value</span></span>  | <span data-ttu-id="98642-133">Описание</span><span class="sxs-lookup"><span data-stu-id="98642-133">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="98642-134">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="98642-134">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="98642-135">строка</span><span class="sxs-lookup"><span data-stu-id="98642-135">string</span></span> | <span data-ttu-id="98642-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98642-136">Required.</span></span> <span data-ttu-id="98642-137">Идентификатор объекта пользователя, которому принадлежит хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="98642-137">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="98642-138">Получение библиотеки документов, связанной с группой</span><span class="sxs-lookup"><span data-stu-id="98642-138">Get the document library associated with a group</span></span>

<span data-ttu-id="98642-139">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для группы, ваше приложение должно запросить связь **drive** в объекте Group.</span><span class="sxs-lookup"><span data-stu-id="98642-139">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="98642-140">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98642-140">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="98642-141">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="98642-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="98642-142">C#</span><span class="sxs-lookup"><span data-stu-id="98642-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="98642-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="98642-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="98642-144">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="98642-144">Path parameters</span></span>

| <span data-ttu-id="98642-145">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="98642-145">Parameter name</span></span> | <span data-ttu-id="98642-146">Значение</span><span class="sxs-lookup"><span data-stu-id="98642-146">Value</span></span>  | <span data-ttu-id="98642-147">Описание</span><span class="sxs-lookup"><span data-stu-id="98642-147">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="98642-148">_groupId_</span><span class="sxs-lookup"><span data-stu-id="98642-148">_groupId_</span></span>      | <span data-ttu-id="98642-149">строка</span><span class="sxs-lookup"><span data-stu-id="98642-149">string</span></span> | <span data-ttu-id="98642-150">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98642-150">Required.</span></span> <span data-ttu-id="98642-151">Идентификатор группы, которой принадлежит библиотека документов.</span><span class="sxs-lookup"><span data-stu-id="98642-151">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="98642-152">Получение библиотеки документов для сайта</span><span class="sxs-lookup"><span data-stu-id="98642-152">Get the document library for a site</span></span>

<span data-ttu-id="98642-153">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для [сайта](../resources/site.md), ваше приложение должно запросить связь **drive** в объекте Site.</span><span class="sxs-lookup"><span data-stu-id="98642-153">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="98642-154">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98642-154">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="98642-155">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="98642-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="98642-156">C#</span><span class="sxs-lookup"><span data-stu-id="98642-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="98642-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="98642-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="98642-158">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="98642-158">Path parameters</span></span>

| <span data-ttu-id="98642-159">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="98642-159">Parameter name</span></span> | <span data-ttu-id="98642-160">Значение</span><span class="sxs-lookup"><span data-stu-id="98642-160">Value</span></span>  | <span data-ttu-id="98642-161">Описание</span><span class="sxs-lookup"><span data-stu-id="98642-161">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="98642-162">_siteId_</span><span class="sxs-lookup"><span data-stu-id="98642-162">_siteId_</span></span>       | <span data-ttu-id="98642-163">строка</span><span class="sxs-lookup"><span data-stu-id="98642-163">string</span></span> | <span data-ttu-id="98642-164">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98642-164">Required.</span></span> <span data-ttu-id="98642-165">Идентификатор для сайта, который содержит библиотеку документов.</span><span class="sxs-lookup"><span data-stu-id="98642-165">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="98642-166">Получение диска с использованием его идентификатора</span><span class="sxs-lookup"><span data-stu-id="98642-166">Get a drive by ID</span></span>

<span data-ttu-id="98642-167">Если у вас есть уникальный идентификатор диска, вы можете получить доступ к этому диску непосредственно из коллекции дисков верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="98642-167">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="98642-168">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98642-168">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```

### <a name="path-parameters"></a><span data-ttu-id="98642-169">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="98642-169">Path parameters</span></span>

| <span data-ttu-id="98642-170">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="98642-170">Parameter name</span></span> | <span data-ttu-id="98642-171">Значение</span><span class="sxs-lookup"><span data-stu-id="98642-171">Value</span></span>  | <span data-ttu-id="98642-172">Описание</span><span class="sxs-lookup"><span data-stu-id="98642-172">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="98642-173">_driveId_</span><span class="sxs-lookup"><span data-stu-id="98642-173">_driveId_</span></span>      | <span data-ttu-id="98642-174">string</span><span class="sxs-lookup"><span data-stu-id="98642-174">string</span></span> | <span data-ttu-id="98642-p105">Обязательный. Идентификатор запрошенного диска.</span><span class="sxs-lookup"><span data-stu-id="98642-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="98642-177">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="98642-177">Optional query parameters</span></span>

<span data-ttu-id="98642-178">Эти методы поддерживают [параметр запроса $select][odata-query-parameters] для формирования ответа.</span><span class="sxs-lookup"><span data-stu-id="98642-178">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="98642-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="98642-179">Response</span></span>

<span data-ttu-id="98642-180">Каждый из этих методов возвращает [ресурс Drive][drive-resource] для соответствующего диска в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="98642-180">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="98642-181">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="98642-181">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="98642-182">C#</span><span class="sxs-lookup"><span data-stu-id="98642-182">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="98642-183">Javascript</span><span class="sxs-lookup"><span data-stu-id="98642-183">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="error-response-codes"></a><span data-ttu-id="98642-184">Коды ответов с ошибками</span><span class="sxs-lookup"><span data-stu-id="98642-184">Error response codes</span></span>

<span data-ttu-id="98642-185">Если диск не существует, и не удается подготовить его к работе автоматически (при использовании делегированной проверки подлинности), будет возвращен ответ `HTTP 404`.</span><span class="sxs-lookup"><span data-stu-id="98642-185">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

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
