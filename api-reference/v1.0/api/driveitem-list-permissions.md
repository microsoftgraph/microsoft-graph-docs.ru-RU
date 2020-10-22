---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Список пользователей, имеющих доступ к файлу
localization_priority: Normal
ms.prod: sharepoint
description: Перечислите эффективные разрешения общего доступа в driveItem.
doc_type: apiPageType
ms.openlocfilehash: 1aa566d42a65d3e3c168759d3b76ce175895af3f
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634503"
---
# <a name="list-sharing-permissions-on-a-driveitem"></a><span data-ttu-id="4da18-103">Список разрешений на совместное использование в driveItem</span><span class="sxs-lookup"><span data-stu-id="4da18-103">List sharing permissions on a driveItem</span></span>

<span data-ttu-id="4da18-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4da18-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4da18-105">Перечислите эффективные разрешения на общий доступ к [driveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="4da18-105">List the effective sharing permissions on a [driveItem](../resources/driveitem.md).</span></span>

## <a name="access-to-sharing-permissions"></a><span data-ttu-id="4da18-106">Доступ к разрешениями совместного доступа</span><span class="sxs-lookup"><span data-stu-id="4da18-106">Access to sharing permissions</span></span>

<span data-ttu-id="4da18-107">Коллекция разрешений включает потенциально конфиденциальные данные и может быть доступна не для каждого отправителя вызовов.</span><span class="sxs-lookup"><span data-stu-id="4da18-107">The permissions collection includes potentially sensitive information and may not be available for every caller.</span></span>

* <span data-ttu-id="4da18-108">Для владельца элемента возвращаются все разрешения совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="4da18-108">For the owner of the item, all sharing permissions will be returned.</span></span> <span data-ttu-id="4da18-109">Это относится и к совладельцам.</span><span class="sxs-lookup"><span data-stu-id="4da18-109">This includes co-owners.</span></span>
* <span data-ttu-id="4da18-110">Если вызов отправляет не владелец, возвращаются только те разрешения, которые относятся к отправителю вызова.</span><span class="sxs-lookup"><span data-stu-id="4da18-110">For a non-owner caller, only the sharing permissions that apply to the caller are returned.</span></span>
* <span data-ttu-id="4da18-111">Свойства разрешений совместного доступа, содержащие секреты (например, `shareId` и `webUrl`), возвращаются только для тех пользователей, которые могут создать такое разрешение.</span><span class="sxs-lookup"><span data-stu-id="4da18-111">Sharing permission properties that contain secrets (e.g. `shareId` and `webUrl`) are only returned for callers that are able to create the sharing permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="4da18-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4da18-112">Permissions</span></span>

<span data-ttu-id="4da18-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4da18-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4da18-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4da18-115">Permission type</span></span>      | <span data-ttu-id="4da18-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4da18-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4da18-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4da18-117">Delegated (work or school account)</span></span> | <span data-ttu-id="4da18-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4da18-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4da18-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4da18-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4da18-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4da18-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4da18-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4da18-121">Application</span></span> | <span data-ttu-id="4da18-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4da18-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4da18-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4da18-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /sites/{siteId}/drive/items/{itemId}/permissions
GET /users/{userId}/drive/items/{itemId}/permissions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4da18-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="4da18-124">Optional query parameters</span></span>

<span data-ttu-id="4da18-125">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="4da18-125">This method supports the `$select` [OData Query Parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="4da18-126">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4da18-126">Optional request headers</span></span>

| <span data-ttu-id="4da18-127">Имя</span><span class="sxs-lookup"><span data-stu-id="4da18-127">Name</span></span>          | <span data-ttu-id="4da18-128">Тип</span><span class="sxs-lookup"><span data-stu-id="4da18-128">Type</span></span>   | <span data-ttu-id="4da18-129">Описание</span><span class="sxs-lookup"><span data-stu-id="4da18-129">Description</span></span>                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="4da18-130">if-none-match</span><span class="sxs-lookup"><span data-stu-id="4da18-130">if-none-match</span></span> | <span data-ttu-id="4da18-131">string</span><span class="sxs-lookup"><span data-stu-id="4da18-131">string</span></span> | <span data-ttu-id="4da18-132">Если указан заголовок запроса, а предоставленный тег etag совпадает с текущим тегом etag элемента, то возвращается ответ `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="4da18-132">If this request header is included and the etag provided matches the current etag on the item, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="4da18-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="4da18-133">Response</span></span>

<span data-ttu-id="4da18-134">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и коллекцию ресурсов [Permission](../resources/permission.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4da18-134">If successful, this method returns a `200 OK` response code and collection of [Permission](../resources/permission.md) resources in the response body.</span></span>

<span data-ttu-id="4da18-135">Действующие разрешения совместного доступа для элемента DriveItem можно получить из двух источников:</span><span class="sxs-lookup"><span data-stu-id="4da18-135">Effective sharing permissions of a DriveItem can come from two sources:</span></span>

* <span data-ttu-id="4da18-136">разрешения совместного доступа, примененные непосредственно к самому элементу DriveItem;</span><span class="sxs-lookup"><span data-stu-id="4da18-136">Sharing permissions applied directly on the DriveItem itself</span></span>
* <span data-ttu-id="4da18-137">разрешения совместного доступа, унаследованные от предков элемента DriveItem.</span><span class="sxs-lookup"><span data-stu-id="4da18-137">Sharing permissions inherited from the DriveItem's ancestors</span></span>

<span data-ttu-id="4da18-p103">Абоненты могут распознать унаследованное разрешение, проверив свойство **inheritedFrom**. Это свойство — ресурс [**itemReference**](../resources/itemreference.md), отсылающий к предшествующему элементу, от которого унаследовано разрешение.</span><span class="sxs-lookup"><span data-stu-id="4da18-p103">Callers can differentiate if the permission is inherited or not by checking the **inheritedFrom** property. This property is an [**itemReference**](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="4da18-p104">Уровни разрешений SharePoint, заданные для элемента, возвращаются с префиксом SP. Примеры: SP.View Only, SP.Limited Access, SP.View Web Analytics Data. См. [полный список ролей SharePoint](/SharePoint/sites/user-permissions-and-permission-levels#section1).</span><span class="sxs-lookup"><span data-stu-id="4da18-p104">SharePoint permission levels set on an item are returned with an 'SP' prefix. For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data. See [Full list of SharePoint roles](/SharePoint/sites/user-permissions-and-permission-levels#section1).</span></span>

## <a name="example"></a><span data-ttu-id="4da18-143">Пример</span><span class="sxs-lookup"><span data-stu-id="4da18-143">Example</span></span>

<span data-ttu-id="4da18-144">В этом примере показано, как получить набор разрешений для элемента в объекте drive пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="4da18-144">This example retrieves the collection of permissions on an item in the signed in user's drive.</span></span>

# <a name="http"></a>[<span data-ttu-id="4da18-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="4da18-145">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-item-permissions", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/permissions
```
# <a name="c"></a>[<span data-ttu-id="4da18-146">C#</span><span class="sxs-lookup"><span data-stu-id="4da18-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-permissions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4da18-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4da18-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-permissions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4da18-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4da18-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-permissions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4da18-149">Java</span><span class="sxs-lookup"><span data-stu-id="4da18-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-permissions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4da18-150">Отклик</span><span class="sxs-lookup"><span data-stu-id="4da18-150">Response</span></span>

<span data-ttu-id="4da18-151">Этот пример ответа включает три разрешения. Первое разрешение представляет собой ссылку совместного доступа с разрешениями на изменение, второе — явное разрешение для пользователя с именем John, которое унаследовано от родительской папки, а третье разрешение — это ссылка совместного доступа с правами на чтение и запись, созданная приложением.</span><span class="sxs-lookup"><span data-stu-id="4da18-151">This example response includes three permissions, the first is a sharing link with edit permissions, the second is an explicit permission for a user named John, which was inherited from a parent folder, and the third is a read-write sharing link created by an application.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="4da18-152">Примечания</span><span class="sxs-lookup"><span data-stu-id="4da18-152">Remarks</span></span>

<span data-ttu-id="4da18-p105">Связи между **разрешениями** ресурса DriveItem невозможно развернуть как часть запроса на [получение DriveItem](driveitem-get.md) или коллекции DriveItems. Необходимо открыть доступ непосредственно к свойству разрешений.</span><span class="sxs-lookup"><span data-stu-id="4da18-p105">The **permissions** relationship of DriveItem cannot be expanded as part of a call to [get DriveItem](driveitem-get.md) or a collection of DriveItems. You must access the permissions property directly.</span></span>

## <a name="error-responses"></a><span data-ttu-id="4da18-155">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="4da18-155">Error responses</span></span>

<span data-ttu-id="4da18-156">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="4da18-156">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "List an item's permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions",
  "suppressions": [
  ]
} -->
