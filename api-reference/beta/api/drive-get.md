---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение доступа к ресурсу Drive
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: f1fd3b48646c0df4a982652545e8494839f40c02
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589656"
---
# <a name="get-drive"></a><span data-ttu-id="7aa38-102">Получение ресурса Drive</span><span class="sxs-lookup"><span data-stu-id="7aa38-102">Get Drive</span></span>

<span data-ttu-id="7aa38-103">В этой статье рассказывается, как получить свойства и связи ресурса [Drive](../resources/drive.md).</span><span class="sxs-lookup"><span data-stu-id="7aa38-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="7aa38-104">Drive — это контейнер верхнего уровня для файловой системы, например OneDrive или библиотек документов SharePoint.</span><span class="sxs-lookup"><span data-stu-id="7aa38-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="7aa38-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7aa38-105">Permissions</span></span>

<span data-ttu-id="7aa38-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7aa38-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7aa38-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7aa38-108">Permission type</span></span>      | <span data-ttu-id="7aa38-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7aa38-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7aa38-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7aa38-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7aa38-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aa38-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7aa38-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7aa38-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7aa38-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aa38-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="7aa38-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7aa38-114">Application</span></span> | <span data-ttu-id="7aa38-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aa38-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="7aa38-116">Получение хранилища OneDrive текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="7aa38-116">Get current user's OneDrive</span></span>

<span data-ttu-id="7aa38-117">Доступ к диску пользователя, выполнившего вход в систему (при использовании делегированной проверки подлинности), можно получить из одноэлементного множества `me`.</span><span class="sxs-lookup"><span data-stu-id="7aa38-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="7aa38-118">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="7aa38-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="7aa38-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7aa38-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7aa38-120">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="7aa38-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7aa38-121">Языках</span><span class="sxs-lookup"><span data-stu-id="7aa38-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7aa38-122">Язык</span><span class="sxs-lookup"><span data-stu-id="7aa38-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-default-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="get-a-users-onedrive"></a><span data-ttu-id="7aa38-123">Получение хранилища OneDrive пользователя</span><span class="sxs-lookup"><span data-stu-id="7aa38-123">Get a user's OneDrive</span></span>

<span data-ttu-id="7aa38-124">Чтобы получить доступ к хранилищу OneDrive или OneDrive для бизнеса пользователя, ваше приложение должно запросить связь **drive** в ресурсе User.</span><span class="sxs-lookup"><span data-stu-id="7aa38-124">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="7aa38-125">Если хранилище OneDrive пользователя не подготовлено к работе, но у пользователя есть лицензия на использование OneDrive, то в результате выполнения этого запроса будет автоматически подготовлен диск пользователя (при использовании делегированной проверки подлинности).</span><span class="sxs-lookup"><span data-stu-id="7aa38-125">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="7aa38-126">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7aa38-126">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7aa38-127">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="7aa38-127">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7aa38-128">Языках</span><span class="sxs-lookup"><span data-stu-id="7aa38-128">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7aa38-129">Язык</span><span class="sxs-lookup"><span data-stu-id="7aa38-129">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="7aa38-130">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="7aa38-130">Path parameters</span></span>

| <span data-ttu-id="7aa38-131">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="7aa38-131">Parameter name</span></span> | <span data-ttu-id="7aa38-132">Значение</span><span class="sxs-lookup"><span data-stu-id="7aa38-132">Value</span></span>  | <span data-ttu-id="7aa38-133">Описание</span><span class="sxs-lookup"><span data-stu-id="7aa38-133">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="7aa38-134">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="7aa38-134">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="7aa38-135">строка</span><span class="sxs-lookup"><span data-stu-id="7aa38-135">string</span></span> | <span data-ttu-id="7aa38-136">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7aa38-136">Required.</span></span> <span data-ttu-id="7aa38-137">Идентификатор объекта пользователя, которому принадлежит хранилище OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7aa38-137">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="7aa38-138">Получение библиотеки документов, связанной с группой</span><span class="sxs-lookup"><span data-stu-id="7aa38-138">Get the document library associated with a group</span></span>

<span data-ttu-id="7aa38-139">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для группы, ваше приложение должно запросить связь **drive** в объекте Group.</span><span class="sxs-lookup"><span data-stu-id="7aa38-139">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="7aa38-140">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7aa38-140">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="7aa38-141">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="7aa38-141">Path parameters</span></span>

| <span data-ttu-id="7aa38-142">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="7aa38-142">Parameter name</span></span> | <span data-ttu-id="7aa38-143">Значение</span><span class="sxs-lookup"><span data-stu-id="7aa38-143">Value</span></span>  | <span data-ttu-id="7aa38-144">Описание</span><span class="sxs-lookup"><span data-stu-id="7aa38-144">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="7aa38-145">_groupId_</span><span class="sxs-lookup"><span data-stu-id="7aa38-145">_groupId_</span></span>      | <span data-ttu-id="7aa38-146">строка</span><span class="sxs-lookup"><span data-stu-id="7aa38-146">string</span></span> | <span data-ttu-id="7aa38-147">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7aa38-147">Required.</span></span> <span data-ttu-id="7aa38-148">Идентификатор группы, которой принадлежит библиотека документов.</span><span class="sxs-lookup"><span data-stu-id="7aa38-148">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="7aa38-149">Получение библиотеки документов для сайта</span><span class="sxs-lookup"><span data-stu-id="7aa38-149">Get the document library for a site</span></span>

