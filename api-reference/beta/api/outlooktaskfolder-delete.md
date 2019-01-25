---
title: Удаление outlookTaskFolder
description: Удаление указанной папки задач Outlook.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 0ad240cb28fc17204bbad7a608b79d457ca763cf
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515876"
---
# <a name="delete-outlooktaskfolder"></a><span data-ttu-id="dc485-103">Удаление outlookTaskFolder</span><span class="sxs-lookup"><span data-stu-id="dc485-103">Delete outlookTaskFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc485-104">Удаление указанной папки задач Outlook.</span><span class="sxs-lookup"><span data-stu-id="dc485-104">Delete the specified Outlook task folder.</span></span>
## <a name="permissions"></a><span data-ttu-id="dc485-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc485-105">Permissions</span></span>
<span data-ttu-id="dc485-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc485-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc485-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc485-108">Permission type</span></span>      | <span data-ttu-id="dc485-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc485-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc485-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc485-110">Delegated (work or school account)</span></span> | <span data-ttu-id="dc485-111">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc485-111">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="dc485-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc485-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc485-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="dc485-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="dc485-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc485-114">Application</span></span> | <span data-ttu-id="dc485-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc485-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc485-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc485-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id|userPrincipalName}/outlook/taskFolders/{id}
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}/taskFolders/{id}

```
## <a name="request-headers"></a><span data-ttu-id="dc485-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc485-117">Request headers</span></span>
| <span data-ttu-id="dc485-118">Имя</span><span class="sxs-lookup"><span data-stu-id="dc485-118">Name</span></span>       | <span data-ttu-id="dc485-119">Описание</span><span class="sxs-lookup"><span data-stu-id="dc485-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dc485-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dc485-120">Authorization</span></span>  | <span data-ttu-id="dc485-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dc485-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dc485-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc485-123">Request body</span></span>
<span data-ttu-id="dc485-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dc485-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc485-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc485-125">Response</span></span>

<span data-ttu-id="dc485-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="dc485-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc485-128">Пример</span><span class="sxs-lookup"><span data-stu-id="dc485-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dc485-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc485-129">Request</span></span>
<span data-ttu-id="dc485-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc485-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskFolders('AAMkADIyAAAhrbPXAAA=')
```
##### <a name="response"></a><span data-ttu-id="dc485-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="dc485-131">Response</span></span>
<span data-ttu-id="dc485-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dc485-132">Here is an example of the response.</span></span> 
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
