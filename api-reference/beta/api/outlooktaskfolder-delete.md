---
title: Удаление outlookTaskFolder
description: Удаление указанной папки задач Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 67b5898c29911724639b6de1556e6d4563840227
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33596338"
---
# <a name="delete-outlooktaskfolder"></a><span data-ttu-id="56453-103">Удаление outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="56453-103">Delete outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56453-104">Удаление указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="56453-104">Delete the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="56453-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56453-105">Permissions</span></span>
<span data-ttu-id="56453-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56453-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56453-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56453-108">Permission type</span></span>      | <span data-ttu-id="56453-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56453-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56453-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56453-110">Delegated (work or school account)</span></span> | <span data-ttu-id="56453-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56453-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="56453-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56453-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56453-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="56453-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="56453-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56453-114">Application</span></span> | <span data-ttu-id="56453-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56453-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="56453-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56453-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskFolders/{id}
DELETE /me/outlook/taskGroups/{id}/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="56453-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56453-117">Request headers</span></span>
| <span data-ttu-id="56453-118">Имя</span><span class="sxs-lookup"><span data-stu-id="56453-118">Name</span></span>       | <span data-ttu-id="56453-119">Описание</span><span class="sxs-lookup"><span data-stu-id="56453-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="56453-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56453-120">Authorization</span></span>  | <span data-ttu-id="56453-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56453-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56453-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="56453-123">Request body</span></span>
<span data-ttu-id="56453-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="56453-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56453-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="56453-125">Response</span></span>

<span data-ttu-id="56453-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="56453-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56453-128">Пример</span><span class="sxs-lookup"><span data-stu-id="56453-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56453-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="56453-129">Request</span></span>
<span data-ttu-id="56453-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56453-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskFolders/AAMkADIyAAAhrbPXAAA=
```
##### <a name="response"></a><span data-ttu-id="56453-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="56453-131">Response</span></span>
<span data-ttu-id="56453-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="56453-132">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="56453-133">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="56453-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="56453-134">Языках</span><span class="sxs-lookup"><span data-stu-id="56453-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_outlooktaskfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="56453-135">Язык</span><span class="sxs-lookup"><span data-stu-id="56453-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_outlooktaskfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/outlooktaskfolder-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlooktaskfolder-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
