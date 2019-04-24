---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Создание списка ресурсов Drive
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 6a5d716aef5a47acf3f0752d91a478f2d3299a24
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454738"
---
# <a name="list-available-drives"></a><span data-ttu-id="b9301-102">Создание списка доступных дисков</span><span class="sxs-lookup"><span data-stu-id="b9301-102">List available drives</span></span>

<span data-ttu-id="b9301-103">В этой статье рассказывается, как получить список ресурсов [Drive](../resources/drive.md), доступных для целевого объекта User, Group или [Site](../resources/site.md).</span><span class="sxs-lookup"><span data-stu-id="b9301-103">Retrieve the list of [Drive](../resources/drive.md) resources available for a target User, Group, or [Site](../resources/site.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b9301-104">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b9301-104">Permissions</span></span>

<span data-ttu-id="b9301-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9301-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9301-107">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b9301-107">Permission type</span></span>      | <span data-ttu-id="b9301-108">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b9301-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b9301-109">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b9301-109">Delegated (work or school account)</span></span> | <span data-ttu-id="b9301-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9301-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b9301-111">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b9301-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b9301-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9301-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b9301-113">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b9301-113">Application</span></span> | <span data-ttu-id="b9301-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9301-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="list-a-groups-drives"></a><span data-ttu-id="b9301-115">Создание списка дисков группы</span><span class="sxs-lookup"><span data-stu-id="b9301-115">List a group's drives</span></span>

<span data-ttu-id="b9301-116">Чтобы создать список библиотек документов для группы, ваше приложение должно запросить связь **drives** в объекте Group.</span><span class="sxs-lookup"><span data-stu-id="b9301-116">To list the document libraries for a group, your app requests the **drives** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="b9301-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b9301-117">HTTP request</span></span>

<!-- {"blockType": "request", "name": "group-list-drives", "scopes": "groups.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drives
```

## <a name="list-a-sites-drives"></a><span data-ttu-id="b9301-118">Создание списка дисков сайта</span><span class="sxs-lookup"><span data-stu-id="b9301-118">List a site's drives</span></span>

<span data-ttu-id="b9301-119">Чтобы создать список библиотек документов для сайта, ваше приложение должно запросить связь **drives** в объекте Site.</span><span class="sxs-lookup"><span data-stu-id="b9301-119">To list the document libraries for a site, your app requests the **drives** relationship on the Site.</span></span>

<!-- {"blockType": "request", "name": "site-list-drives", "scopes": "sites.read.all", "tags": "service.graph" } -->

```http
GET /sites/{siteId}/drives
```

## <a name="list-a-users-drives"></a><span data-ttu-id="b9301-120">Создание списка дисков пользователя</span><span class="sxs-lookup"><span data-stu-id="b9301-120">List a user's drives</span></span>

<!-- {"blockType": "request", "name": "user-list-drives", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /users/{userId}/drives
```

## <a name="list-the-current-users-drives"></a><span data-ttu-id="b9301-121">Создание списка дисков текущего пользователя</span><span class="sxs-lookup"><span data-stu-id="b9301-121">List the current user's drives</span></span>

<!-- {"blockType": "request", "name": "enum-drives", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drives
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b9301-122">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b9301-122">Optional query parameters</span></span>

<span data-ttu-id="b9301-123">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) `$expand`, `$select`, `$skipToken`, `$top` и `$orderby` для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b9301-123">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>


## <a name="response"></a><span data-ttu-id="b9301-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="b9301-124">Response</span></span>

<span data-ttu-id="b9301-125">При успешном выполнении этот метод возвращает код ответа `200 OK` и коллекцию объектов [Drive](../resources/drive.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b9301-125">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="b9301-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="b9301-126">Remarks</span></span>

<span data-ttu-id="b9301-127">У большинства пользователей имеется только один ресурс Drive.</span><span class="sxs-lookup"><span data-stu-id="b9301-127">Most users will only have a single Drive resource.</span></span>

<span data-ttu-id="b9301-128">Для групп и сайтов может быть доступно несколько ресурсов Drive.</span><span class="sxs-lookup"><span data-stu-id="b9301-128">Groups and Sites may have multiple Drive resources available.</span></span>

<span data-ttu-id="b9301-129">По умолчанию ресурсы Drive с аспектом [system][] скрыты.</span><span class="sxs-lookup"><span data-stu-id="b9301-129">Drives with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="b9301-130">Чтобы создать их список, включите параметр `system` в оператор `$select`.</span><span class="sxs-lookup"><span data-stu-id="b9301-130">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "List the available drives for a user, group, or site.",
  "keywords": "drive,onedrive.drive,list drives",
  "section": "documentation",
  "tocPath": "Drives/List drives"
} -->
