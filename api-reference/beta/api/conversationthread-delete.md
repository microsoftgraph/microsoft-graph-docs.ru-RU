---
title: Удаление объекта conversationThread
description: Удаление объекта conversationThread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: e455467c7c9e4a89c3c6293231d5371251191f69
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956516"
---
# <a name="delete-conversationthread"></a><span data-ttu-id="98864-103">Удаление объекта conversationThread</span><span class="sxs-lookup"><span data-stu-id="98864-103">Delete conversationThread</span></span>

> <span data-ttu-id="98864-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="98864-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="98864-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98864-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="98864-106">Удаление объекта conversationThread.</span><span class="sxs-lookup"><span data-stu-id="98864-106">Delete conversationThread.</span></span>
## <a name="permissions"></a><span data-ttu-id="98864-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="98864-107">Permissions</span></span>
<span data-ttu-id="98864-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="98864-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98864-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="98864-110">Permission type</span></span>      | <span data-ttu-id="98864-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="98864-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98864-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="98864-112">Delegated (work or school account)</span></span> | <span data-ttu-id="98864-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98864-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="98864-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="98864-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="98864-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="98864-115">Not supported.</span></span>    |
|<span data-ttu-id="98864-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="98864-116">Application</span></span> | <span data-ttu-id="98864-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="98864-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="98864-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="98864-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
DELETE /groups/{id}/conversations/{id}/threads/{id}

```
## <a name="request-headers"></a><span data-ttu-id="98864-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="98864-119">Request headers</span></span>
| <span data-ttu-id="98864-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="98864-120">Header</span></span>       | <span data-ttu-id="98864-121">Значение</span><span class="sxs-lookup"><span data-stu-id="98864-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="98864-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="98864-122">Authorization</span></span>  | <span data-ttu-id="98864-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="98864-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="98864-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="98864-125">Request body</span></span>
<span data-ttu-id="98864-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="98864-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="98864-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="98864-127">Response</span></span>

<span data-ttu-id="98864-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="98864-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="98864-130">Пример</span><span class="sxs-lookup"><span data-stu-id="98864-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="98864-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="98864-131">Request</span></span>
<span data-ttu-id="98864-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="98864-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_conversationthread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/threads/{id}
```
##### <a name="response"></a><span data-ttu-id="98864-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="98864-133">Response</span></span>
<span data-ttu-id="98864-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="98864-134">Here is an example of the response.</span></span> 
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
  "description": "Delete conversationThread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
