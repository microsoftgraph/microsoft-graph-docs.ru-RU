---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Предоставление доступа к файлу посредством ссылки
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: da6b1972d029b9e780575b1bf985f4d3c9d6d906
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260237"
---
# <a name="create-a-sharing-link-for-a-driveitem"></a><span data-ttu-id="8962c-102">Создание ссылки совместного доступа для ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="8962c-102">Create a sharing link for a DriveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8962c-103">Используя действие **createLink**, вы можете поделиться ресурсом [DriveItem](../resources/driveitem.md) с помощью ссылки для совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="8962c-103">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="8962c-p101">Действие **createLink** создает ссылку для совместного доступа, если ссылка указанного типа еще не существует для приложения, совершающего вызов. Если для приложения уже создана такая ссылка указанного типа, возвращается она.</span><span class="sxs-lookup"><span data-stu-id="8962c-p101">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="8962c-106">Ресурсы DriveItem наследуют разрешения совместного доступа от своих предков.</span><span class="sxs-lookup"><span data-stu-id="8962c-106">DriveItem resources inherit sharing permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="8962c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8962c-107">Permissions</span></span>

<span data-ttu-id="8962c-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8962c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8962c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8962c-110">Permission type</span></span>      | <span data-ttu-id="8962c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8962c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8962c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8962c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8962c-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8962c-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8962c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8962c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8962c-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8962c-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8962c-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8962c-116">Application</span></span> | <span data-ttu-id="8962c-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8962c-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8962c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8962c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```

### <a name="request-body"></a><span data-ttu-id="8962c-119">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="8962c-119">Request body</span></span>

<span data-ttu-id="8962c-120">В теле запроса определяются свойства ссылки для совместного доступа, запрашиваемой приложением.</span><span class="sxs-lookup"><span data-stu-id="8962c-120">The body of the request defines properties of the sharing link your application is requesting.</span></span>
<span data-ttu-id="8962c-121">Запрос должен быть объектом JSON с указанными ниже свойствами.</span><span class="sxs-lookup"><span data-stu-id="8962c-121">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="8962c-122">Имя</span><span class="sxs-lookup"><span data-stu-id="8962c-122">Name</span></span>    |  <span data-ttu-id="8962c-123">Тип</span><span class="sxs-lookup"><span data-stu-id="8962c-123">Type</span></span>  |                                 <span data-ttu-id="8962c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="8962c-124">Description</span></span>                                  |
| :-------- | :----- | :--------------------------------------------------------------------------- |
| <span data-ttu-id="8962c-125">**type**</span><span class="sxs-lookup"><span data-stu-id="8962c-125">**type**</span></span>  | <span data-ttu-id="8962c-126">string</span><span class="sxs-lookup"><span data-stu-id="8962c-126">string</span></span> | <span data-ttu-id="8962c-p104">Тип создаваемой ссылки для совместного доступа. Возможные значения: `view`, `edit` или `embed`.</span><span class="sxs-lookup"><span data-stu-id="8962c-p104">The type of sharing link to create. Either `view`, `edit`, or `embed`.</span></span>       |
| <span data-ttu-id="8962c-129">**scope**</span><span class="sxs-lookup"><span data-stu-id="8962c-129">**scope**</span></span> | <span data-ttu-id="8962c-130">string</span><span class="sxs-lookup"><span data-stu-id="8962c-130">string</span></span> | <span data-ttu-id="8962c-131">Необязательно.</span><span class="sxs-lookup"><span data-stu-id="8962c-131">Optional.</span></span> <span data-ttu-id="8962c-132">Область создаваемой ссылки.</span><span class="sxs-lookup"><span data-stu-id="8962c-132">The scope of link to create.</span></span> <span data-ttu-id="8962c-133">Возможные значения: `anonymous` или `organization`.</span><span class="sxs-lookup"><span data-stu-id="8962c-133">Either `anonymous` or `organization`.</span></span> |


### <a name="link-types"></a><span data-ttu-id="8962c-134">Типы ссылок</span><span class="sxs-lookup"><span data-stu-id="8962c-134">Link types</span></span>

