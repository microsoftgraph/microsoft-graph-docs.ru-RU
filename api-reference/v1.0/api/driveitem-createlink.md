---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Предоставление доступа к файлу посредством ссылки
localization_priority: Normal
ms.prod: sharepoint
description: Используя действие createLink, вы можете поделиться ресурсом DriveItem с помощью ссылки для совместного доступа.
doc_type: apiPageType
ms.openlocfilehash: 29d29e476a3991fd725d1c1774ac90725436b8db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517785"
---
# <a name="create-a-sharing-link-for-a-driveitem"></a><span data-ttu-id="49084-103">Создание ссылки для доступа к ресурсу DriveItem</span><span class="sxs-lookup"><span data-stu-id="49084-103">Create a sharing link for a DriveItem</span></span>

<span data-ttu-id="49084-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49084-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="49084-105">Используя действие **createLink**, вы можете поделиться ресурсом [DriveItem](../resources/driveitem.md) с помощью ссылки для совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="49084-105">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="49084-p101">Действие **createLink** создает ссылку для совместного доступа, если ссылка указанного типа еще не существует для приложения, совершающего вызов. Если для приложения уже создана такая ссылка указанного типа, возвращается она.</span><span class="sxs-lookup"><span data-stu-id="49084-p101">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="49084-108">Ресурсы DriveItem наследуют разрешения совместного доступа от своих предков.</span><span class="sxs-lookup"><span data-stu-id="49084-108">DriveItem resources inherit sharing permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="49084-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="49084-109">Permissions</span></span>

