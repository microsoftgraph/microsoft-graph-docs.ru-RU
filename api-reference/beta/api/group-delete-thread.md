---
title: Удаление цепочки беседы
description: Удаление объекта thread.
author: dkershaw10
ms.openlocfilehash: eec28f92fcdee1755b1e000225ea9458241f01c6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352950"
---
# <a name="delete-conversation-thread"></a><span data-ttu-id="6967e-103">Удаление цепочки беседы</span><span class="sxs-lookup"><span data-stu-id="6967e-103">Delete conversation thread</span></span>

> <span data-ttu-id="6967e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6967e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6967e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6967e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6967e-106">Удаление объекта [thread](../resources/conversationthread.md).</span><span class="sxs-lookup"><span data-stu-id="6967e-106">Delete a [thread](../resources/conversationthread.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6967e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6967e-107">Permissions</span></span>
<span data-ttu-id="6967e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6967e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6967e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6967e-110">Permission type</span></span>      | <span data-ttu-id="6967e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6967e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6967e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6967e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6967e-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6967e-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6967e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6967e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6967e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6967e-115">Not supported.</span></span>    |
|<span data-ttu-id="6967e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6967e-116">Application</span></span> | <span data-ttu-id="6967e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6967e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6967e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6967e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/threads/{id}
```

## <a name="request-headers"></a><span data-ttu-id="6967e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6967e-119">Request headers</span></span>
| <span data-ttu-id="6967e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="6967e-120">Name</span></span>       | <span data-ttu-id="6967e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="6967e-121">Type</span></span> | <span data-ttu-id="6967e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="6967e-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6967e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6967e-123">Authorization</span></span>  | <span data-ttu-id="6967e-124">string</span><span class="sxs-lookup"><span data-stu-id="6967e-124">string</span></span>  | <span data-ttu-id="6967e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6967e-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6967e-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6967e-127">Request body</span></span>
<span data-ttu-id="6967e-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="6967e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6967e-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="6967e-129">Response</span></span>
<span data-ttu-id="6967e-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="6967e-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6967e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="6967e-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="6967e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="6967e-133">Request</span></span>
<span data-ttu-id="6967e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6967e-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_thread"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==
```

#### <a name="response"></a><span data-ttu-id="6967e-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="6967e-135">Response</span></span>
<span data-ttu-id="6967e-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6967e-136">The following is an example of the response.</span></span> 
><span data-ttu-id="6967e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6967e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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