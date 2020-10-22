---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Получение разрешений
localization_priority: Normal
description: В этой статье рассказывается, как возвратить действующее разрешение на общий доступ для конкретного ресурса разрешения.
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: f2f3072ff2244112d70b1a6ef3e3423191808230
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634573"
---
# <a name="get-sharing-permission-for-a-file-or-folder"></a><span data-ttu-id="6b52c-103">Получение разрешения на общий доступ для файла или папки</span><span class="sxs-lookup"><span data-stu-id="6b52c-103">Get sharing permission for a file or folder</span></span>

<span data-ttu-id="6b52c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b52c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b52c-105">В этой статье рассказывается, как возвратить действующее разрешение на общий доступ для конкретного ресурса разрешения.</span><span class="sxs-lookup"><span data-stu-id="6b52c-105">Return the effective sharing permission for a particular permission resource.</span></span>

<span data-ttu-id="6b52c-106">Действующие разрешения для элемента могут быть заданы непосредственно для элемента или унаследованы от его предков.</span><span class="sxs-lookup"><span data-stu-id="6b52c-106">Effective permissions of an item can come from two sources: permissions set directly on the item itself or permissions that are inherited from the item's ancestors.</span></span>

<span data-ttu-id="6b52c-p101">Вызывающая сторона может распознать унаследованное разрешение, проверив свойство `inheritedFrom`. Это свойство представляет собой ресурс [itemReference](../resources/itemreference.md), ссылающийся на элемент, от которого унаследовано разрешение.</span><span class="sxs-lookup"><span data-stu-id="6b52c-p101">Callers can differentiate if the permission is inherited or not by checking the `inheritedFrom` property. This property is an [ItemReference](../resources/itemreference.md) resource referencing the ancestor that the permission is inherited from.</span></span>

<span data-ttu-id="6b52c-p102">Уровни разрешений SharePoint, заданные для элемента, возвращаются с префиксом SP. Примеры: SP.View Only, SP.Limited Access, SP.View Web Analytics Data. См. [полный список ролей SharePoint](/SharePoint/sites/user-permissions-and-permission-levels#section1).</span><span class="sxs-lookup"><span data-stu-id="6b52c-p102">SharePoint permission levels set on an item are returned with an 'SP' prefix. For example, SP.View Only, SP.Limited Access, SP.View Web Analytics Data. See [Full list of SharePoint roles](/SharePoint/sites/user-permissions-and-permission-levels#section1).</span></span>

## <a name="permissions"></a><span data-ttu-id="6b52c-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b52c-112">Permissions</span></span>

<span data-ttu-id="6b52c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b52c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b52c-115">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b52c-115">Permission type</span></span>      | <span data-ttu-id="6b52c-116">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b52c-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b52c-117">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b52c-117">Delegated (work or school account)</span></span> | <span data-ttu-id="6b52c-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b52c-118">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6b52c-119">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b52c-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b52c-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b52c-120">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="6b52c-121">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b52c-121">Application</span></span> | <span data-ttu-id="6b52c-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b52c-122">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b52c-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b52c-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}/permissions/{perm-id}
GET /groups/{group-id}/drive/items/{item-id}/permissions/{perm-id}
GET /me/drive/items/{item-id}/permissions/{perm-id}
GET /sites/{site-id}/drive/items/{item-id}/permissions/{perm-id}
GET /users/{user-id}/drive/items/{item-id}/permissions/{perm-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6b52c-124">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="6b52c-124">Optional query parameters</span></span>

<span data-ttu-id="6b52c-125">Этот метод поддерживает [параметр запроса $select](/graph/query-parameters) для формирования отклика.</span><span class="sxs-lookup"><span data-stu-id="6b52c-125">This method support the [$select query parameter](/graph/query-parameters) to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="6b52c-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b52c-126">Response</span></span>

<span data-ttu-id="6b52c-127">В случае успеха этот метод возвращает код отклика `200 OK` и ресурс [Permission](../resources/permission.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6b52c-127">If successful, this method returns a `200 OK` response code and [Permission](../resources/permission.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b52c-128">Пример</span><span class="sxs-lookup"><span data-stu-id="6b52c-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b52c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b52c-129">Request</span></span>

<span data-ttu-id="6b52c-130">Ниже показан пример запроса на доступ к разрешению для папки.</span><span class="sxs-lookup"><span data-stu-id="6b52c-130">Here is an example of the request to access a permission on a folder.</span></span>


# <a name="http"></a>[<span data-ttu-id="6b52c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b52c-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-item-permission", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive/items/{item-id}/permissions/{perm-id}
```
# <a name="c"></a>[<span data-ttu-id="6b52c-132">C#</span><span class="sxs-lookup"><span data-stu-id="6b52c-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-item-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b52c-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b52c-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-item-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b52c-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b52c-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-item-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b52c-135">Java</span><span class="sxs-lookup"><span data-stu-id="6b52c-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-item-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6b52c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b52c-136">Response</span></span>

<span data-ttu-id="6b52c-137">При успешном выполнении этот метод возвращает ресурс [Permission](../resources/permission.md) для указанного идентификатора.</span><span class="sxs-lookup"><span data-stu-id="6b52c-137">If successful, this method returns a [Permission](../resources/permission.md) resource for the specified ID.</span></span> 

<!-- {"blockType": "response", "@odata.type": "microsoft.graph.permission", "truncated": true} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "grantedTo": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "efee1b77-fb3b-4f65-99d6-274c11914d12"
    }
  },
  "id": "1",
  "roles": [ "write" ]
}
```

## <a name="remarks"></a><span data-ttu-id="6b52c-138">Замечания</span><span class="sxs-lookup"><span data-stu-id="6b52c-138">Remarks</span></span>

<span data-ttu-id="6b52c-139">Ресурс [Permission](../resources/permission.md) использует _аспекты_ для предоставления сведений о типе разрешения, представленного ресурсом.</span><span class="sxs-lookup"><span data-stu-id="6b52c-139">The [Permission](../resources/permission.md) resource uses _facets_ to provide information about the kind of permission represented by the resource.</span></span>

<span data-ttu-id="6b52c-p104">Разрешения с аспектом [**link**](../resources/sharinglink.md) представляют ссылки для совместного доступа, созданные в элементе. Ссылки для совместного доступа содержат уникальный токен, предоставляющий доступ к элементу для любого пользователя, у которого есть такая ссылка.</span><span class="sxs-lookup"><span data-stu-id="6b52c-p104">Permissions with a [**link**](../resources/sharinglink.md) facet represent sharing links created on the item. Sharing links contain a unique token that provides access to the item for anyone with the link.</span></span>

<span data-ttu-id="6b52c-142">Разрешения с аспектом [**invitation**](../resources/sharinginvitation.md) представляют разрешения, добавленные при приглашении определенных пользователей или групп поработать с файлом.</span><span class="sxs-lookup"><span data-stu-id="6b52c-142">Permissions with a [**invitation**](../resources/sharinginvitation.md) facet represent permissions added by inviting specific users or groups to have access to the file.</span></span>

### <a name="error-responses"></a><span data-ttu-id="6b52c-143">Отклики с ошибками</span><span class="sxs-lookup"><span data-stu-id="6b52c-143">Error responses</span></span>

<span data-ttu-id="6b52c-144">Дополнительные сведения о том, как возвращаются ошибки, см. в статье [Ошибки][error-response].</span><span class="sxs-lookup"><span data-stu-id="6b52c-144">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Get a DriveItem's sharing permissions",
  "keywords": "permission, permissions, sharing",
  "section": "documentation",
  "tocPath": "Sharing/Permissions",
  "suppressions": [
  ]
} -->
