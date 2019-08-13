---
title: Список Таскфолдерс
description: Получение папок задач Outlook в определенном outlookTaskGroup.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1c61a5c07f23932789e0e9d28b8d176001c31f64
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36349704"
---
# <a name="list-taskfolders"></a><span data-ttu-id="a6e59-103">Список Таскфолдерс</span><span class="sxs-lookup"><span data-stu-id="a6e59-103">List taskFolders</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6e59-104">Получение папок задач Outlook в определенном [outlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="a6e59-104">Get Outlook task folders in a specific [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="a6e59-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6e59-105">Permissions</span></span>
<span data-ttu-id="a6e59-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6e59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6e59-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6e59-108">Permission type</span></span>      | <span data-ttu-id="a6e59-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6e59-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6e59-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6e59-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a6e59-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="a6e59-111">Tasks.Read</span></span>    |
|<span data-ttu-id="a6e59-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6e59-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6e59-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="a6e59-113">Tasks.Read</span></span>    |
|<span data-ttu-id="a6e59-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6e59-114">Application</span></span> | <span data-ttu-id="a6e59-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6e59-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6e59-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6e59-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskGroups/{id}/taskFolders
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a6e59-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a6e59-117">Optional query parameters</span></span>
<span data-ttu-id="a6e59-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="a6e59-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6e59-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6e59-119">Request headers</span></span>
| <span data-ttu-id="a6e59-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a6e59-120">Name</span></span>      |<span data-ttu-id="a6e59-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a6e59-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a6e59-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6e59-122">Authorization</span></span>  | <span data-ttu-id="a6e59-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6e59-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6e59-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a6e59-125">Request body</span></span>
<span data-ttu-id="a6e59-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a6e59-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6e59-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6e59-127">Response</span></span>

<span data-ttu-id="a6e59-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [outlookTaskFolder](../resources/outlooktaskfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a6e59-128">If successful, this method returns a `200 OK` response code and collection of [outlookTaskFolder](../resources/outlooktaskfolder.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a6e59-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a6e59-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a6e59-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6e59-130">Request</span></span>
<span data-ttu-id="a6e59-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6e59-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a6e59-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6e59-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_taskfolders"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=/taskFolders
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a6e59-133">C#</span><span class="sxs-lookup"><span data-stu-id="a6e59-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-taskfolders-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a6e59-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6e59-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-taskfolders-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a6e59-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="a6e59-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-taskfolders-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="a6e59-136">Java</span><span class="sxs-lookup"><span data-stu-id="a6e59-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-taskfolders-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a6e59-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6e59-137">Response</span></span>
<span data-ttu-id="a6e59-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6e59-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
