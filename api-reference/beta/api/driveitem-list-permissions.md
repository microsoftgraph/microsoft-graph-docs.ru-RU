---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Создание списка пользователей, имеющих доступ к файлу
ms.openlocfilehash: e221249397b07875e591cc7979bcc61d68f05e8c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076673"
---
# <a name="list-sharing-permissions-on-a-driveitem"></a><span data-ttu-id="32d03-102">Создание списка разрешений совместного доступа в элементе DriveItem</span><span class="sxs-lookup"><span data-stu-id="32d03-102">List sharing permissions on a DriveItem</span></span>

> <span data-ttu-id="32d03-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="32d03-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="32d03-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="32d03-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="32d03-105">Создание списка действующих разрешений на общий доступ в элементе [DriveItem](../resources/driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="32d03-105">List the effective sharing permissions of on a [DriveItem](../resources/driveitem.md).</span></span>

## <a name="access-to-sharing-permissions"></a><span data-ttu-id="32d03-106">Доступ к разрешениями на общий доступ</span><span class="sxs-lookup"><span data-stu-id="32d03-106">Access to sharing permissions</span></span>

<span data-ttu-id="32d03-107">Коллекция разрешений включает потенциально конфиденциальные сведения и может быть доступна не для всех вызывающих объектов.</span><span class="sxs-lookup"><span data-stu-id="32d03-107">The permissions collection includes potentially sensitive information and may not be available for every caller.</span></span>

* <span data-ttu-id="32d03-108">Для владельца элемента возвращаются все разрешения на общий доступ.</span><span class="sxs-lookup"><span data-stu-id="32d03-108">For the owner of the item, all sharing permissions will be returned.</span></span> <span data-ttu-id="32d03-109">К владельцам элемента также относятся его совладельцы.</span><span class="sxs-lookup"><span data-stu-id="32d03-109">This includes co-owners.</span></span>
* <span data-ttu-id="32d03-110">Вызывающему объекту, который не является владельцем, возвращаются только применяемые к нему разрешения.</span><span class="sxs-lookup"><span data-stu-id="32d03-110">For a non-owner caller, only the sharing permissions that apply to the caller are returned.</span></span>
* <span data-ttu-id="32d03-111">Свойства разрешений на общий доступ, содержащие секреты (например, `shareId` и `webUrl`), возвращаются только для вызывающих объектов, которые могут создать разрешение на общий доступ.</span><span class="sxs-lookup"><span data-stu-id="32d03-111">Sharing permission properties that contain secrets (e.g. `shareId` and `webUrl`) are only returned for callers that are able to create the sharing permission.</span></span>

## <a name="permissions"></a><span data-ttu-id="32d03-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="32d03-112">Permissions</span></span>

<span data-ttu-id="32d03-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="32d03-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="32d03-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="32d03-115">Permission type</span></span>      | <span data-ttu-id="32d03-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="32d03-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="32d03-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="32d03-117">Delegated (work or school account)</span></span> | <span data-ttu-id="32d03-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32d03-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="32d03-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="32d03-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="32d03-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32d03-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="32d03-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="32d03-121">Application</span></span> | <span data-ttu-id="32d03-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32d03-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="32d03-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="32d03-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions
GET /groups/{group-id}/drive/items/{item-id}/permissions
GET /me/drive/items/{item-id}/permissions
GET /me/drive/root:/{path}:/permissions
GET /sites/{siteId}/drive/items/{itemId}/permissions
GET /users/{userId}/drive/items/{itemId}/permissions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="32d03-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="32d03-124">Optional query parameters</span></span>

<span data-ttu-id="32d03-125">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$select` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="32d03-125">This method supports the `$select` [OData Query Parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="32d03-126">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="32d03-126">Optional request headers</span></span>

| <span data-ttu-id="32d03-127">Имя</span><span class="sxs-lookup"><span data-stu-id="32d03-127">Name</span></span>          | <span data-ttu-id="32d03-128">Тип</span><span class="sxs-lookup"><span data-stu-id="32d03-128">Type</span></span>   | <span data-ttu-id="32d03-129">Описание</span><span class="sxs-lookup"><span data-stu-id="32d03-129">Description</span></span>                                                                                                                                     |
|:--------------|:-------|:------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="32d03-130">if-none-match</span><span class="sxs-lookup"><span data-stu-id="32d03-130">if-none-match</span></span> | <span data-ttu-id="32d03-131">string</span><span class="sxs-lookup"><span data-stu-id="32d03-131">string</span></span> | <span data-ttu-id="32d03-132">Если указан этот заголовок запроса, а предоставленный тег etag совпадает с текущим тегом etag элемента, будет возвращен отклик `HTTP 304 Not Modified`.</span><span class="sxs-lookup"><span data-stu-id="32d03-132">If this request header is included and the etag provided matches the current etag on the item, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="32d03-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="32d03-133">Response</span></span>

<span data-ttu-id="32d03-134">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию ресурсов [Permission](../resources/permission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="32d03-134">If successful, this method returns a `200 OK` response code and collection of [Permission](../resources/permission.md) resources in the response body.</span></span>

<span data-ttu-id="32d03-135">Действующие разрешения на общий доступ для элемента DriveItem могут быть получены двумя путями:</span><span class="sxs-lookup"><span data-stu-id="32d03-135">Effective sharing permissions of a DriveItem can come from two sources:</span></span>

* <span data-ttu-id="32d03-136">разрешения на общий доступ, примененные непосредственно к самому элементу DriveItem;</span><span class="sxs-lookup"><span data-stu-id="32d03-136">Sharing permissions applied directly on the DriveItem itself</span></span>
* <span data-ttu-id="32d03-137">разрешения на общий доступ, унаследованные от предков элемента DriveItem.</span><span class="sxs-lookup"><span data-stu-id="32d03-137">Sharing permissions inherited from the DriveItem's ancestors</span></span>

<span data-ttu-id="32d03-p104">Абоненты могут распознать унаследованное разрешение, проверив свойство **inheritedFrom**. Это свойство — ресурс [**itemReference**](../resources/itemreference.md), отсылающий к предшествующему элементу, от которого унаследовано разрешение.</span><span class="sxs-lookup"><span data-stu-id="32d03-p104">Callers can differentiate if the permission is inherited or not by checking the **inheritedFrom** property. This property is an [**itemReference**](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="32d03-140">Уровни разрешений SharePoint, заданные для элемента, возвращаются с префиксом SP.</span><span class="sxs-lookup"><span data-stu-id="32d03-140">SharePoint permission levels set on an item are returned with an 'SP' prefix.</span></span> <span data-ttu-id="32d03-141">Примеры: SP.View Only, SP.Limited Access, SP.View Web Analytics Data.</span><span class="sxs-lookup"><span data-stu-id="32d03-141">For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data.</span></span> <span data-ttu-id="32d03-142">См. [полный список ролей SharePoint](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span><span class="sxs-lookup"><span data-stu-id="32d03-142">See [Full list of SharePoint roles](https://technet.microsoft.com/en-us/library/cc721640.aspx#section1).</span></span>

## <a name="example"></a><span data-ttu-id="32d03-143">Пример</span><span class="sxs-lookup"><span data-stu-id="32d03-143">Example</span></span>

<span data-ttu-id="32d03-144">В этом примере показано, как получить набор разрешений для элемента в объекте drive пользователя, выполнившего вход в систему.</span><span class="sxs-lookup"><span data-stu-id="32d03-144">This example retrieves the collection of permissions on an item in the signed in user's drive.</span></span>

<!-- { "blockType": "request", "name": "get-item-permissions", "scopes": "files.read" } -->

```http
GET /me/drive/items/{item-id}/permissions
```

### <a name="response"></a><span data-ttu-id="32d03-145">Ответ</span><span class="sxs-lookup"><span data-stu-id="32d03-145">Response</span></span>

<span data-ttu-id="32d03-146">Этот пример отклика включает три разрешения. Первое разрешение представляет собой ссылку для общего доступа с разрешениями на изменение, второе — явное разрешение для пользователя с именем John, которое унаследовано от родительской папки, а третье разрешение — это ссылка для общего доступа с правами на чтение и запись, созданная приложением.</span><span class="sxs-lookup"><span data-stu-id="32d03-146">This example response includes three permissions, the first is a sharing link with edit permissions, the second is an explicit permission for a user named John, which was inherited from a parent folder, and the third is a read-write sharing link created by an application.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="32d03-147">Примечания</span><span class="sxs-lookup"><span data-stu-id="32d03-147">Remarks</span></span>

<span data-ttu-id="32d03-p106">Связи между **разрешениями** ресурса DriveItem невозможно развернуть как часть запроса на [получение DriveItem](driveitem-get.md) или коллекции DriveItems. Необходимо открыть доступ непосредственно к свойству разрешений.</span><span class="sxs-lookup"><span data-stu-id="32d03-p106">The **permissions** relationship of DriveItem cannot be expanded as part of a call to [get DriveItem](driveitem-get.md) or a collection of DriveItems. You must access the permissions property directly.</span></span>

## <a name="error-responses"></a><span data-ttu-id="32d03-150">Ответы с ошибками</span><span class="sxs-lookup"><span data-stu-id="32d03-150">Error responses</span></span>

<span data-ttu-id="32d03-151">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="32d03-151">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "List an item's permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions"
} -->
