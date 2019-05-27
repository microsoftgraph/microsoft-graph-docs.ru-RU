---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение доступа к ресурсу Drive
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 47d068dd00223513ad0f49a784916e8a8185ea91
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466488"
---
# <a name="get-drive"></a><span data-ttu-id="84191-102">Получение ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="84191-102">Get Drive</span></span>

<span data-ttu-id="84191-103">В этой статье рассказывается, как получить свойства и связи ресурса [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="84191-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="84191-104">Drive — это контейнер верхнего уровня для файловой системы, например OneDrive или библиотек документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="84191-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="84191-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="84191-105">Permissions</span></span>

<span data-ttu-id="84191-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="84191-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84191-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="84191-108">Permission type</span></span>      | <span data-ttu-id="84191-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="84191-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="84191-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="84191-110">Delegated (work or school account)</span></span> | <span data-ttu-id="84191-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84191-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="84191-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="84191-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="84191-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84191-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="84191-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="84191-114">Application</span></span> | <span data-ttu-id="84191-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84191-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="84191-116">Получение хранилища OneDrive текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="84191-116">Get current user's OneDrive</span></span>

<span data-ttu-id="84191-117">Доступ к диску пользователя, выполнившего вход в систему (при использовании делегированной проверки подлинности), можно получить из одноэлементного множества `me`.</span><span class="sxs-lookup"><span data-stu-id="84191-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="84191-118">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="84191-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="84191-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84191-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="84191-120">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="84191-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="84191-121">C#</span><span class="sxs-lookup"><span data-stu-id="84191-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84191-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84191-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-default-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="get-a-users-onedrive"></a><span data-ttu-id="84191-123">Получение хранилища OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="84191-123">Get a user's OneDrive</span></span>

<span data-ttu-id="84191-124">Чтобы получить доступ к хранилищу OneDrive или OneDrive для бизнеса пользователя, ваше приложение должно запросить связь **drive** в ресурсе User.</span><span class="sxs-lookup"><span data-stu-id="84191-124">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="84191-125">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="84191-125">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="84191-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84191-126">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="84191-127">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="84191-127">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="84191-128">C#</span><span class="sxs-lookup"><span data-stu-id="84191-128">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84191-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84191-129">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="84191-130">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="84191-130">Path parameters</span></span>

| <span data-ttu-id="84191-131">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="84191-131">Parameter name</span></span> | <span data-ttu-id="84191-132">Значение</span><span class="sxs-lookup"><span data-stu-id="84191-132">Value</span></span>  | <span data-ttu-id="84191-133">Описание</span><span class="sxs-lookup"><span data-stu-id="84191-133">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="84191-134">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="84191-134">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="84191-135">строка</span><span class="sxs-lookup"><span data-stu-id="84191-135">string</span></span> | <span data-ttu-id="84191-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84191-136">Required.</span></span> <span data-ttu-id="84191-137">Идентификатор объекта пользователя, которому принадлежит хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="84191-137">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="84191-138">Получение библиотеки документов, связанной с группой</span><span class="sxs-lookup"><span data-stu-id="84191-138">Get the document library associated with a group</span></span>

<span data-ttu-id="84191-139">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для группы, ваше приложение должно запросить связь **drive** в объекте Group.</span><span class="sxs-lookup"><span data-stu-id="84191-139">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="84191-140">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84191-140">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="84191-141">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="84191-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="84191-142">C#</span><span class="sxs-lookup"><span data-stu-id="84191-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84191-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84191-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="84191-144">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="84191-144">Path parameters</span></span>

| <span data-ttu-id="84191-145">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="84191-145">Parameter name</span></span> | <span data-ttu-id="84191-146">Значение</span><span class="sxs-lookup"><span data-stu-id="84191-146">Value</span></span>  | <span data-ttu-id="84191-147">Описание</span><span class="sxs-lookup"><span data-stu-id="84191-147">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="84191-148">_groupId_</span><span class="sxs-lookup"><span data-stu-id="84191-148">_groupId_</span></span>      | <span data-ttu-id="84191-149">строка</span><span class="sxs-lookup"><span data-stu-id="84191-149">string</span></span> | <span data-ttu-id="84191-150">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84191-150">Required.</span></span> <span data-ttu-id="84191-151">Идентификатор группы, которой принадлежит библиотека документов.</span><span class="sxs-lookup"><span data-stu-id="84191-151">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="84191-152">Получение библиотеки документов для сайта</span><span class="sxs-lookup"><span data-stu-id="84191-152">Get the document library for a site</span></span>

<span data-ttu-id="84191-153">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для [сайта](../resources/site.md), ваше приложение должно запросить связь **drive** в объекте Site.</span><span class="sxs-lookup"><span data-stu-id="84191-153">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="84191-154">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84191-154">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="84191-155">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="84191-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="84191-156">C#</span><span class="sxs-lookup"><span data-stu-id="84191-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84191-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84191-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="84191-158">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="84191-158">Path parameters</span></span>

| <span data-ttu-id="84191-159">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="84191-159">Parameter name</span></span> | <span data-ttu-id="84191-160">Значение</span><span class="sxs-lookup"><span data-stu-id="84191-160">Value</span></span>  | <span data-ttu-id="84191-161">Описание</span><span class="sxs-lookup"><span data-stu-id="84191-161">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="84191-162">_siteId_</span><span class="sxs-lookup"><span data-stu-id="84191-162">_siteId_</span></span>       | <span data-ttu-id="84191-163">строка</span><span class="sxs-lookup"><span data-stu-id="84191-163">string</span></span> | <span data-ttu-id="84191-164">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="84191-164">Required.</span></span> <span data-ttu-id="84191-165">Идентификатор для сайта, который содержит библиотеку документов.</span><span class="sxs-lookup"><span data-stu-id="84191-165">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="84191-166">Получение диска с использованием его идентификатора</span><span class="sxs-lookup"><span data-stu-id="84191-166">Get a drive by ID</span></span>

<span data-ttu-id="84191-167">Если у вас есть уникальный идентификатор диска, вы можете получить доступ к этому диску непосредственно из коллекции дисков верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="84191-167">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="84191-168">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="84191-168">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}
```

### <a name="path-parameters"></a><span data-ttu-id="84191-169">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="84191-169">Path parameters</span></span>

| <span data-ttu-id="84191-170">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="84191-170">Parameter name</span></span> | <span data-ttu-id="84191-171">Значение</span><span class="sxs-lookup"><span data-stu-id="84191-171">Value</span></span>  | <span data-ttu-id="84191-172">Описание</span><span class="sxs-lookup"><span data-stu-id="84191-172">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="84191-173">_driveId_</span><span class="sxs-lookup"><span data-stu-id="84191-173">_driveId_</span></span>      | <span data-ttu-id="84191-174">string</span><span class="sxs-lookup"><span data-stu-id="84191-174">string</span></span> | <span data-ttu-id="84191-p105">Обязательный. Идентификатор запрошенного диска.</span><span class="sxs-lookup"><span data-stu-id="84191-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="84191-177">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="84191-177">Optional query parameters</span></span>

<span data-ttu-id="84191-178">Эти методы поддерживают [параметр запроса $select][odata-query-parameters] для формирования ответа.</span><span class="sxs-lookup"><span data-stu-id="84191-178">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="84191-179">Отклик</span><span class="sxs-lookup"><span data-stu-id="84191-179">Response</span></span>

<span data-ttu-id="84191-180">Каждый из этих методов возвращает [ресурс Drive][drive-resource] для соответствующего диска в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="84191-180">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="84191-181">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="84191-181">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="84191-182">C#</span><span class="sxs-lookup"><span data-stu-id="84191-182">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="84191-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="84191-183">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="error-response-codes"></a><span data-ttu-id="84191-184">Коды ответов с ошибками</span><span class="sxs-lookup"><span data-stu-id="84191-184">Error response codes</span></span>

<span data-ttu-id="84191-185">Если диск не существует, и не удается подготовить его к работе автоматически (при использовании делегированной проверки подлинности), будет возвращен ответ `HTTP 404`.</span><span class="sxs-lookup"><span data-stu-id="84191-185">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
      "Warning: /api-reference/v1.0/api/drive-get.md:
        Unable to map some markdown elements into schema.
            Unmapped methods:
        get-drive-default, get-drive-by-user, get-drive-by-group, get-drive-by-id
            Unmapped tables:
        Permissions - AuthScopes, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters"
  ],
  "tocPath": "Drives/Get drive"
} -->
