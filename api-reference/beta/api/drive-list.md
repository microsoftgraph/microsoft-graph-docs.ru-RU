---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Создание списка ресурсов Drive
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 8826d802c6f5507887326dca9fec6b1453485830
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260342"
---
# <a name="list-available-drives"></a><span data-ttu-id="c625d-102">Создание списка доступных дисков</span><span class="sxs-lookup"><span data-stu-id="c625d-102">List available drives</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c625d-103">В этой статье рассказывается, как получить список ресурсов [Drive](../resources/drive.md), доступных для целевого объекта User, Group или [Site](../resources/site.md).</span><span class="sxs-lookup"><span data-stu-id="c625d-103">Retrieve the list of [Drive](../resources/drive.md) resources available for a target User, Group, or [Site](../resources/site.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c625d-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c625d-104">Permissions</span></span>

<span data-ttu-id="c625d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c625d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c625d-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c625d-107">Permission type</span></span>      | <span data-ttu-id="c625d-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c625d-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c625d-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c625d-109">Delegated (work or school account)</span></span> | <span data-ttu-id="c625d-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c625d-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c625d-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c625d-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c625d-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c625d-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c625d-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c625d-113">Application</span></span> | <span data-ttu-id="c625d-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c625d-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="list-a-groups-drives"></a><span data-ttu-id="c625d-115">Создание списка дисков группы</span><span class="sxs-lookup"><span data-stu-id="c625d-115">List a group's drives</span></span>

<span data-ttu-id="c625d-116">Чтобы создать список библиотек документов для группы, ваше приложение должно запросить связь **drives** в объекте Group.</span><span class="sxs-lookup"><span data-stu-id="c625d-116">To list the document libraries for a group, your app requests the **drives** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="c625d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c625d-117">HTTP request</span></span>

<!-- {"blockType": "request", "name": "group-list-drives", "scopes": "groups.read.all" } -->

```http
GET /groups/{groupId}/drives
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c625d-118">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c625d-118">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c625d-119">C#</span><span class="sxs-lookup"><span data-stu-id="c625d-119">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group-list-drives-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c625d-120">Javascript</span><span class="sxs-lookup"><span data-stu-id="c625d-120">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group-list-drives-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c625d-121">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c625d-121">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group-list-drives-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="list-a-sites-drives"></a><span data-ttu-id="c625d-122">Создание списка дисков сайта</span><span class="sxs-lookup"><span data-stu-id="c625d-122">List a site's drives</span></span>

<span data-ttu-id="c625d-123">Чтобы создать список библиотек документов для сайта, ваше приложение должно запросить связь **drives** в объекте Site.</span><span class="sxs-lookup"><span data-stu-id="c625d-123">To list the document libraries for a site, your app requests the **drives** relationship on the Site.</span></span>

<!-- {"blockType": "request", "name": "site-list-drives", "scopes": "sites.read.all" } -->

```http
GET /sites/{siteId}/drives
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c625d-124">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c625d-124">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c625d-125">C#</span><span class="sxs-lookup"><span data-stu-id="c625d-125">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/site-list-drives-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c625d-126">Javascript</span><span class="sxs-lookup"><span data-stu-id="c625d-126">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/site-list-drives-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c625d-127">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c625d-127">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/site-list-drives-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="list-a-users-drives"></a><span data-ttu-id="c625d-128">Создание списка дисков пользователя</span><span class="sxs-lookup"><span data-stu-id="c625d-128">List a user's drives</span></span>

<!-- {"blockType": "request", "name": "user-list-drives", "scopes": "files.read.all" } -->

```http
GET /users/{userId}/drives
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c625d-129">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c625d-129">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c625d-130">C#</span><span class="sxs-lookup"><span data-stu-id="c625d-130">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user-list-drives-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c625d-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="c625d-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user-list-drives-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c625d-132">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c625d-132">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user-list-drives-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="list-the-current-users-drives"></a><span data-ttu-id="c625d-133">Создание списка дисков текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="c625d-133">List the current user's drives</span></span>

<!-- {"blockType": "request", "name": "enum-drives", "scopes": "files.read" } -->

```http
GET /me/drives
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c625d-134">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c625d-134">Optional query parameters</span></span>

<span data-ttu-id="c625d-135">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` и `$orderby` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="c625d-135">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="response"></a><span data-ttu-id="c625d-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="c625d-136">Response</span></span>

<span data-ttu-id="c625d-137">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [Drive](../resources/drive.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="c625d-137">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c625d-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="c625d-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c625d-139">C#</span><span class="sxs-lookup"><span data-stu-id="c625d-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/enum-drives-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c625d-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="c625d-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/enum-drives-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c625d-141">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c625d-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/enum-drives-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="c625d-142">Примечания</span><span class="sxs-lookup"><span data-stu-id="c625d-142">Remarks</span></span>

<span data-ttu-id="c625d-143">У большинства пользователей имеется только один ресурс Drive.</span><span class="sxs-lookup"><span data-stu-id="c625d-143">Most users will only have a single Drive resource.</span></span>

<span data-ttu-id="c625d-144">Для групп и сайтов может быть доступно несколько ресурсов Drive.</span><span class="sxs-lookup"><span data-stu-id="c625d-144">Groups and Sites may have multiple Drive resources available.</span></span>

<span data-ttu-id="c625d-145">По умолчанию ресурсы Drive с аспектом [system][] скрыты.</span><span class="sxs-lookup"><span data-stu-id="c625d-145">Drives with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="c625d-146">Чтобы создать их список, включите параметр `system` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="c625d-146">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!--
{
  "type": "#page.annotation",
  "description": "List the available drives for a user, group, or site.",
  "keywords": "drive,onedrive.drive,list drives",
  "section": "documentation",
  "tocPath": "Drives/List drives",
  "suppressions": [
    "Error: /api-reference/beta/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
