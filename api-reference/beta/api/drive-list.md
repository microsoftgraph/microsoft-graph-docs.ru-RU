---
author: JeremyKelley
description: В этой статье рассказывается, как получить список ресурсов Drive, доступных для целевого объекта User, Group или Site.
ms.date: 09/10/2017
title: Создание списка ресурсов Drive
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b6588cfe45fc48988ee7a2226d1414f0357c7900
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718166"
---
# <a name="list-available-drives"></a><span data-ttu-id="d93ab-103">Создание списка доступных дисков</span><span class="sxs-lookup"><span data-stu-id="d93ab-103">List available drives</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d93ab-104">В этой статье рассказывается, как получить список ресурсов [Drive](../resources/drive.md), доступных для целевого объекта User, Group или [Site](../resources/site.md).</span><span class="sxs-lookup"><span data-stu-id="d93ab-104">Retrieve the list of [Drive](../resources/drive.md) resources available for a target User, Group, or [Site](../resources/site.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d93ab-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d93ab-105">Permissions</span></span>

<span data-ttu-id="d93ab-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d93ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d93ab-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d93ab-108">Permission type</span></span>      | <span data-ttu-id="d93ab-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d93ab-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d93ab-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d93ab-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d93ab-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d93ab-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d93ab-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d93ab-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d93ab-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d93ab-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d93ab-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d93ab-114">Application</span></span> | <span data-ttu-id="d93ab-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d93ab-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="list-a-groups-drives"></a><span data-ttu-id="d93ab-116">Создание списка дисков группы</span><span class="sxs-lookup"><span data-stu-id="d93ab-116">List a group's drives</span></span>

<span data-ttu-id="d93ab-117">Чтобы создать список библиотек документов для группы, ваше приложение должно запросить связь **drives** в объекте Group.</span><span class="sxs-lookup"><span data-stu-id="d93ab-117">To list the document libraries for a group, your app requests the **drives** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="d93ab-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d93ab-118">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d93ab-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="d93ab-119">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "group-list-drives", "scopes": "groups.read.all" } -->

```msgraph-interactive
GET /groups/{groupId}/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d93ab-120">C#</span><span class="sxs-lookup"><span data-stu-id="d93ab-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d93ab-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d93ab-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d93ab-122">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d93ab-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-a-sites-drives"></a><span data-ttu-id="d93ab-123">Создание списка дисков сайта</span><span class="sxs-lookup"><span data-stu-id="d93ab-123">List a site's drives</span></span>

<span data-ttu-id="d93ab-124">Чтобы создать список библиотек документов для сайта, ваше приложение должно запросить связь **drives** в объекте Site.</span><span class="sxs-lookup"><span data-stu-id="d93ab-124">To list the document libraries for a site, your app requests the **drives** relationship on the Site.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d93ab-125">HTTP</span><span class="sxs-lookup"><span data-stu-id="d93ab-125">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "site-list-drives", "scopes": "sites.read.all" } -->

```msgraph-interactive
GET /sites/{siteId}/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d93ab-126">C#</span><span class="sxs-lookup"><span data-stu-id="d93ab-126">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/site-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d93ab-127">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d93ab-127">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/site-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d93ab-128">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d93ab-128">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/site-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-a-users-drives"></a><span data-ttu-id="d93ab-129">Создание списка дисков пользователя</span><span class="sxs-lookup"><span data-stu-id="d93ab-129">List a user's drives</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d93ab-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="d93ab-130">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "user-list-drives", "scopes": "files.read.all" } -->

```msgraph-interactive
GET /users/{userId}/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d93ab-131">C#</span><span class="sxs-lookup"><span data-stu-id="d93ab-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d93ab-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d93ab-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d93ab-133">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d93ab-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-the-current-users-drives"></a><span data-ttu-id="d93ab-134">Создание списка дисков текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="d93ab-134">List the current user's drives</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d93ab-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d93ab-135">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "enum-drives", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d93ab-136">C#</span><span class="sxs-lookup"><span data-stu-id="d93ab-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d93ab-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d93ab-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d93ab-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="d93ab-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="optional-query-parameters"></a><span data-ttu-id="d93ab-139">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d93ab-139">Optional query parameters</span></span>

<span data-ttu-id="d93ab-140">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` и `$orderby` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d93ab-140">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="d93ab-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="d93ab-141">Response</span></span>

<span data-ttu-id="d93ab-142">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [Drive](../resources/drive.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="d93ab-142">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.drive)",
       "name": ["group-list-drives", "site-list-drives", "user-list-drives", "enum-drives"],
       "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "942CAEB0-13AE-491B-85E4-7557CDC0F25F",
      "driveType": "documentLibrary",
      "name": "Shared Documents",
      "owner": {
        "user": {
          "id": "AE2A1EE9-81A7-423C-ABE4-B945F47509BB",
          "displayName": "Ryan Gregg"
        }
      }
    },
    {
      "id": "C1CD3ED9-0E98-4B0B-82D3-C8FB784B9DCC",
      "driveType": "documentLibrary",
      "name": "Contoso Project Files",
      "owner": {
        "user": {
          "id": "406B2281-18E8-4416-9857-38C531B904F1",
          "displayName": "Daron Spektor"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="d93ab-143">Примечания</span><span class="sxs-lookup"><span data-stu-id="d93ab-143">Remarks</span></span>

<span data-ttu-id="d93ab-144">У большинства пользователей имеется только один ресурс Drive.</span><span class="sxs-lookup"><span data-stu-id="d93ab-144">Most users will only have a single Drive resource.</span></span>

<span data-ttu-id="d93ab-145">Для групп и сайтов может быть доступно несколько ресурсов Drive.</span><span class="sxs-lookup"><span data-stu-id="d93ab-145">Groups and Sites may have multiple Drive resources available.</span></span>

<span data-ttu-id="d93ab-146">По умолчанию ресурсы Drive с аспектом [system][] скрыты.</span><span class="sxs-lookup"><span data-stu-id="d93ab-146">Drives with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="d93ab-147">Чтобы создать их список, включите параметр `system` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="d93ab-147">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!--
{
  "type": "#page.annotation",
  "description": "List the available drives for a user, group, or site.",
  "keywords": "drive,onedrive.drive,list drives",
  "section": "documentation",
  "tocPath": "Drives/List drives",
  "suppressions": [
  ]
}
-->
