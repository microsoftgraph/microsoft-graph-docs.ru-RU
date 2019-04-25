---
title: Список childFolders
description: 'Получение коллекции папок в указанной папке. Вы можете использовать `.../me/MailFolders` ярлык для получения верхнего уровня '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 96dec9ca1ba6dbd8e50e8eb978756a98657d2c9d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540881"
---
# <a name="list-childfolders"></a><span data-ttu-id="c7ae2-104">Вывод списка объектов childFolder</span><span class="sxs-lookup"><span data-stu-id="c7ae2-104">List childFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c7ae2-p102">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/MailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="c7ae2-p102">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="c7ae2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c7ae2-107">Permissions</span></span>

<span data-ttu-id="c7ae2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c7ae2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c7ae2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c7ae2-110">Permission type</span></span>                        | <span data-ttu-id="c7ae2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c7ae2-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="c7ae2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c7ae2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="c7ae2-113">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7ae2-113">Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="c7ae2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c7ae2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c7ae2-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7ae2-115">Mail.Read, Mail.ReadWrite</span></span>           |
| <span data-ttu-id="c7ae2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c7ae2-116">Application</span></span>                            | <span data-ttu-id="c7ae2-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c7ae2-117">Mail.Read, Mail.ReadWrite</span></span>           |

## <a name="http-request"></a><span data-ttu-id="c7ae2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c7ae2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c7ae2-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="c7ae2-119">Optional query parameters</span></span>

<span data-ttu-id="c7ae2-120">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="c7ae2-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c7ae2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c7ae2-121">Request headers</span></span>

| <span data-ttu-id="c7ae2-122">Имя</span><span class="sxs-lookup"><span data-stu-id="c7ae2-122">Name</span></span>          | <span data-ttu-id="c7ae2-123">Тип</span><span class="sxs-lookup"><span data-stu-id="c7ae2-123">Type</span></span>   | <span data-ttu-id="c7ae2-124">Описание</span><span class="sxs-lookup"><span data-stu-id="c7ae2-124">Description</span></span>               |
|:--------------|:-------|:--------------------------|
| <span data-ttu-id="c7ae2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c7ae2-125">Authorization</span></span> | <span data-ttu-id="c7ae2-126">string</span><span class="sxs-lookup"><span data-stu-id="c7ae2-126">string</span></span> | <span data-ttu-id="c7ae2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c7ae2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c7ae2-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c7ae2-129">Request body</span></span>

<span data-ttu-id="c7ae2-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c7ae2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c7ae2-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="c7ae2-131">Response</span></span>

<span data-ttu-id="c7ae2-132">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [MailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c7ae2-132">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c7ae2-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="c7ae2-133">Examples</span></span>

### <a name="example-1-list-mail-folders"></a><span data-ttu-id="c7ae2-134">Пример 1: список почтовых папок</span><span class="sxs-lookup"><span data-stu-id="c7ae2-134">Example 1: List mail folders</span></span>

#### <a name="request"></a><span data-ttu-id="c7ae2-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7ae2-135">Request</span></span>

<span data-ttu-id="c7ae2-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7ae2-136">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="c7ae2-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7ae2-137">Response</span></span>

<span data-ttu-id="c7ae2-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c7ae2-138">The following is an example of the response.</span></span>

> <span data-ttu-id="c7ae2-139">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c7ae2-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c7ae2-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7ae2-140">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-list-mail-search-folders"></a><span data-ttu-id="c7ae2-141">Пример 2: список папок поиска почты</span><span class="sxs-lookup"><span data-stu-id="c7ae2-141">Example 2: List mail search folders</span></span>

#### <a name="request"></a><span data-ttu-id="c7ae2-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="c7ae2-142">Request</span></span>

<span data-ttu-id="c7ae2-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c7ae2-143">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->

```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response"></a><span data-ttu-id="c7ae2-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="c7ae2-144">Response</span></span>

<span data-ttu-id="c7ae2-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c7ae2-145">The following is an example of the response.</span></span>

> <span data-ttu-id="c7ae2-146">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c7ae2-146">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c7ae2-147">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c7ae2-147">All the properties will be returned from an actual call.</span></span>

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