<span data-ttu-id="49084-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="49084-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49084-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="49084-112">Permission type</span></span>      | <span data-ttu-id="49084-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="49084-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49084-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="49084-114">Delegated (work or school account)</span></span> | <span data-ttu-id="49084-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49084-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="49084-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="49084-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49084-117">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49084-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="49084-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="49084-118">Application</span></span> | <span data-ttu-id="49084-119">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49084-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49084-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="49084-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```

### <a name="request-body"></a><span data-ttu-id="49084-121">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="49084-121">Request body</span></span>

<span data-ttu-id="49084-122">В теле запроса определяются свойства ссылки для совместного доступа, запрашиваемой приложением.</span><span class="sxs-lookup"><span data-stu-id="49084-122">The body of the request defines properties of the sharing link your application is requesting.</span></span>
<span data-ttu-id="49084-123">Запрос должен быть объектом JSON с указанными ниже свойствами.</span><span class="sxs-lookup"><span data-stu-id="49084-123">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="49084-124">Имя</span><span class="sxs-lookup"><span data-stu-id="49084-124">Name</span></span>    |  <span data-ttu-id="49084-125">Тип</span><span class="sxs-lookup"><span data-stu-id="49084-125">Type</span></span>  |                                 <span data-ttu-id="49084-126">Описание</span><span class="sxs-lookup"><span data-stu-id="49084-126">Description</span></span>                                  |
| :-------- | :----- | :--------------------------------------------------------------------------- |
| <span data-ttu-id="49084-127">**type**</span><span class="sxs-lookup"><span data-stu-id="49084-127">**type**</span></span>  | <span data-ttu-id="49084-128">string</span><span class="sxs-lookup"><span data-stu-id="49084-128">string</span></span> | <span data-ttu-id="49084-p104">Тип создаваемой ссылки для совместного доступа. Возможные значения: `view`, `edit` или `embed`.</span><span class="sxs-lookup"><span data-stu-id="49084-p104">The type of sharing link to create. Either `view`, `edit`, or `embed`.</span></span>       |
| <span data-ttu-id="49084-131">**scope**</span><span class="sxs-lookup"><span data-stu-id="49084-131">**scope**</span></span> | <span data-ttu-id="49084-132">string</span><span class="sxs-lookup"><span data-stu-id="49084-132">string</span></span> | <span data-ttu-id="49084-133">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="49084-133">Optional.</span></span> <span data-ttu-id="49084-134">Область создаваемой ссылки.</span><span class="sxs-lookup"><span data-stu-id="49084-134">The scope of link to create.</span></span> <span data-ttu-id="49084-135">Возможные значения: `anonymous` или `organization`.</span><span class="sxs-lookup"><span data-stu-id="49084-135">Either `anonymous` or `organization`.</span></span> |


### <a name="link-types"></a><span data-ttu-id="49084-136">Типы ссылок</span><span class="sxs-lookup"><span data-stu-id="49084-136">Link types</span></span>

<span data-ttu-id="49084-137">Параметр **type** может принимать указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="49084-137">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="49084-138">Значение типа</span><span class="sxs-lookup"><span data-stu-id="49084-138">Type value</span></span> | <span data-ttu-id="49084-139">Описание</span><span class="sxs-lookup"><span data-stu-id="49084-139">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | <span data-ttu-id="49084-140">Создает ссылку на объект DriveItem, предполагающую доступ только для чтения.</span><span class="sxs-lookup"><span data-stu-id="49084-140">Creates a read-only link to the DriveItem.</span></span>                                                        |
| `edit`     | <span data-ttu-id="49084-141">Создает ссылку на объект DriveItem, предполагающую доступ для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="49084-141">Creates a read-write link to the DriveItem.</span></span>                                                       |
| `embed`    | <span data-ttu-id="49084-142">Создает встраиваемую ссылку на объект DriveItem.</span><span class="sxs-lookup"><span data-stu-id="49084-142">Creates an embeddable link to the DriveItem.</span></span> <span data-ttu-id="49084-143">Этот вариант доступен только для файлов в личных учетных записях OneDrive.</span><span class="sxs-lookup"><span data-stu-id="49084-143">This option is only available for files in OneDrive personal.</span></span> |

### <a name="scope-types"></a><span data-ttu-id="49084-144">Типы областей</span><span class="sxs-lookup"><span data-stu-id="49084-144">Scope types</span></span>

<span data-ttu-id="49084-145">Параметр **scope** может принимать указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="49084-145">The following values are allowed for the **scope** parameter.</span></span>
<span data-ttu-id="49084-146">Если параметр **scope** не задан, создается ссылка того типа, который используется в организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="49084-146">If the **scope** parameter is not specified, the default link type for the organization is created.</span></span>

| <span data-ttu-id="49084-147">Значение</span><span class="sxs-lookup"><span data-stu-id="49084-147">Value</span></span>          | <span data-ttu-id="49084-148">Описание</span><span class="sxs-lookup"><span data-stu-id="49084-148">Description</span></span>
|:---------------|:------------------------------------------------------------
| `anonymous`    | <span data-ttu-id="49084-149">Любой пользователь со ссылкой обладает правом доступа без необходимости входа в систему.</span><span class="sxs-lookup"><span data-stu-id="49084-149">Anyone with the link has access, without needing to sign in.</span></span> <span data-ttu-id="49084-150">Это также относится к людям вне вашей организации.</span><span class="sxs-lookup"><span data-stu-id="49084-150">This may include people outside of your organization.</span></span> <span data-ttu-id="49084-151">Администратор может отключить поддержку ссылок, не требующих проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="49084-151">Anonymous link support may be disabled by an administrator.</span></span>
| `organization` | <span data-ttu-id="49084-152">Любой пользователь, вошедший в вашу организацию (клиент), может использовать ссылку для получения доступа.</span><span class="sxs-lookup"><span data-stu-id="49084-152">Anyone signed into your organization (tenant) can use the link to get access.</span></span> <span data-ttu-id="49084-153">Доступно только в OneDrive для бизнеса и SharePoint.</span><span class="sxs-lookup"><span data-stu-id="49084-153">Only available in OneDrive for Business and SharePoint.</span></span>


## <a name="response"></a><span data-ttu-id="49084-154">Отклик</span><span class="sxs-lookup"><span data-stu-id="49084-154">Response</span></span>

<span data-ttu-id="49084-155">В случае успешного выполнения этот метод возвращает в тексте ответа один ресурс [Permission](../resources/permission.md), представляющий запрашиваемые разрешения для совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="49084-155">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing permissions.</span></span>

<span data-ttu-id="49084-156">Если для элемента создается новая ссылка совместного доступа, возвращается код ответа `201 Created`, а если возвращается существующая ссылка — код `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="49084-156">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="example"></a><span data-ttu-id="49084-157">Пример</span><span class="sxs-lookup"><span data-stu-id="49084-157">Example</span></span>

<span data-ttu-id="49084-158">В приведенном ниже примере запрашивается создание ссылки для совместного доступа к объекту DriveItem, указанному по {itemId}, в хранилище OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="49084-158">The following example requests a sharing link to be created for the DriveItem specified by {itemId} in the user's OneDrive.</span></span>
<span data-ttu-id="49084-159">Ссылка для совместного доступа подразумевает доступ только для чтения, и ее может использовать каждый, кому она предоставлена.</span><span class="sxs-lookup"><span data-stu-id="49084-159">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

### <a name="request"></a><span data-ttu-id="49084-160">Запрос</span><span class="sxs-lookup"><span data-stu-id="49084-160">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="49084-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="49084-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create-link"
}-->

