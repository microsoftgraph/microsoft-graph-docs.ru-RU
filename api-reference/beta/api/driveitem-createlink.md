---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Предоставление доступа к файлу посредством ссылки
ms.openlocfilehash: 85621a167d3ec3a8ecf9218ceca79367dade76e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079819"
---
# <a name="create-a-sharing-link-for-a-driveitem"></a><span data-ttu-id="9a438-102">Создание ссылки совместного доступа для ресурса DriveItem</span><span class="sxs-lookup"><span data-stu-id="9a438-102">Create a sharing link for a DriveItem</span></span>

> <span data-ttu-id="9a438-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9a438-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9a438-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9a438-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9a438-105">Используя действие **createLink**, вы можете поделиться ресурсом [DriveItem](../resources/driveitem.md) с помощью ссылки для совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="9a438-105">You can use **createLink** action to share a [DriveItem](../resources/driveitem.md) via a sharing link.</span></span>

<span data-ttu-id="9a438-p102">Действие **createLink** создает ссылку для совместного доступа, если ссылка указанного типа еще не существует для приложения, совершающего вызов. Если для приложения уже создана такая ссылка указанного типа, возвращается она.</span><span class="sxs-lookup"><span data-stu-id="9a438-p102">The **createLink** action will create a new sharing link if the specified link type doesn't already exist for the calling application. If a sharing link of the specified type already exists for the app, the existing sharing link will be returned.</span></span>

<span data-ttu-id="9a438-108">Ресурсы DriveItem наследуют разрешения совместного доступа от своих предков.</span><span class="sxs-lookup"><span data-stu-id="9a438-108">DriveItem resources inherit sharing permissions from their ancestors.</span></span>

## <a name="permissions"></a><span data-ttu-id="9a438-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9a438-109">Permissions</span></span>

