---
title: Удаление outlookTaskGroup
description: Удаление указанного outlookTaskGroup.
author: angelgolfer-ms
ms.openlocfilehash: e2494823db2415afda2d6b5060c1a34e2d78d131
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319476"
---
# <a name="delete-outlooktaskgroup"></a><span data-ttu-id="db1e0-103">Удаление outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="db1e0-103">Delete outlookTaskGroup</span></span>

> <span data-ttu-id="db1e0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="db1e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db1e0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db1e0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="db1e0-106">Удаление указанного [outlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="db1e0-106">Delete the specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="db1e0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db1e0-107">Permissions</span></span>
<span data-ttu-id="db1e0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db1e0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db1e0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db1e0-110">Permission type</span></span>      | <span data-ttu-id="db1e0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db1e0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db1e0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db1e0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="db1e0-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db1e0-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="db1e0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db1e0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db1e0-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="db1e0-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="db1e0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="db1e0-116">Application</span></span> | <span data-ttu-id="db1e0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db1e0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="db1e0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db1e0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}

```
## <a name="request-headers"></a><span data-ttu-id="db1e0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db1e0-119">Request headers</span></span>
| <span data-ttu-id="db1e0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="db1e0-120">Name</span></span>       | <span data-ttu-id="db1e0-121">Описание</span><span class="sxs-lookup"><span data-stu-id="db1e0-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="db1e0-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db1e0-122">Authorization</span></span>  | <span data-ttu-id="db1e0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db1e0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="db1e0-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="db1e0-125">Request body</span></span>
<span data-ttu-id="db1e0-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="db1e0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db1e0-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="db1e0-127">Response</span></span>

<span data-ttu-id="db1e0-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="db1e0-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db1e0-130">Пример</span><span class="sxs-lookup"><span data-stu-id="db1e0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="db1e0-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="db1e0-131">Request</span></span>
<span data-ttu-id="db1e0-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="db1e0-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskgroups('AAMkADIyAAAhrbe-AAA=')
```
##### <a name="response"></a><span data-ttu-id="db1e0-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="db1e0-133">Response</span></span>
<span data-ttu-id="db1e0-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="db1e0-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->