---
title: Получение outlookTaskFolder
description: Получение свойств и связей указанной папки задач Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 82e482f740b4292b723971e21682df32160a8a72
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723695"
---
# <a name="get-outlooktaskfolder"></a><span data-ttu-id="50bdb-103">Получение outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="50bdb-103">Get outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50bdb-104">Получение свойств и связей указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="50bdb-104">Get the properties and relationships of the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="50bdb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="50bdb-105">Permissions</span></span>
<span data-ttu-id="50bdb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="50bdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50bdb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="50bdb-108">Permission type</span></span>      | <span data-ttu-id="50bdb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="50bdb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50bdb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="50bdb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="50bdb-111">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="50bdb-111">Tasks.Read</span></span>    |
|<span data-ttu-id="50bdb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="50bdb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50bdb-113">Tasks.Read</span><span class="sxs-lookup"><span data-stu-id="50bdb-113">Tasks.Read</span></span>    |
|<span data-ttu-id="50bdb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="50bdb-114">Application</span></span> | <span data-ttu-id="50bdb-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="50bdb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="50bdb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="50bdb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/outlook/taskFolders/{id}
GET /me/outlook/taskGroups/{id}/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskFolders/{id}
GET /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="50bdb-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="50bdb-117">Optional query parameters</span></span>
<span data-ttu-id="50bdb-118">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="50bdb-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="50bdb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="50bdb-119">Request headers</span></span>
| <span data-ttu-id="50bdb-120">Имя</span><span class="sxs-lookup"><span data-stu-id="50bdb-120">Name</span></span>      |<span data-ttu-id="50bdb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="50bdb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="50bdb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="50bdb-122">Authorization</span></span>  | <span data-ttu-id="50bdb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="50bdb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="50bdb-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="50bdb-125">Request body</span></span>
<span data-ttu-id="50bdb-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="50bdb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50bdb-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="50bdb-127">Response</span></span>

<span data-ttu-id="50bdb-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [outlookTaskFolder](../resources/outlooktaskfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="50bdb-128">If successful, this method returns a `200 OK` response code and [outlookTaskFolder](../resources/outlooktaskfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="50bdb-129">Пример</span><span class="sxs-lookup"><span data-stu-id="50bdb-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="50bdb-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="50bdb-130">Request</span></span>
<span data-ttu-id="50bdb-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="50bdb-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="50bdb-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="50bdb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_outlooktaskfolder"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAAABrJAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="50bdb-133">C#</span><span class="sxs-lookup"><span data-stu-id="50bdb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="50bdb-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50bdb-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="50bdb-135">Цель — C</span><span class="sxs-lookup"><span data-stu-id="50bdb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="50bdb-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="50bdb-136">Response</span></span>
<span data-ttu-id="50bdb-p103">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="50bdb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
