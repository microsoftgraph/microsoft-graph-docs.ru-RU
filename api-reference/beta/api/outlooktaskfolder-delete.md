---
title: Удаление outlookTaskFolder
description: Удаление указанной папки задач Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: d5280d0919c7f18d93191c3ff888adae3f1c6f01
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414090"
---
# <a name="delete-outlooktaskfolder"></a><span data-ttu-id="47250-103">Удаление outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="47250-103">Delete outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47250-104">Удаление указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="47250-104">Delete the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="47250-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47250-105">Permissions</span></span>
<span data-ttu-id="47250-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47250-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47250-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47250-108">Permission type</span></span>      | <span data-ttu-id="47250-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47250-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47250-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47250-110">Delegated (work or school account)</span></span> | <span data-ttu-id="47250-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47250-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="47250-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47250-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47250-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47250-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="47250-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47250-114">Application</span></span> | <span data-ttu-id="47250-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47250-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="47250-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47250-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskFolders/{id}
DELETE /me/outlook/taskGroups/{id}/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="47250-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47250-117">Request headers</span></span>
| <span data-ttu-id="47250-118">Имя</span><span class="sxs-lookup"><span data-stu-id="47250-118">Name</span></span>       | <span data-ttu-id="47250-119">Описание</span><span class="sxs-lookup"><span data-stu-id="47250-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="47250-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47250-120">Authorization</span></span>  | <span data-ttu-id="47250-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47250-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47250-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="47250-123">Request body</span></span>
<span data-ttu-id="47250-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47250-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47250-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="47250-125">Response</span></span>

<span data-ttu-id="47250-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="47250-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47250-128">Пример</span><span class="sxs-lookup"><span data-stu-id="47250-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47250-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="47250-129">Request</span></span>
<span data-ttu-id="47250-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47250-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="47250-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="47250-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPXAAA=
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="47250-132">C#</span><span class="sxs-lookup"><span data-stu-id="47250-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="47250-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="47250-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="47250-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="47250-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="47250-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="47250-135">Response</span></span>
<span data-ttu-id="47250-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="47250-136">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete outlookTaskFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
