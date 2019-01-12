---
title: Удаление цепочки беседы
description: Удаление объекта thread.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f4e40763a1221575fbe45e8294aad0d2e0bdf764
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935789"
---
# <a name="delete-conversation-thread"></a><span data-ttu-id="538c0-103">Удаление цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="538c0-103">Delete conversation thread</span></span>

> <span data-ttu-id="538c0-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="538c0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="538c0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="538c0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="538c0-106">Удаление объекта [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="538c0-106">Delete a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="538c0-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="538c0-107">Permissions</span></span>
<span data-ttu-id="538c0-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="538c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="538c0-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="538c0-110">Permission type</span></span>      | <span data-ttu-id="538c0-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="538c0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="538c0-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="538c0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="538c0-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="538c0-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="538c0-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="538c0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="538c0-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="538c0-115">Not supported.</span></span>    |
|<span data-ttu-id="538c0-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="538c0-116">Application</span></span> | <span data-ttu-id="538c0-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="538c0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="538c0-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="538c0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="538c0-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="538c0-119">Request headers</span></span>
| <span data-ttu-id="538c0-120">Имя</span><span class="sxs-lookup"><span data-stu-id="538c0-120">Name</span></span>       | <span data-ttu-id="538c0-121">Тип</span><span class="sxs-lookup"><span data-stu-id="538c0-121">Type</span></span> | <span data-ttu-id="538c0-122">Описание</span><span class="sxs-lookup"><span data-stu-id="538c0-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="538c0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="538c0-123">Authorization</span></span>  | <span data-ttu-id="538c0-124">строка</span><span class="sxs-lookup"><span data-stu-id="538c0-124">string</span></span>  | <span data-ttu-id="538c0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="538c0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="538c0-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="538c0-127">Request body</span></span>
<span data-ttu-id="538c0-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="538c0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="538c0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="538c0-129">Response</span></span>
<span data-ttu-id="538c0-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="538c0-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="538c0-132">Пример</span><span class="sxs-lookup"><span data-stu-id="538c0-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="538c0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="538c0-133">Request</span></span>
<span data-ttu-id="538c0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="538c0-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_thread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="538c0-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="538c0-135">Response</span></span>
<span data-ttu-id="538c0-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="538c0-136">The following is an example of the response.</span></span> 
><span data-ttu-id="538c0-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="538c0-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete conversation thread",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
