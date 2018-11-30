---
title: Удаление события
description: Удаление объекта event.
ms.openlocfilehash: 41623ad938a37ba762e843ab007f772ac8ae7504
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081431"
---
# <a name="delete-event"></a><span data-ttu-id="a6c89-103">Удаление события</span><span class="sxs-lookup"><span data-stu-id="a6c89-103">Delete event</span></span>

> <span data-ttu-id="a6c89-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a6c89-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6c89-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6c89-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6c89-106">Удаление объекта [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="a6c89-106">Delete an [event](../resources/event.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6c89-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6c89-107">Permissions</span></span>
<span data-ttu-id="a6c89-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6c89-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6c89-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6c89-110">Permission type</span></span>      | <span data-ttu-id="a6c89-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6c89-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6c89-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6c89-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a6c89-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6c89-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a6c89-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6c89-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6c89-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6c89-115">Not supported.</span></span>    |
|<span data-ttu-id="a6c89-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6c89-116">Application</span></span> | <span data-ttu-id="a6c89-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6c89-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6c89-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6c89-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/events/{id}
DELETE /groups/{id}/calendar/events/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a6c89-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6c89-119">Request headers</span></span>
| <span data-ttu-id="a6c89-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a6c89-120">Name</span></span>       | <span data-ttu-id="a6c89-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a6c89-121">Type</span></span> | <span data-ttu-id="a6c89-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a6c89-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a6c89-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6c89-123">Authorization</span></span>  | <span data-ttu-id="a6c89-124">string</span><span class="sxs-lookup"><span data-stu-id="a6c89-124">string</span></span>  | <span data-ttu-id="a6c89-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6c89-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6c89-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6c89-127">Request body</span></span>
<span data-ttu-id="a6c89-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a6c89-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6c89-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6c89-129">Response</span></span>
<span data-ttu-id="a6c89-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a6c89-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6c89-132">Пример</span><span class="sxs-lookup"><span data-stu-id="a6c89-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a6c89-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6c89-133">Request</span></span>
<span data-ttu-id="a6c89-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a6c89-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_group_event"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/events/AQMkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NwAzZWYARgAAA_b2VnUAiWNLj0xeSOs499YHAMT2RdsuOqRIlQZ4vOzp66YAAAIBDQAAAMT2RdsuOqRIlQZ4vOzp66YAAAIJOgAAAA==
```

#### <a name="response"></a><span data-ttu-id="a6c89-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="a6c89-135">Response</span></span>
<span data-ttu-id="a6c89-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a6c89-136">The following is an example of the response.</span></span> 
><span data-ttu-id="a6c89-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a6c89-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Delete event",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->