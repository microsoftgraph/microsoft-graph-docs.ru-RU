---
author: JeremyKelley
description: Перечислите эффективные разрешения общего доступа в driveItem.
ms.date: 09/10/2017
title: Список пользователей, имеющих доступ к файлу
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 98d8f28c6f0cf516ca908b0de138417010bf8d53
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868600"
---
# <a name="list-sharing-permissions-on-a-driveitem"></a><span data-ttu-id="cd460-103">Список разрешений на совместное использование в driveItem</span><span class="sxs-lookup"><span data-stu-id="cd460-103">List sharing permissions on a driveItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd460-104">Перечислите эффективные разрешения общего доступа в [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="cd460-104">List the effective sharing permissions of on a [driveItem](../resources/driveitem.md).</span></span>

## <a name="access-to-sharing-permissions"></a><span data-ttu-id="cd460-105">Доступ к разрешениями совместного доступа</span><span class="sxs-lookup"><span data-stu-id="cd460-105">Access to sharing permissions</span></span>

<span data-ttu-id="cd460-106">Коллекция разрешений включает потенциально конфиденциальные данные и может быть доступна не для каждого отправителя вызовов.</span><span class="sxs-lookup"><span data-stu-id="cd460-106">The permissions collection includes potentially sensitive information and may not be available for every caller.</span></span>

* <span data-ttu-id="cd460-107">Для владельца элемента возвращаются все разрешения совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="cd460-107">For the owner of the item, all sharing permissions will be returned.</span></span> <span data-ttu-id="cd460-108">Это относится и к совладельцам.</span><span class="sxs-lookup"><span data-stu-id="cd460-108">This includes co-owners.</span></span>
* <span data-ttu-id="cd460-109">Если вызов отправляет не владелец, возвращаются только те разрешения, которые относятся к отправителю вызова.</span><span class="sxs-lookup"><span data-stu-id="cd460-109">For a non-owner caller, only the sharing permissions that apply to the caller are returned.</span></span>
* <span data-ttu-id="cd460-110">Свойства разрешений совместного доступа, содержащие секреты (например, `shareId` и `webUrl`), возвращаются только для тех пользователей, которые могут создать такое разрешение.</span><span class="sxs-lookup"><span data-stu-id="cd460-110">Sharing permission properties that contain secrets (e.g. `shareId` and `webUrl`) are only returned for callers that are able to create the sharing permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd460-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd460-111">Permissions</span></span>

<span data-ttu-id="cd460-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd460-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd460-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd460-114">Permission type</span></span>      | <span data-ttu-id="cd460-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd460-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd460-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd460-116">Delegated (work or school account)</span></span> | <span data-ttu-id="cd460-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd460-117">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="cd460-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd460-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd460-119">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd460-119">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="cd460-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd460-120">Application</span></span> | <span data-ttu-id="cd460-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd460-121">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd460-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd460-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /sites/{siteId}/drive/items/{itemId}/permissions
GET /users/{userId}/drive/items/{itemId}/permissions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cd460-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cd460-123">Optional query parameters</span></span>