<span data-ttu-id="8962c-135">Параметр **type** может принимать указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="8962c-135">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="8962c-136">Значение типа</span><span class="sxs-lookup"><span data-stu-id="8962c-136">Type value</span></span> | <span data-ttu-id="8962c-137">Описание</span><span class="sxs-lookup"><span data-stu-id="8962c-137">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | <span data-ttu-id="8962c-138">Создает ссылку на объект DriveItem, предполагающую доступ только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8962c-138">Creates a read-only link to the DriveItem.</span></span>                                                        |
| `edit`     | <span data-ttu-id="8962c-139">Создает ссылку на объект DriveItem, предполагающую доступ для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="8962c-139">Creates a read-write link to the DriveItem.</span></span>                                                       |
| `embed`    | <span data-ttu-id="8962c-140">Создает встраиваемую ссылку на объект DriveItem.</span><span class="sxs-lookup"><span data-stu-id="8962c-140">Creates an embeddable link to the DriveItem.</span></span> <span data-ttu-id="8962c-141">Этот вариант доступен только для файлов в личных учетных записях OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8962c-141">This option is only available for files in OneDrive personal.</span></span> |

### <a name="scope-types"></a><span data-ttu-id="8962c-142">Типы областей</span><span class="sxs-lookup"><span data-stu-id="8962c-142">Scope types</span></span>

<span data-ttu-id="8962c-143">Параметр **scope** может принимать указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="8962c-143">The following values are allowed for the **scope** parameter.</span></span>
<span data-ttu-id="8962c-144">Если параметр **scope** не задан, создается ссылка того типа, который используется в организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8962c-144">If the **scope** parameter is not specified, the default link type for the organization is created.</span></span>

| <span data-ttu-id="8962c-145">Значение типа</span><span class="sxs-lookup"><span data-stu-id="8962c-145">Type value</span></span>     | <span data-ttu-id="8962c-146">Описание</span><span class="sxs-lookup"><span data-stu-id="8962c-146">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="8962c-147">Создает ссылку на объект DriveItem, доступный всем, кому она предоставлена.</span><span class="sxs-lookup"><span data-stu-id="8962c-147">Creates a link to the DriveItem accessible to anyone with the link.</span></span> <span data-ttu-id="8962c-148">Администратор может отключить ссылки, не требующие проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="8962c-148">Anonymous links may be disabled by an administrator.</span></span>                 |
| `organization` | <span data-ttu-id="8962c-149">Создает ссылку на объект DriveItem, доступный всем в организации пользователя.</span><span class="sxs-lookup"><span data-stu-id="8962c-149">Creates a link to the DriveItem accessible to anyone within the user's organization.</span></span> <span data-ttu-id="8962c-150">Область организации для ссылок недоступна в личных учетных записях OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8962c-150">Organization link scope is not available for OneDrive personal.</span></span> |

## <a name="response"></a><span data-ttu-id="8962c-151">Ответ</span><span class="sxs-lookup"><span data-stu-id="8962c-151">Response</span></span>

<span data-ttu-id="8962c-152">В случае успешного выполнения этот метод возвращает в тексте ответа один ресурс [Permission](../resources/permission.md), представляющий запрашиваемые разрешения для совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="8962c-152">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing permissions.</span></span>

<span data-ttu-id="8962c-153">Если для элемента создается новая ссылка совместного доступа, возвращается код ответа `201 Created`, а если возвращается существующая ссылка — код `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="8962c-153">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="example"></a><span data-ttu-id="8962c-154">Пример</span><span class="sxs-lookup"><span data-stu-id="8962c-154">Example</span></span>

<span data-ttu-id="8962c-155">В приведенном ниже примере запрашивается создание ссылки для совместного доступа к объекту DriveItem, указанному по {itemId}, в хранилище OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="8962c-155">The following example requests a sharing link to be created for the DriveItem specified by {itemId} in the user's OneDrive.</span></span>
<span data-ttu-id="8962c-156">Ссылка для совместного доступа подразумевает доступ только для чтения, и ее может использовать каждый, кому она предоставлена.</span><span class="sxs-lookup"><span data-stu-id="8962c-156">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

### <a name="request"></a><span data-ttu-id="8962c-157">Запрос</span><span class="sxs-lookup"><span data-stu-id="8962c-157">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "item_createlink"
}-->

```http
POST /me/drive/items/{itemId}/createLink
Content-type: application/json

