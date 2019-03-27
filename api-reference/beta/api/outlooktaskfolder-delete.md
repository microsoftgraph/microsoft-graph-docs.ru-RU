---
title: Удаление outlookTaskFolder
description: Удаление указанной папки задач Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 4c526c937f7d92b6e2b0482193f6c0327f4870c1
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/27/2019
ms.locfileid: "30869388"
---
# <a name="delete-outlooktaskfolder"></a><span data-ttu-id="47129-103">Удаление outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="47129-103">Delete outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47129-104">Удаление указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="47129-104">Delete the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="47129-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47129-105">Permissions</span></span>
<span data-ttu-id="47129-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47129-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47129-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47129-108">Permission type</span></span>      | <span data-ttu-id="47129-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47129-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47129-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47129-110">Delegated (work or school account)</span></span> | <span data-ttu-id="47129-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47129-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="47129-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47129-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47129-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="47129-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="47129-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47129-114">Application</span></span> | <span data-ttu-id="47129-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47129-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="47129-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47129-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/outlook/taskFolders/{id}
DELETE /me/outlook/taskGroups/{id}/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="47129-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47129-117">Request headers</span></span>
| <span data-ttu-id="47129-118">Имя</span><span class="sxs-lookup"><span data-stu-id="47129-118">Name</span></span>       | <span data-ttu-id="47129-119">Описание</span><span class="sxs-lookup"><span data-stu-id="47129-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="47129-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47129-120">Authorization</span></span>  | <span data-ttu-id="47129-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47129-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="47129-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47129-123">Request body</span></span>
<span data-ttu-id="47129-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47129-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47129-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="47129-125">Response</span></span>

<span data-ttu-id="47129-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="47129-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47129-128">Пример</span><span class="sxs-lookup"><span data-stu-id="47129-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47129-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="47129-129">Request</span></span>
<span data-ttu-id="47129-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47129-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskFolders('AAMkADIyAAAhrbPXAAA=')
```
##### <a name="response"></a><span data-ttu-id="47129-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="47129-131">Response</span></span>
<span data-ttu-id="47129-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="47129-132">Here is an example of the response.</span></span> 
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
    "Error: /api-reference/beta/api/outlooktaskfolder-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