<span data-ttu-id="cd460-124">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="cd460-124">This method supports the `$select` [OData Query Parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="cd460-125">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd460-125">Optional request headers</span></span>

| <span data-ttu-id="cd460-126">Имя</span><span class="sxs-lookup"><span data-stu-id="cd460-126">Name</span></span>          | <span data-ttu-id="cd460-127">Тип</span><span class="sxs-lookup"><span data-stu-id="cd460-127">Type</span></span>   | <span data-ttu-id="cd460-128">Описание</span><span class="sxs-lookup"><span data-stu-id="cd460-128">Description</span></span>                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="cd460-129">if-none-match</span><span class="sxs-lookup"><span data-stu-id="cd460-129">if-none-match</span></span> | <span data-ttu-id="cd460-130">string</span><span class="sxs-lookup"><span data-stu-id="cd460-130">string</span></span> | <span data-ttu-id="cd460-131">Если указан заголовок запроса, а предоставленный тег etag совпадает с текущим тегом etag элемента, то возвращается ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="cd460-131">If this request header is included and the etag provided matches the current etag on the item, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="cd460-132">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd460-132">Response</span></span>

<span data-ttu-id="cd460-133">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию ресурсов [Permission](../resources/permission.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cd460-133">If successful, this method returns a `200 OK` response code and collection of [Permission](../resources/permission.md) resources in the response body.</span></span>

<span data-ttu-id="cd460-134">Действующие разрешения совместного доступа для элемента DriveItem можно получить из двух источников:</span><span class="sxs-lookup"><span data-stu-id="cd460-134">Effective sharing permissions of a DriveItem can come from two sources:</span></span>

* <span data-ttu-id="cd460-135">разрешения совместного доступа, примененные непосредственно к самому элементу DriveItem;</span><span class="sxs-lookup"><span data-stu-id="cd460-135">Sharing permissions applied directly on the DriveItem itself</span></span>
* <span data-ttu-id="cd460-136">разрешения совместного доступа, унаследованные от предков элемента DriveItem.</span><span class="sxs-lookup"><span data-stu-id="cd460-136">Sharing permissions inherited from the DriveItem's ancestors</span></span>

<span data-ttu-id="cd460-p103">Абоненты могут распознать унаследованное разрешение, проверив свойство **inheritedFrom**. Это свойство — ресурс [**itemReference**](../resources/itemreference.md), отсылающий к предшествующему элементу, от которого унаследовано разрешение.</span><span class="sxs-lookup"><span data-stu-id="cd460-p103">Callers can differentiate if the permission is inherited or not by checking the **inheritedFrom** property. This property is an [**itemReference**](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="cd460-p104">Уровни разрешений SharePoint, заданные для элемента, возвращаются с префиксом SP. Примеры: SP.View Only, SP.Limited Access, SP.View Web Analytics Data. См. [полный список ролей SharePoint](https://technet.microsoft.com/library/cc721640.aspx#section1).</span><span class="sxs-lookup"><span data-stu-id="cd460-p104">SharePoint permission levels set on an item are returned with an 'SP' prefix. For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data. See [Full list of SharePoint roles](https://technet.microsoft.com/library/cc721640.aspx#section1).</span></span>

## <a name="example"></a><span data-ttu-id="cd460-142">Пример</span><span class="sxs-lookup"><span data-stu-id="cd460-142">Example</span></span>

<span data-ttu-id="cd460-143">В этом примере показано, как получить набор разрешений для элемента в объекте drive пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="cd460-143">This example retrieves the collection of permissions on an item in the signed in user's drive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="cd460-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd460-144">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-item-permissions", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/permissions
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="cd460-145">C#</span><span class="sxs-lookup"><span data-stu-id="cd460-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-permissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cd460-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd460-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-permissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cd460-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd460-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-permissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cd460-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="cd460-148">Response</span></span>

<span data-ttu-id="cd460-149">Этот пример ответа включает три разрешения. Первое разрешение представляет собой ссылку совместного доступа с разрешениями на изменение, второе — явное разрешение для пользователя с именем John, которое унаследовано от родительской папки, а третье разрешение — это ссылка совместного доступа с правами на чтение и запись, созданная приложением.</span><span class="sxs-lookup"><span data-stu-id="cd460-149">This example response includes three permissions, the first is a sharing link with edit permissions, the second is an explicit permission for a user named John, which was inherited from a parent folder, and the third is a read-write sharing link created by an application.</span></span>

<!-- {"blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit"
      }
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedTo": {
        "user": {
          "id": "5D33DD65C6932946",
          "displayName": "John Doe"
        }
      },
      "inheritedFrom": {
        "driveId": "1234567890ABD",
        "id": "1234567890ABC!123",
        "path": "/drive/root:/Documents" }
    },
    {
      "id": "3",
      "roles": ["write"],
      "link": {
        "webUrl": "https://onedrive.live.com/redir?resid=5D33DD65C6932946!70859&authkey=!AL7N1QAfSWcjNU8&ithint=folder%2cgif",
        "type": "edit",
        "application": {
          "id": "12345",
          "displayName": "Contoso Time Manager"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="cd460-150">Примечания</span><span class="sxs-lookup"><span data-stu-id="cd460-150">Remarks</span></span>

<span data-ttu-id="cd460-p105">Связи между **разрешениями** ресурса DriveItem невозможно развернуть как часть запроса на [получение DriveItem](driveitem-get.md) или коллекции DriveItems. Необходимо открыть доступ непосредственно к свойству разрешений.</span><span class="sxs-lookup"><span data-stu-id="cd460-p105">The **permissions** relationship of DriveItem cannot be expanded as part of a call to [get DriveItem](driveitem-get.md) or a collection of DriveItems. You must access the permissions property directly.</span></span>

## <a name="error-responses"></a><span data-ttu-id="cd460-153">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="cd460-153">Error responses</span></span>

<span data-ttu-id="cd460-154">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="cd460-154">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "List an item's permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions",
  "suppressions": [
  ]
}
-->