{
  "type": "view",
  "scope": "anonymous"
}
```

### <a name="response"></a><span data-ttu-id="8962c-158">Отклик</span><span class="sxs-lookup"><span data-stu-id="8962c-158">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8962c-159">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="8962c-159">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8962c-160">C#</span><span class="sxs-lookup"><span data-stu-id="8962c-160">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/item_createlink-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8962c-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="8962c-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/item_createlink-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8962c-162">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8962c-162">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/item_createlink-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="creating-company-sharable-links"></a><span data-ttu-id="8962c-163">Создание ссылок с возможностью общего доступа в компании</span><span class="sxs-lookup"><span data-stu-id="8962c-163">Creating company sharable links</span></span>

<span data-ttu-id="8962c-164">OneDrive для бизнеса и SharePoint поддерживают ссылки с возможностью общего доступа в компании.</span><span class="sxs-lookup"><span data-stu-id="8962c-164">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="8962c-165">Они аналогичны ссылкам, не требующим проверки подлинности, но работают только для элементов соответствующей организации.</span><span class="sxs-lookup"><span data-stu-id="8962c-165">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="8962c-166">Чтобы создать такую ссылку, задайте для параметра **scope** значение `organization`.</span><span class="sxs-lookup"><span data-stu-id="8962c-166">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

### <a name="request"></a><span data-ttu-id="8962c-167">Запрос</span><span class="sxs-lookup"><span data-stu-id="8962c-167">Request</span></span>

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

### <a name="response"></a><span data-ttu-id="8962c-168">Отклик</span><span class="sxs-lookup"><span data-stu-id="8962c-168">Response</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="8962c-169">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="8962c-169">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8962c-170">C#</span><span class="sxs-lookup"><span data-stu-id="8962c-170">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create-link-scoped-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8962c-171">Javascript</span><span class="sxs-lookup"><span data-stu-id="8962c-171">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-link-scoped-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8962c-172">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8962c-172">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create-link-scoped-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="creating-embeddable-links"></a><span data-ttu-id="8962c-173">Создание встраиваемых ссылок</span><span class="sxs-lookup"><span data-stu-id="8962c-173">Creating embeddable links</span></span>

<span data-ttu-id="8962c-p112">При использовании типа ссылки `embed` возвращаемое значение webUrl можно внедрять в элемент HTML `<iframe>`. При создании встроенной ссылки свойство `webHtml` содержит HTML-код для объекта `<iframe>`, в котором размещается содержимое.</span><span class="sxs-lookup"><span data-stu-id="8962c-p112">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

<span data-ttu-id="8962c-176">**Примечание.** Внедрение ссылок поддерживается только в личных учетных записях OneDrive.</span><span class="sxs-lookup"><span data-stu-id="8962c-176">**Note:** Embed links are only supported for OneDrive personal.</span></span>

### <a name="request"></a><span data-ttu-id="8962c-177">Запрос</span><span class="sxs-lookup"><span data-stu-id="8962c-177">Request</span></span>

<!-- { "blockType": "request", "name": "create-embedded-link", "scopes": "files.readwrite service.onedrive" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```

### <a name="response"></a><span data-ttu-id="8962c-178">Отклик</span><span class="sxs-lookup"><span data-stu-id="8962c-178">Response</span></span>

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
    "webUrl": "https://onedive.live.com/...",
    "application": {
      "id": "1234",
      "displayName": "Sample Application"
    },
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8962c-179">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="8962c-179">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8962c-180">C#</span><span class="sxs-lookup"><span data-stu-id="8962c-180">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create-embedded-link-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8962c-181">Javascript</span><span class="sxs-lookup"><span data-stu-id="8962c-181">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create-embedded-link-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8962c-182">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8962c-182">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create-embedded-link-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="8962c-183">Примечания</span><span class="sxs-lookup"><span data-stu-id="8962c-183">Remarks</span></span>

* <span data-ttu-id="8962c-184">Срок действия ссылок, созданных с помощью этого действия, не истекает при условии, что в организации не включена политика срока действия.</span><span class="sxs-lookup"><span data-stu-id="8962c-184">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="8962c-185">Ссылки отображаются в разрешениях на совместное использование для элемента и могут быть удалены владельцем элемента.</span><span class="sxs-lookup"><span data-stu-id="8962c-185">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="8962c-186">Они всегда указывают на текущую версию элемента, если он не был извлечен (только в SharePoint).</span><span class="sxs-lookup"><span data-stu-id="8962c-186">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-createlink.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/driveitem-createlink.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-createlink.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/driveitem-createlink.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-createlink.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/driveitem-createlink.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/driveitem-createlink.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
