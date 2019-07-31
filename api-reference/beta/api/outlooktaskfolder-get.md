---
title: Получение outlookTaskFolder
description: Получение свойств и связей указанной папки задач Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: c7288f3a5abc5dbc5327ed11cf5680906b45c98a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992530"
---
# <a name="get-outlooktaskfolder"></a><span data-ttu-id="06783-103">Получение outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="06783-103">Get outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06783-104">Получение свойств и связей указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="06783-104">Get the properties and relationships of the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="06783-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="06783-105">Permissions</span></span>
<span data-ttu-id="06783-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="06783-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="06783-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="06783-108">Permission type</span></span>      | <span data-ttu-id="06783-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="06783-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06783-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="06783-110">Delegated (work or school account)</span></span> | <span data-ttu-id="06783-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="06783-111">Tasks.Read</span></span>    |
|<span data-ttu-id="06783-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="06783-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06783-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="06783-113">Tasks.Read</span></span>    |
|<span data-ttu-id="06783-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="06783-114">Application</span></span> | <span data-ttu-id="06783-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="06783-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="06783-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="06783-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}
GET /me/outlook/taskGroups/{id}/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="06783-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="06783-117">Optional query parameters</span></span>
<span data-ttu-id="06783-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="06783-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="06783-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="06783-119">Request headers</span></span>
| <span data-ttu-id="06783-120">Имя</span><span class="sxs-lookup"><span data-stu-id="06783-120">Name</span></span>      |<span data-ttu-id="06783-121">Описание</span><span class="sxs-lookup"><span data-stu-id="06783-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="06783-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="06783-122">Authorization</span></span>  | <span data-ttu-id="06783-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="06783-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="06783-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="06783-125">Request body</span></span>
<span data-ttu-id="06783-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="06783-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06783-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="06783-127">Response</span></span>

<span data-ttu-id="06783-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [outlookTaskFolder](../resources/outlooktaskfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="06783-128">If successful, this method returns a `200 OK` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="06783-129">Пример</span><span class="sxs-lookup"><span data-stu-id="06783-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="06783-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="06783-130">Request</span></span>
<span data-ttu-id="06783-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="06783-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="06783-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="06783-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskfolder"
}-->
```http
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAAABrJAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="06783-133">C#</span><span class="sxs-lookup"><span data-stu-id="06783-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="06783-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="06783-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="06783-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="06783-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="06783-136">Java</span><span class="sxs-lookup"><span data-stu-id="06783-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-outlooktaskfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="06783-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="06783-137">Response</span></span>
<span data-ttu-id="06783-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="06783-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 151

{
  "id": "AAMkADIyAAAAABrJAAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAAAAeAA==",
  "isDefaultFolder": false,
  "name": "Monthly tasks",
  "parentGroupKey": "0006f0b7-0000-0000-c000-000000000046"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