<span data-ttu-id="7aa38-150">Чтобы получить доступ к библиотеке документов, используемой по умолчанию, для [сайта](../resources/site.md), ваше приложение должно запросить связь **drive** в объекте Site.</span><span class="sxs-lookup"><span data-stu-id="7aa38-150">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="7aa38-151">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7aa38-151">HTTP request</span></span>

```http
GET /sites/{siteId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7aa38-152">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="7aa38-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7aa38-153">Языках</span><span class="sxs-lookup"><span data-stu-id="7aa38-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7aa38-154">Язык</span><span class="sxs-lookup"><span data-stu-id="7aa38-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="7aa38-155">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="7aa38-155">Path parameters</span></span>

| <span data-ttu-id="7aa38-156">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="7aa38-156">Parameter name</span></span> | <span data-ttu-id="7aa38-157">Значение</span><span class="sxs-lookup"><span data-stu-id="7aa38-157">Value</span></span>  | <span data-ttu-id="7aa38-158">Описание</span><span class="sxs-lookup"><span data-stu-id="7aa38-158">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="7aa38-159">_siteId_</span><span class="sxs-lookup"><span data-stu-id="7aa38-159">_siteId_</span></span>       | <span data-ttu-id="7aa38-160">строка</span><span class="sxs-lookup"><span data-stu-id="7aa38-160">string</span></span> | <span data-ttu-id="7aa38-161">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7aa38-161">Required.</span></span> <span data-ttu-id="7aa38-162">Идентификатор для сайта, который содержит библиотеку документов.</span><span class="sxs-lookup"><span data-stu-id="7aa38-162">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="7aa38-163">Получение диска с использованием его идентификатора</span><span class="sxs-lookup"><span data-stu-id="7aa38-163">Get a drive by ID</span></span>

<span data-ttu-id="7aa38-164">Если у вас есть уникальный идентификатор диска, вы можете получить доступ к этому диску непосредственно из коллекции дисков верхнего уровня.</span><span class="sxs-lookup"><span data-stu-id="7aa38-164">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="7aa38-165">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7aa38-165">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}
```

### <a name="path-parameters"></a><span data-ttu-id="7aa38-166">Параметры пути</span><span class="sxs-lookup"><span data-stu-id="7aa38-166">Path parameters</span></span>

| <span data-ttu-id="7aa38-167">Имя параметра</span><span class="sxs-lookup"><span data-stu-id="7aa38-167">Parameter name</span></span> | <span data-ttu-id="7aa38-168">Значение</span><span class="sxs-lookup"><span data-stu-id="7aa38-168">Value</span></span>  | <span data-ttu-id="7aa38-169">Описание</span><span class="sxs-lookup"><span data-stu-id="7aa38-169">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="7aa38-170">_driveId_</span><span class="sxs-lookup"><span data-stu-id="7aa38-170">_driveId_</span></span>      | <span data-ttu-id="7aa38-171">string</span><span class="sxs-lookup"><span data-stu-id="7aa38-171">string</span></span> | <span data-ttu-id="7aa38-p105">Обязательный. Идентификатор запрошенного диска.</span><span class="sxs-lookup"><span data-stu-id="7aa38-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="7aa38-174">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="7aa38-174">Optional query parameters</span></span>

<span data-ttu-id="7aa38-175">Эти методы поддерживают [параметр запроса $select][odata-query-parameters] для формирования ответа.</span><span class="sxs-lookup"><span data-stu-id="7aa38-175">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="7aa38-176">Отклик</span><span class="sxs-lookup"><span data-stu-id="7aa38-176">Response</span></span>

<span data-ttu-id="7aa38-177">Каждый из этих методов возвращает [ресурс Drive][drive-resource] для соответствующего диска в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="7aa38-177">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default"] } -->

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="7aa38-178">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="7aa38-178">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7aa38-179">Языках</span><span class="sxs-lookup"><span data-stu-id="7aa38-179">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7aa38-180">Язык</span><span class="sxs-lookup"><span data-stu-id="7aa38-180">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="error-response-codes"></a><span data-ttu-id="7aa38-181">Коды ответов с ошибками</span><span class="sxs-lookup"><span data-stu-id="7aa38-181">Error response codes</span></span>

<span data-ttu-id="7aa38-182">Если диск не существует, и не удается подготовить его к работе автоматически (при использовании делегированной проверки подлинности), будет возвращен ответ `HTTP 404`.</span><span class="sxs-lookup"><span data-stu-id="7aa38-182">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

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
