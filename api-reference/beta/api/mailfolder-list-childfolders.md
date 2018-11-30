---
title: Список childFolders
description: 'Получите коллекцию папок в указанной папке. Можно использовать `.../me/MailFolders` ярлык для получения верхнего уровня '
ms.openlocfilehash: 826ce59f0f808ee94107a41e76207e83632361ff
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079551"
---
# <a name="list-childfolders"></a><span data-ttu-id="cbd74-104">Список childFolders</span><span class="sxs-lookup"><span data-stu-id="cbd74-104">List childFolders</span></span>

> <span data-ttu-id="cbd74-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cbd74-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbd74-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cbd74-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cbd74-p103">Получение коллекции папок в указанной папке. С помощью ярлыка `.../me/MailFolders` вы можете получить коллекцию папок верхнего уровня и перейти к другой папке.</span><span class="sxs-lookup"><span data-stu-id="cbd74-p103">Get the folder collection under the specified folder. You can use the `.../me/MailFolders` shortcut to get the top-level folder collection and navigate to another folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="cbd74-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cbd74-109">Permissions</span></span>
<span data-ttu-id="cbd74-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cbd74-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbd74-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cbd74-112">Permission type</span></span>      | <span data-ttu-id="cbd74-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cbd74-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cbd74-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cbd74-114">Delegated (work or school account)</span></span> | <span data-ttu-id="cbd74-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbd74-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="cbd74-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cbd74-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cbd74-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbd74-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="cbd74-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cbd74-118">Application</span></span> | <span data-ttu-id="cbd74-119">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cbd74-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="cbd74-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cbd74-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}/childFolders
GET /users/{id | userPrincipalName}/mailFolders/{id}/childFolders
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cbd74-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cbd74-121">Optional query parameters</span></span>
<span data-ttu-id="cbd74-122">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="cbd74-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cbd74-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cbd74-123">Request headers</span></span>
| <span data-ttu-id="cbd74-124">Имя</span><span class="sxs-lookup"><span data-stu-id="cbd74-124">Name</span></span>       | <span data-ttu-id="cbd74-125">Тип</span><span class="sxs-lookup"><span data-stu-id="cbd74-125">Type</span></span> | <span data-ttu-id="cbd74-126">Описание</span><span class="sxs-lookup"><span data-stu-id="cbd74-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cbd74-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbd74-127">Authorization</span></span>  | <span data-ttu-id="cbd74-128">string</span><span class="sxs-lookup"><span data-stu-id="cbd74-128">string</span></span>  | <span data-ttu-id="cbd74-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cbd74-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cbd74-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cbd74-131">Request body</span></span>
<span data-ttu-id="cbd74-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cbd74-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbd74-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="cbd74-133">Response</span></span>
<span data-ttu-id="cbd74-134">В случае успеха этот метод возвращает код отклика `200 OK` и коллекцию объектов [MailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="cbd74-134">If successful, this method returns a `200 OK` response code and collection of [MailFolder](../resources/mailfolder.md) objects in the response body.</span></span>

## <a name="example-1"></a><span data-ttu-id="cbd74-135">Пример 1</span><span class="sxs-lookup"><span data-stu-id="cbd74-135">Example 1</span></span>
#### <a name="request-1"></a><span data-ttu-id="cbd74-136">Запрос 1</span><span class="sxs-lookup"><span data-stu-id="cbd74-136">Request 1</span></span>
<span data-ttu-id="cbd74-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbd74-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/childFolders
```

#### <a name="response-1"></a><span data-ttu-id="cbd74-138">Ответ 1</span><span class="sxs-lookup"><span data-stu-id="cbd74-138">Response 1</span></span>
<span data-ttu-id="cbd74-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cbd74-139">The following is an example of the response.</span></span>
><span data-ttu-id="cbd74-140">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="cbd74-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cbd74-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cbd74-141">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

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

## <a name="example-2"></a><span data-ttu-id="cbd74-142">Пример 2</span><span class="sxs-lookup"><span data-stu-id="cbd74-142">Example 2</span></span>
#### <a name="request-2"></a><span data-ttu-id="cbd74-143">Запрос 2</span><span class="sxs-lookup"><span data-stu-id="cbd74-143">Request 2</span></span>
<span data-ttu-id="cbd74-144">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cbd74-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_childfolders_of_searchfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/mailFolders/searchfolders/childFolders
```

#### <a name="response-2"></a><span data-ttu-id="cbd74-145">Ответ 2</span><span class="sxs-lookup"><span data-stu-id="cbd74-145">Response 2</span></span>
<span data-ttu-id="cbd74-146">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cbd74-146">The following is an example of the response.</span></span>
><span data-ttu-id="cbd74-147">**Примечание:** объект ответа, показанный здесь может быть сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="cbd74-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cbd74-148">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cbd74-148">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailSearchFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List childFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