<span data-ttu-id="9a438-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9a438-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a438-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9a438-112">Permission type</span></span>      | <span data-ttu-id="9a438-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9a438-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9a438-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9a438-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9a438-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a438-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="9a438-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9a438-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9a438-117">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a438-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="9a438-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9a438-118">Application</span></span> | <span data-ttu-id="9a438-119">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a438-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9a438-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9a438-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/createLink
POST /groups/{groupId}/drive/items/{itemId}/createLink
POST /me/drive/items/{itemId}/createLink
POST /sites/{siteId}/drive/items/{itemId}/createLink
POST /users/{userId}/drive/items/{itemId}/createLink
```

### <a name="request-body"></a><span data-ttu-id="9a438-121">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9a438-121">Request body</span></span>

<span data-ttu-id="9a438-122">В теле запроса определяются свойства ссылки для совместного доступа, запрашиваемой приложением.</span><span class="sxs-lookup"><span data-stu-id="9a438-122">The body of the request defines properties of the sharing link your application is requesting.</span></span>
<span data-ttu-id="9a438-123">Запрос должен быть объектом JSON с указанными ниже свойствами.</span><span class="sxs-lookup"><span data-stu-id="9a438-123">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="9a438-124">Имя</span><span class="sxs-lookup"><span data-stu-id="9a438-124">Name</span></span>    |  <span data-ttu-id="9a438-125">Тип</span><span class="sxs-lookup"><span data-stu-id="9a438-125">Type</span></span>  |                                 <span data-ttu-id="9a438-126">Описание</span><span class="sxs-lookup"><span data-stu-id="9a438-126">Description</span></span>                                  |
| :-------- | :----- | :--------------------------------------------------------------------------- |
| <span data-ttu-id="9a438-127">**type**</span><span class="sxs-lookup"><span data-stu-id="9a438-127">**type**</span></span>  | <span data-ttu-id="9a438-128">string</span><span class="sxs-lookup"><span data-stu-id="9a438-128">string</span></span> | <span data-ttu-id="9a438-p105">Тип создаваемой ссылки для совместного доступа. Возможные значения: `view`, `edit` или `embed`.</span><span class="sxs-lookup"><span data-stu-id="9a438-p105">The type of sharing link to create. Either `view`, `edit`, or `embed`.</span></span>       |
| <span data-ttu-id="9a438-131">**scope**</span><span class="sxs-lookup"><span data-stu-id="9a438-131">**scope**</span></span> | <span data-ttu-id="9a438-132">string</span><span class="sxs-lookup"><span data-stu-id="9a438-132">string</span></span> | <span data-ttu-id="9a438-133">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="9a438-133">Optional.</span></span> <span data-ttu-id="9a438-134">Область создаваемой ссылки.</span><span class="sxs-lookup"><span data-stu-id="9a438-134">The scope of link to create.</span></span> <span data-ttu-id="9a438-135">Возможные значения: `anonymous` или `organization`.</span><span class="sxs-lookup"><span data-stu-id="9a438-135">Either `anonymous` or `organization`.</span></span> |


### <a name="link-types"></a><span data-ttu-id="9a438-136">Типы ссылок</span><span class="sxs-lookup"><span data-stu-id="9a438-136">Link types</span></span>

<span data-ttu-id="9a438-137">Параметр **type** может принимать указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="9a438-137">The following values are allowed for the **type** parameter.</span></span>

| <span data-ttu-id="9a438-138">Значение типа</span><span class="sxs-lookup"><span data-stu-id="9a438-138">Type value</span></span> | <span data-ttu-id="9a438-139">Описание</span><span class="sxs-lookup"><span data-stu-id="9a438-139">Description</span></span>                                                                                  |
|:-----------|:---------------------------------------------------------------------------------------------|
| `view`     | <span data-ttu-id="9a438-140">Создает ссылку на объект DriveItem, предполагающую доступ только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9a438-140">Creates a read-only link to the DriveItem.</span></span>                                                        |
| `edit`     | <span data-ttu-id="9a438-141">Создает ссылку на объект DriveItem, предполагающую доступ для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="9a438-141">Creates a read-write link to the DriveItem.</span></span>                                                       |
| `embed`    | <span data-ttu-id="9a438-142">Создает встраиваемую ссылку на объект DriveItem.</span><span class="sxs-lookup"><span data-stu-id="9a438-142">Creates an embeddable link to the DriveItem.</span></span> <span data-ttu-id="9a438-143">Этот вариант доступен только для файлов в личных учетных записях OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9a438-143">This option is only available for files in OneDrive personal.</span></span> |

### <a name="scope-types"></a><span data-ttu-id="9a438-144">Типы областей</span><span class="sxs-lookup"><span data-stu-id="9a438-144">Scope types</span></span>

<span data-ttu-id="9a438-145">Параметр **scope** может принимать указанные ниже значения.</span><span class="sxs-lookup"><span data-stu-id="9a438-145">The following values are allowed for the **scope** parameter.</span></span>
<span data-ttu-id="9a438-146">Если параметр **scope** не задан, создается ссылка того типа, который используется в организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9a438-146">If the **scope** parameter is not specified, the default link type for the organization is created.</span></span>

| <span data-ttu-id="9a438-147">Значение типа</span><span class="sxs-lookup"><span data-stu-id="9a438-147">Type value</span></span>     | <span data-ttu-id="9a438-148">Описание</span><span class="sxs-lookup"><span data-stu-id="9a438-148">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------------------------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="9a438-149">Создает ссылку на объект DriveItem, доступный всем, кому она предоставлена.</span><span class="sxs-lookup"><span data-stu-id="9a438-149">Creates a link to the DriveItem accessible to anyone with the link.</span></span> <span data-ttu-id="9a438-150">Администратор может отключить ссылки, не требующие проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="9a438-150">Anonymous links may be disabled by an administrator.</span></span>                 |
| `organization` | <span data-ttu-id="9a438-151">Создает ссылку на объект DriveItem, доступный всем в организации пользователя.</span><span class="sxs-lookup"><span data-stu-id="9a438-151">Creates a link to the DriveItem accessible to anyone within the user's organization.</span></span> <span data-ttu-id="9a438-152">Область организации для ссылок недоступна в личных учетных записях OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9a438-152">Organization link scope is not available for OneDrive personal.</span></span> |

## <a name="response"></a><span data-ttu-id="9a438-153">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a438-153">Response</span></span>

<span data-ttu-id="9a438-154">В случае успешного выполнения этот метод возвращает в тексте ответа один ресурс [Permission](../resources/permission.md), представляющий запрашиваемые разрешения для совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="9a438-154">If successful, this method returns a single [Permission](../resources/permission.md) resource in the response body that represents the requested sharing permissions.</span></span>

<span data-ttu-id="9a438-155">Если для элемента создается новая ссылка совместного доступа, возвращается код ответа `201 Created`, а если возвращается существующая ссылка — код `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="9a438-155">The response will be `201 Created` if a new sharing link is created for the item or `200 OK` if an existing link is returned.</span></span>

## <a name="example"></a><span data-ttu-id="9a438-156">Пример</span><span class="sxs-lookup"><span data-stu-id="9a438-156">Example</span></span>

<span data-ttu-id="9a438-157">В приведенном ниже примере запрашивается создание ссылки для совместного доступа к объекту DriveItem, указанному по {itemId}, в хранилище OneDrive пользователя.</span><span class="sxs-lookup"><span data-stu-id="9a438-157">The following example requests a sharing link to be created for the DriveItem specified by {itemId} in the user's OneDrive.</span></span>
<span data-ttu-id="9a438-158">Ссылка для совместного доступа подразумевает доступ только для чтения, и ее может использовать каждый, кому она предоставлена.</span><span class="sxs-lookup"><span data-stu-id="9a438-158">The sharing link is configured to be read-only and usable by anyone with the link.</span></span>

