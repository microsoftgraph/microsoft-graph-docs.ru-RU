---
title: Удаление outlookTaskFolder
description: Удаление указанной папки задач Outlook.
author: mashriv
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 7738f51788f417284db5bb11f72a2dc845f76e83
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43403212"
---
# <a name="delete-outlooktaskfolder"></a><span data-ttu-id="9c0cc-103">Удаление outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="9c0cc-103">Delete outlookTaskFolder</span></span>

<span data-ttu-id="9c0cc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c0cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c0cc-105">Удаление указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="9c0cc-105">Delete the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="9c0cc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c0cc-106">Permissions</span></span>
<span data-ttu-id="9c0cc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c0cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c0cc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c0cc-109">Permission type</span></span>      | <span data-ttu-id="9c0cc-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c0cc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c0cc-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c0cc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9c0cc-112">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c0cc-112">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="9c0cc-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c0cc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c0cc-114">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c0cc-114">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="9c0cc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c0cc-115">Application</span></span> | <span data-ttu-id="9c0cc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c0cc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c0cc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c0cc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskFolders/{id}
DELETE /me/outlook/taskGroups/{id}/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9c0cc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c0cc-118">Request headers</span></span>
| <span data-ttu-id="9c0cc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="9c0cc-119">Name</span></span>       | <span data-ttu-id="9c0cc-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9c0cc-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9c0cc-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9c0cc-121">Authorization</span></span>  | <span data-ttu-id="9c0cc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c0cc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c0cc-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c0cc-124">Request body</span></span>
<span data-ttu-id="9c0cc-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9c0cc-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c0cc-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="9c0cc-126">Response</span></span>

<span data-ttu-id="9c0cc-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9c0cc-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c0cc-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9c0cc-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c0cc-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c0cc-130">Request</span></span>
<span data-ttu-id="9c0cc-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c0cc-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9c0cc-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c0cc-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPXAAA=
```
# <a name="c"></a>[<span data-ttu-id="9c0cc-133">C#</span><span class="sxs-lookup"><span data-stu-id="9c0cc-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-outlooktaskfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c0cc-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c0cc-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-outlooktaskfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c0cc-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c0cc-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-outlooktaskfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9c0cc-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c0cc-136">Response</span></span>
<span data-ttu-id="9c0cc-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9c0cc-137">Here is an example of the response.</span></span> 
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
