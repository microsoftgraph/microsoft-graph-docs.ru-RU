---
title: Список Таскфолдерс
description: Получение папок задач Outlook в определенном outlookTaskGroup.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b245d2a0a1621fc7336819ad1fc66e8dd375bd7f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414009"
---
# <a name="list-taskfolders"></a><span data-ttu-id="152a1-103">Список Таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="152a1-103">List taskFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="152a1-104">Получение папок задач Outlook в определенном [outlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="152a1-104">Get Outlook task folders in a specific [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="152a1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="152a1-105">Permissions</span></span>
<span data-ttu-id="152a1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="152a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="152a1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="152a1-108">Permission type</span></span>      | <span data-ttu-id="152a1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="152a1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="152a1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="152a1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="152a1-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="152a1-111">Tasks.Read</span></span>    |
|<span data-ttu-id="152a1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="152a1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="152a1-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="152a1-113">Tasks.Read</span></span>    |
|<span data-ttu-id="152a1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="152a1-114">Application</span></span> | <span data-ttu-id="152a1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="152a1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="152a1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="152a1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}/taskFolders
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="152a1-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="152a1-117">Optional query parameters</span></span>
<span data-ttu-id="152a1-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="152a1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="152a1-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="152a1-119">Request headers</span></span>
| <span data-ttu-id="152a1-120">Имя</span><span class="sxs-lookup"><span data-stu-id="152a1-120">Name</span></span>      |<span data-ttu-id="152a1-121">Описание</span><span class="sxs-lookup"><span data-stu-id="152a1-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="152a1-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="152a1-122">Authorization</span></span>  | <span data-ttu-id="152a1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="152a1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="152a1-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="152a1-125">Request body</span></span>
<span data-ttu-id="152a1-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="152a1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="152a1-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="152a1-127">Response</span></span>

<span data-ttu-id="152a1-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [outlookTaskFolder](../resources/outlooktaskfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="152a1-128">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="152a1-129">Пример</span><span class="sxs-lookup"><span data-stu-id="152a1-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="152a1-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="152a1-130">Request</span></span>
<span data-ttu-id="152a1-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="152a1-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="152a1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="152a1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=/taskFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="152a1-133">C#</span><span class="sxs-lookup"><span data-stu-id="152a1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="152a1-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="152a1-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="152a1-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="152a1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="152a1-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="152a1-136">Response</span></span>
<span data-ttu-id="152a1-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="152a1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 200

{
  "value": [
    {
      "id": "AAMkADIyAAAhrbPXAAA=",
      "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAOlA==",
      "isDefaultFolder": false,
      "name": "Cooking",
      "parentGroupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"
    }

  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List taskFolders",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
