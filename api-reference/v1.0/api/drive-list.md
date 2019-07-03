---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Создание списка ресурсов Drive
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 21c811e501116c8865686a9f5efb379e3631c229
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35458511"
---
# <a name="list-available-drives"></a><span data-ttu-id="373a9-102">Создание списка доступных дисков</span><span class="sxs-lookup"><span data-stu-id="373a9-102">List available drives</span></span>

<span data-ttu-id="373a9-103">В этой статье рассказывается, как получить список ресурсов [Drive](../resources/drive.md), доступных для целевого объекта User, Group или [Site](../resources/site.md).</span><span class="sxs-lookup"><span data-stu-id="373a9-103">Retrieve the list of [Drive](../resources/drive.md) resources available for a target User, Group, or [Site](../resources/site.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="373a9-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="373a9-104">Permissions</span></span>

<span data-ttu-id="373a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="373a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="373a9-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="373a9-107">Permission type</span></span>      | <span data-ttu-id="373a9-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="373a9-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="373a9-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="373a9-109">Delegated (work or school account)</span></span> | <span data-ttu-id="373a9-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="373a9-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="373a9-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="373a9-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="373a9-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="373a9-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="373a9-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="373a9-113">Application</span></span> | <span data-ttu-id="373a9-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="373a9-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="list-a-groups-drives"></a><span data-ttu-id="373a9-115">Создание списка дисков группы</span><span class="sxs-lookup"><span data-stu-id="373a9-115">List a group's drives</span></span>

<span data-ttu-id="373a9-116">Чтобы создать список библиотек документов для группы, ваше приложение должно запросить связь **drives** в объекте Group.</span><span class="sxs-lookup"><span data-stu-id="373a9-116">To list the document libraries for a group, your app requests the **drives** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="373a9-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="373a9-117">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="373a9-118">HTTP</span><span class="sxs-lookup"><span data-stu-id="373a9-118">--Http</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "group-list-drives", "scopes": "groups.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="373a9-119">C#</span><span class="sxs-lookup"><span data-stu-id="373a9-119">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="373a9-120">JavaScript</span><span class="sxs-lookup"><span data-stu-id="373a9-120">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="373a9-121">Objective-C</span><span class="sxs-lookup"><span data-stu-id="373a9-121">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-a-sites-drives"></a><span data-ttu-id="373a9-122">Создание списка дисков сайта</span><span class="sxs-lookup"><span data-stu-id="373a9-122">List a site's drives</span></span>

<span data-ttu-id="373a9-123">Чтобы создать список библиотек документов для сайта, ваше приложение должно запросить связь **drives** в объекте Site.</span><span class="sxs-lookup"><span data-stu-id="373a9-123">To list the document libraries for a site, your app requests the **drives** relationship on the Site.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="373a9-124">HTTP</span><span class="sxs-lookup"><span data-stu-id="373a9-124">--Http</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "site-list-drives", "scopes": "sites.read.all", "tags": "service.graph" } -->

```http
GET /sites/{siteId}/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="373a9-125">C#</span><span class="sxs-lookup"><span data-stu-id="373a9-125">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/site-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="373a9-126">JavaScript</span><span class="sxs-lookup"><span data-stu-id="373a9-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/site-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="373a9-127">Objective-C</span><span class="sxs-lookup"><span data-stu-id="373a9-127">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/site-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-a-users-drives"></a><span data-ttu-id="373a9-128">Получение списка дисков пользователя</span><span class="sxs-lookup"><span data-stu-id="373a9-128">List a user's drives</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="373a9-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="373a9-129">--Http</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "user-list-drives", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /users/{userId}/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="373a9-130">C#</span><span class="sxs-lookup"><span data-stu-id="373a9-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="373a9-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="373a9-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="373a9-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="373a9-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-the-current-users-drives"></a><span data-ttu-id="373a9-133">Получение списка дисков текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="373a9-133">List the current user's drives</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="373a9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="373a9-134">--Http</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "enum-drives", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="373a9-135">C#</span><span class="sxs-lookup"><span data-stu-id="373a9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="373a9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="373a9-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="373a9-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="373a9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="optional-query-parameters"></a><span data-ttu-id="373a9-138">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="373a9-138">Optional query parameters</span></span>

<span data-ttu-id="373a9-139">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` и `$orderby` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="373a9-139">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>


## <a name="response"></a><span data-ttu-id="373a9-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="373a9-140">Response</span></span>

<span data-ttu-id="373a9-141">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [Drive](../resources/drive.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="373a9-141">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="373a9-142">Примечания</span><span class="sxs-lookup"><span data-stu-id="373a9-142">Remarks</span></span>

<span data-ttu-id="373a9-143">У большинства пользователей имеется только один ресурс Drive.</span><span class="sxs-lookup"><span data-stu-id="373a9-143">Most users will only have a single Drive resource.</span></span>

<span data-ttu-id="373a9-144">Для групп и сайтов может быть доступно несколько ресурсов Drive.</span><span class="sxs-lookup"><span data-stu-id="373a9-144">Groups and Sites may have multiple Drive resources available.</span></span>

<span data-ttu-id="373a9-145">По умолчанию ресурсы Drive с аспектом [system][] скрыты.</span><span class="sxs-lookup"><span data-stu-id="373a9-145">Drives with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="373a9-146">Чтобы создать их список, включите параметр `system` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="373a9-146">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "List the available drives for a user, group, or site.",
  "keywords": "drive,onedrive.drive,list drives",
  "section": "documentation",
  "tocPath": "Drives/List drives",
  "suppressions": [
  ]
} -->
