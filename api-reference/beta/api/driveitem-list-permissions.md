---
author: JeremyKelley
description: Список эффективных разрешений общего доступа на driveItem.
ms.date: 09/10/2017
title: Список, у которого есть доступ к файлу
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 346fb5de25021ae9672722a8a128fed224853368
ms.sourcegitcommit: 0ca0a1e2810701c2392e5c685e984fbfb6785579
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2021
ms.locfileid: "53151477"
---
# <a name="list-sharing-permissions-on-a-driveitem"></a><span data-ttu-id="37c39-103">Разрешения общего доступа к списку на driveItem</span><span class="sxs-lookup"><span data-stu-id="37c39-103">List sharing permissions on a driveItem</span></span>

<span data-ttu-id="37c39-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37c39-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37c39-105">Список эффективных разрешений общего доступа на [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="37c39-105">List the effective sharing permissions on a [driveItem](../resources/driveitem.md).</span></span>

## <a name="access-to-sharing-permissions"></a><span data-ttu-id="37c39-106">Доступ к разрешениями совместного доступа</span><span class="sxs-lookup"><span data-stu-id="37c39-106">Access to sharing permissions</span></span>

<span data-ttu-id="37c39-107">Коллекция разрешений включает потенциально конфиденциальные данные и может быть доступна не для каждого отправителя вызовов.</span><span class="sxs-lookup"><span data-stu-id="37c39-107">The permissions collection includes potentially sensitive information and may not be available for every caller.</span></span>

* <span data-ttu-id="37c39-108">Для владельца элемента возвращаются все разрешения совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="37c39-108">For the owner of the item, all sharing permissions will be returned.</span></span> <span data-ttu-id="37c39-109">Это относится и к совладельцам.</span><span class="sxs-lookup"><span data-stu-id="37c39-109">This includes co-owners.</span></span>
* <span data-ttu-id="37c39-110">Если вызов отправляет не владелец, возвращаются только те разрешения, которые относятся к отправителю вызова.</span><span class="sxs-lookup"><span data-stu-id="37c39-110">For a non-owner caller, only the sharing permissions that apply to the caller are returned.</span></span>
* <span data-ttu-id="37c39-111">Свойства разрешений совместного доступа, содержащие секреты (например, `shareId` и `webUrl`), возвращаются только для тех пользователей, которые могут создать такое разрешение.</span><span class="sxs-lookup"><span data-stu-id="37c39-111">Sharing permission properties that contain secrets (e.g. `shareId` and `webUrl`) are only returned for callers that are able to create the sharing permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="37c39-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="37c39-112">Permissions</span></span>

<span data-ttu-id="37c39-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="37c39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37c39-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="37c39-115">Permission type</span></span>      | <span data-ttu-id="37c39-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="37c39-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="37c39-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="37c39-117">Delegated (work or school account)</span></span> | <span data-ttu-id="37c39-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37c39-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="37c39-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="37c39-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="37c39-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37c39-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="37c39-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="37c39-121">Application</span></span> | <span data-ttu-id="37c39-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37c39-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="37c39-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="37c39-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /sites/{siteId}/drive/items/{itemId}/permissions
GET /users/{userId}/drive/items/{itemId}/permissions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37c39-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="37c39-124">Optional query parameters</span></span>

<span data-ttu-id="37c39-125">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="37c39-125">This method supports the `$select` [OData Query Parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="37c39-126">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="37c39-126">Optional request headers</span></span>

| <span data-ttu-id="37c39-127">Имя</span><span class="sxs-lookup"><span data-stu-id="37c39-127">Name</span></span>          | <span data-ttu-id="37c39-128">Тип</span><span class="sxs-lookup"><span data-stu-id="37c39-128">Type</span></span>   | <span data-ttu-id="37c39-129">Описание</span><span class="sxs-lookup"><span data-stu-id="37c39-129">Description</span></span>                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="37c39-130">if-none-match</span><span class="sxs-lookup"><span data-stu-id="37c39-130">if-none-match</span></span> | <span data-ttu-id="37c39-131">string</span><span class="sxs-lookup"><span data-stu-id="37c39-131">string</span></span> | <span data-ttu-id="37c39-132">Если указан заголовок запроса, а предоставленный тег etag совпадает с текущим тегом etag элемента, то возвращается ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="37c39-132">If this request header is included and the etag provided matches the current etag on the item, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="37c39-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="37c39-133">Response</span></span>

<span data-ttu-id="37c39-134">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию ресурсов [Permission](../resources/permission.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="37c39-134">If successful, this method returns a `200 OK` response code and collection of [Permission](../resources/permission.md) resources in the response body.</span></span>

<span data-ttu-id="37c39-135">Действующие разрешения совместного доступа для элемента DriveItem можно получить из двух источников:</span><span class="sxs-lookup"><span data-stu-id="37c39-135">Effective sharing permissions of a DriveItem can come from two sources:</span></span>

* <span data-ttu-id="37c39-136">разрешения совместного доступа, примененные непосредственно к самому элементу DriveItem;</span><span class="sxs-lookup"><span data-stu-id="37c39-136">Sharing permissions applied directly on the DriveItem itself</span></span>
* <span data-ttu-id="37c39-137">разрешения совместного доступа, унаследованные от предков элемента DriveItem.</span><span class="sxs-lookup"><span data-stu-id="37c39-137">Sharing permissions inherited from the DriveItem's ancestors</span></span>

<span data-ttu-id="37c39-p103">Абоненты могут распознать унаследованное разрешение, проверив свойство **inheritedFrom**. Это свойство — ресурс [**itemReference**](../resources/itemreference.md), отсылающий к предшествующему элементу, от которого унаследовано разрешение.</span><span class="sxs-lookup"><span data-stu-id="37c39-p103">Callers can differentiate if the permission is inherited or not by checking the **inheritedFrom** property. This property is an [**itemReference**](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

## <a name="example"></a><span data-ttu-id="37c39-140">Пример</span><span class="sxs-lookup"><span data-stu-id="37c39-140">Example</span></span>

<span data-ttu-id="37c39-141">В этом примере показано, как получить набор разрешений для элемента в объекте drive пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="37c39-141">This example retrieves the collection of permissions on an item in the signed in user's drive.</span></span>


# <a name="http"></a>[<span data-ttu-id="37c39-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="37c39-142">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-item-permissions", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/permissions
```
# <a name="c"></a>[<span data-ttu-id="37c39-143">C#</span><span class="sxs-lookup"><span data-stu-id="37c39-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-permissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37c39-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37c39-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-permissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37c39-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37c39-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-permissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37c39-146">Java</span><span class="sxs-lookup"><span data-stu-id="37c39-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-permissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="37c39-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="37c39-147">Response</span></span>

<span data-ttu-id="37c39-148">Этот пример ответа включает три разрешения. Первое разрешение представляет собой ссылку совместного доступа с разрешениями на изменение, второе — явное разрешение для пользователя с именем John, которое унаследовано от родительской папки, а третье разрешение — это ссылка совместного доступа с правами на чтение и запись, созданная приложением.</span><span class="sxs-lookup"><span data-stu-id="37c39-148">This example response includes three permissions, the first is a sharing link with edit permissions, the second is an explicit permission for a user named John, which was inherited from a parent folder, and the third is a read-write sharing link created by an application.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="37c39-149">Примечания</span><span class="sxs-lookup"><span data-stu-id="37c39-149">Remarks</span></span>

<span data-ttu-id="37c39-p104">Связи между **разрешениями** ресурса DriveItem невозможно развернуть как часть запроса на [получение DriveItem](driveitem-get.md) или коллекции DriveItems. Необходимо открыть доступ непосредственно к свойству разрешений.</span><span class="sxs-lookup"><span data-stu-id="37c39-p104">The **permissions** relationship of DriveItem cannot be expanded as part of a call to [get DriveItem](driveitem-get.md) or a collection of DriveItems. You must access the permissions property directly.</span></span>

## <a name="error-responses"></a><span data-ttu-id="37c39-152">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="37c39-152">Error responses</span></span>

<span data-ttu-id="37c39-153">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Отклики ошибок][error-response].</span><span class="sxs-lookup"><span data-stu-id="37c39-153">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

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