### <a name="request"></a><span data-ttu-id="9a438-159">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a438-159">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="9a438-160">Отклик</span><span class="sxs-lookup"><span data-stu-id="9a438-160">Response</span></span>

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

## <a name="creating-company-sharable-links"></a><span data-ttu-id="9a438-161">Создание ссылок с возможностью общего доступа в компании</span><span class="sxs-lookup"><span data-stu-id="9a438-161">Creating company sharable links</span></span>

<span data-ttu-id="9a438-162">OneDrive для бизнеса и SharePoint поддерживают ссылки с возможностью общего доступа в компании.</span><span class="sxs-lookup"><span data-stu-id="9a438-162">OneDrive for Business and SharePoint support company sharable links.</span></span>
<span data-ttu-id="9a438-163">Они аналогичны ссылкам, не требующим проверки подлинности, но работают только для элементов соответствующей организации.</span><span class="sxs-lookup"><span data-stu-id="9a438-163">These are similar to anonymous links, except they only work for members of the owning organization.</span></span>
<span data-ttu-id="9a438-164">Чтобы создать такую ссылку, задайте для параметра **scope** значение `organization`.</span><span class="sxs-lookup"><span data-stu-id="9a438-164">To create a company sharable link, use the **scope** parameter with a value of `organization`.</span></span>

### <a name="request"></a><span data-ttu-id="9a438-165">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a438-165">Request</span></span>

<!-- { "blockType": "request", "name": "create-link-scoped", "scopes": "files.readwrite service.sharepoint" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "edit",
  "scope": "organization"
}
```

### <a name="response"></a><span data-ttu-id="9a438-166">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a438-166">Response</span></span>

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

## <a name="creating-embeddable-links"></a><span data-ttu-id="9a438-167">Создание встраиваемых ссылок</span><span class="sxs-lookup"><span data-stu-id="9a438-167">Creating embeddable links</span></span>

<span data-ttu-id="9a438-p113">При использовании типа ссылки `embed` возвращаемое значение webUrl можно внедрять в элемент HTML `<iframe>`. При создании встроенной ссылки свойство `webHtml` содержит HTML-код для объекта `<iframe>`, в котором размещается содержимое.</span><span class="sxs-lookup"><span data-stu-id="9a438-p113">When using the `embed` link type, the webUrl returned can be embedded in an `<iframe>` HTML element. When an embed link is created the `webHtml` property contains the HTML code for an `<iframe>` to host the content.</span></span>

<span data-ttu-id="9a438-170">**Примечание.** Внедрение ссылок поддерживается только в личных учетных записях OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9a438-170">**Note:** Embed links are only supported for OneDrive personal.</span></span>

### <a name="request"></a><span data-ttu-id="9a438-171">Запрос</span><span class="sxs-lookup"><span data-stu-id="9a438-171">Request</span></span>

<!-- { "blockType": "request", "name": "create-embedded-link", "scopes": "files.readwrite service.onedrive" } -->

```http
POST /me/drive/items/{item-id}/createLink
Content-Type: application/json

{
  "type": "embed"
}
```

### <a name="response"></a><span data-ttu-id="9a438-172">Ответ</span><span class="sxs-lookup"><span data-stu-id="9a438-172">Response</span></span>

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

## <a name="remarks"></a><span data-ttu-id="9a438-173">Примечания</span><span class="sxs-lookup"><span data-stu-id="9a438-173">Remarks</span></span>

* <span data-ttu-id="9a438-174">Срок действия ссылок, созданных с помощью этого действия, не истекает при условии, что в организации не включена политика срока действия.</span><span class="sxs-lookup"><span data-stu-id="9a438-174">Links created using this action do not expire unless a default expiration policy is enforced for the organization.</span></span>
* <span data-ttu-id="9a438-175">Ссылки отображаются в разрешениях на совместное использование для элемента и могут быть удалены владельцем элемента.</span><span class="sxs-lookup"><span data-stu-id="9a438-175">Links are visible in the sharing permissions for the item and can be removed by an owner of the item.</span></span>
* <span data-ttu-id="9a438-176">Они всегда указывают на текущую версию элемента, если он не был извлечен (только в SharePoint).</span><span class="sxs-lookup"><span data-stu-id="9a438-176">Links always point to the current version of a item unless the item is checked out (SharePoint only).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "Create a new sharing link for an item.",
  "keywords": "create,sharing,sharing link",
  "section": "documentation",
  "tocPath": "Sharing/Create link"
} -->
