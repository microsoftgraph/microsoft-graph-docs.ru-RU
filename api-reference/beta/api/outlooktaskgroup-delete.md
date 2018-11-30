---
title: Удаление outlookTaskGroup
description: Удаление указанного outlookTaskGroup.
ms.openlocfilehash: c700b104db6c89d9b762ca7d6f7dc571d430878d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081236"
---
# <a name="delete-outlooktaskgroup"></a><span data-ttu-id="a7892-103">Удаление outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="a7892-103">Delete outlookTaskGroup</span></span>

> <span data-ttu-id="a7892-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a7892-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7892-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7892-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a7892-106">Удаление указанного [outlookTaskGroup](../resources/outlooktaskgroup.md).</span><span class="sxs-lookup"><span data-stu-id="a7892-106">Delete the specified [outlookTaskGroup](../resources/outlooktaskgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="a7892-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7892-107">Permissions</span></span>
<span data-ttu-id="a7892-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7892-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7892-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7892-110">Permission type</span></span>      | <span data-ttu-id="a7892-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7892-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7892-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7892-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a7892-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7892-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a7892-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7892-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7892-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7892-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="a7892-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7892-116">Application</span></span> | <span data-ttu-id="a7892-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a7892-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7892-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7892-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /users/{id|userPrincipalName}/outlook/taskGroups/{id}

```
## <a name="request-headers"></a><span data-ttu-id="a7892-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7892-119">Request headers</span></span>
| <span data-ttu-id="a7892-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a7892-120">Name</span></span>       | <span data-ttu-id="a7892-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a7892-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a7892-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7892-122">Authorization</span></span>  | <span data-ttu-id="a7892-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7892-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7892-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7892-125">Request body</span></span>
<span data-ttu-id="a7892-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a7892-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7892-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7892-127">Response</span></span>

<span data-ttu-id="a7892-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a7892-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7892-130">Пример</span><span class="sxs-lookup"><span data-stu-id="a7892-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7892-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7892-131">Request</span></span>
<span data-ttu-id="a7892-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7892-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_outlooktaskgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/outlook/taskgroups('AAMkADIyAAAhrbe-AAA=')
```
##### <a name="response"></a><span data-ttu-id="a7892-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="a7892-133">Response</span></span>
<span data-ttu-id="a7892-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a7892-134">Here is an example of the response.</span></span>
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