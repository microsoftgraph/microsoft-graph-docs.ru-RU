---
title: Список childFolders
description: 'Получите коллекцию папок в указанной папке. Можно использовать `.../me/MailFolders` ярлык для получения верхнего уровня '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 96dec9ca1ba6dbd8e50e8eb978756a98657d2c9d
ms.sourcegitcommit: bdbc68ed8eaf43386d2cdf7b79e64ebbe1e860c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/13/2019
ms.locfileid: "29967237"
---
# <a name="list-childfolders"></a><span data-ttu-id="e4f13-104">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="e4f13-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4f13-p102">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/MailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="e4f13-p102">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="e4f13-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4f13-107">Permissions</span></span>

<span data-ttu-id="e4f13-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4f13-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e4f13-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4f13-110">Permission type</span></span>                        | <span data-ttu-id="e4f13-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4f13-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="e4f13-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4f13-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e4f13-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4f13-113">Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="e4f13-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4f13-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4f13-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4f13-115">Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="e4f13-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4f13-116">Application</span></span>                            | <span data-ttu-id="e4f13-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4f13-117">Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="e4f13-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4f13-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e4f13-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e4f13-119">Optional query parameters</span></span>

<span data-ttu-id="e4f13-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e4f13-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e4f13-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4f13-121">Request headers</span></span>

| <span data-ttu-id="e4f13-122">Имя</span><span class="sxs-lookup"><span data-stu-id="e4f13-122">Name</span></span>          | <span data-ttu-id="e4f13-123">Тип</span><span class="sxs-lookup"><span data-stu-id="e4f13-123">Type</span></span>   | <span data-ttu-id="e4f13-124">Описание</span><span class="sxs-lookup"><span data-stu-id="e4f13-124">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="e4f13-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4f13-125">Authorization</span></span> | <span data-ttu-id="e4f13-126">string</span><span class="sxs-lookup"><span data-stu-id="e4f13-126">string</span></span> | <span data-ttu-id="e4f13-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4f13-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e4f13-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4f13-129">Request body</span></span>

<span data-ttu-id="e4f13-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e4f13-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e4f13-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="e4f13-131">Response</span></span>

<span data-ttu-id="e4f13-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [MailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e4f13-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e4f13-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="e4f13-133">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="e4f13-134">В примере 1: Список почтовых папок</span><span class="sxs-lookup"><span data-stu-id="e4f13-134">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="e4f13-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4f13-135">Request</span></span>

<span data-ttu-id="e4f13-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4f13-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="e4f13-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4f13-137">Response</span></span>

<span data-ttu-id="e4f13-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e4f13-138">The following is an example of the response.</span></span>

> <span data-ttu-id="e4f13-139">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e4f13-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e4f13-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4f13-140">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "AAMkAGVmMDEzA",
      "displayName": "Internal Screens",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 2,
      "totalItemCount": 2,
      "wellKnownName": null
    },
    {
      "id": "AAMkAGVmMDEzB",
      "displayName": "Project Falcon",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 0,
      "unreadItemCount": 5,
      "totalItemCount": 5,
      "wellKnownName": null
    },
    {
      "id": "AAMkAGVmMDEzMA",
      "displayName": "Finder",
      "parentFolderId": "AAMkAGVmMDEzM",
      "childFolderCount": 4,
      "unreadItemCount": 0,
      "totalItemCount": 0,
      "wellKnownName": "searchfolders"
    }
  ]
}
```

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="e4f13-141">Пример 2: Список почтовых папок поиска</span><span class="sxs-lookup"><span data-stu-id="e4f13-141">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="e4f13-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4f13-142">Request</span></span>

<span data-ttu-id="e4f13-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4f13-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response"></a><span data-ttu-id="e4f13-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4f13-144">Response</span></span>

<span data-ttu-id="e4f13-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e4f13-145">The following is an example of the response.</span></span>

> <span data-ttu-id="e4f13-146">**Примечание.**  Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e4f13-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e4f13-147">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4f13-147">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mailSearchFolder",
      "id": "AAMkAGE1NWMz",
      "displayName": "Get MyAnalytics",
      "parentFolderId": "AAMkAGE1NWMx",
      "childFolderCount": 0,
      "unreadItemCount": 6,
      "totalItemCount": 6,
      "wellKnownName": null,
      "isSupported": true,
      "filterQuery": "contains(subject, 'MyAnalytics')"
    },
    {
      "@odata.type": "#microsoft.graph.mailSearchFolder",
      "id": "AAMkAGE1NWMy",
      "displayName": "Action Required",
      "parentFolderId": "AAMkAGE1NWMx",
      "childFolderCount": 0,
      "unreadItemCount": 2,
      "totalItemCount": 4,
      "wellKnownName": null,
      "isSupported": true,
      "filterQuery": "contains(subject, 'ACTION REQUIRED')"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-list-childfolders.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