```http
POST /me/drive/items/{item-id}/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```
# <a name="c"></a>[<span data-ttu-id="49084-162">C#</span><span class="sxs-lookup"><span data-stu-id="49084-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-link-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49084-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49084-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-link-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49084-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49084-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-link-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49084-165">Java</span><span class="sxs-lookup"><span data-stu-id="49084-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-link-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="49084-166">Отклик</span><span class="sxs-lookup"><span data-stu-id="49084-166">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "view",
    "scope": "anonymous",
    "webUrl": "https://1drv.ms/A6913278E564460AA616C71B28AD6EB6",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-company-sharable-links"></a><span data-ttu-id="49084-167">Создание ссылок с возможностью общего доступа в компании</span><span class="sxs-lookup"><span data-stu-id="49084-167">Creating company sharable links</span></span>

<span data-ttu-id="49084-168">OneDrive для бизнеса и SharePoint поддерживают ссылки с возможностью общего доступа в компании.</span><span class="sxs-lookup"><span data-stu-id="49084-168">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="49084-169">Они аналогичны ссылкам, не требующим проверки подлинности, но работают только для элементов соответствующей организации.</span><span class="sxs-lookup"><span data-stu-id="49084-169">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="49084-170">Чтобы создать такую ссылку, задайте для параметра **scope** значение `organization`.</span><span class="sxs-lookup"><span data-stu-id="49084-170">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

### <a name="request"></a><span data-ttu-id="49084-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="49084-171">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="49084-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="49084-172">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite", "tags": "service.sharepoint" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```
# <a name="c"></a>[<span data-ttu-id="49084-173">C#</span><span class="sxs-lookup"><span data-stu-id="49084-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-link-scoped-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49084-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49084-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-link-scoped-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49084-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49084-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-link-scoped-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49084-176">Java</span><span class="sxs-lookup"><span data-stu-id="49084-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-link-scoped-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="49084-177">Ответ</span><span class="sxs-lookup"><span data-stu-id="49084-177">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["write"],
  "link": {
    "type": "edit",
    "scope": "organization",
    "webUrl": "https://contoso-my.sharepoint.com/personal/ellen_contoso_com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="creating-embeddable-links"></a><span data-ttu-id="49084-178">Создание встраиваемых ссылок</span><span class="sxs-lookup"><span data-stu-id="49084-178">Creating embeddable links</span></span>

<span data-ttu-id="49084-p112">При использовании типа ссылки `embed` возвращаемое значение webUrl можно внедрять в элемент HTML `<iframe>`. При создании встроенной ссылки свойство `webHtml` содержит HTML-код для объекта `<iframe>`, в котором размещается содержимое.</span><span class="sxs-lookup"><span data-stu-id="49084-p112">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

<span data-ttu-id="49084-181">**Примечание.** Внедрение ссылок поддерживается только в личных учетных записях OneDrive.</span><span class="sxs-lookup"><span data-stu-id="49084-181">**Note:** Embed links are only supported for OneDrive personal.</span></span>

### <a name="request"></a><span data-ttu-id="49084-182">Запрос</span><span class="sxs-lookup"><span data-stu-id="49084-182">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="49084-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="49084-183">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-embedded-link", "scopes": "files.readwrite", "tags": "service.onedrive service.graph" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```
# <a name="c"></a>[<span data-ttu-id="49084-184">C#</span><span class="sxs-lookup"><span data-stu-id="49084-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-embedded-link-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49084-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49084-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-embedded-link-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49084-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49084-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-embedded-link-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="49084-187">Java</span><span class="sxs-lookup"><span data-stu-id="49084-187">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-embedded-link-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="49084-188">Отклик</span><span class="sxs-lookup"><span data-stu-id="49084-188">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.permission" } -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "123ABC",
  "roles": ["read"],
  "link": {
    "type": "embed",
    "webHtml": "<IFRAME src=\"https://onedrive.live.com/...\"></IFRAME>",
    "webUrl": "https://onedrive.live.com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```

## <a name="remarks"></a><span data-ttu-id="49084-189">Примечания</span><span class="sxs-lookup"><span data-stu-id="49084-189">Remarks</span></span>

* <span data-ttu-id="49084-190">Срок действия ссылок, созданных с помощью этого действия, не истекает при условии, что в организации не включена политика срока действия.</span><span class="sxs-lookup"><span data-stu-id="49084-190">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="49084-191">Ссылки отображаются в разрешениях на совместное использование для элемента и могут быть удалены владельцем элемента.</span><span class="sxs-lookup"><span data-stu-id="49084-191">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="49084-192">Они всегда указывают на текущую версию элемента, если он не был извлечен (только в SharePoint).</span><span class="sxs-lookup"><span data-stu-id="49084-192">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
  ]
} -->
