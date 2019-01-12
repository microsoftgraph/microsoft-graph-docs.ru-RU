---
title: Создание объекта rejectedSender
description: Добавление пользователя или группы в список объектов rejectedSender.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 20a9cfbadfef5febbca90ed77230fbbc5e515ef7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984691"
---
# <a name="create-rejectedsender"></a><span data-ttu-id="c4e10-103">Создание объекта rejectedSender</span><span class="sxs-lookup"><span data-stu-id="c4e10-103">Create rejectedSender</span></span>

> <span data-ttu-id="c4e10-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c4e10-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c4e10-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4e10-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c4e10-106">Добавление пользователя или группы в список объектов rejectedSender.</span><span class="sxs-lookup"><span data-stu-id="c4e10-106">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="c4e10-p102">Укажите пользователя или группу с помощью параметра `@odata.id` в тексте запроса. Пользователи из списка запрещенных отправителей не могут отправлять записи в беседы группы (определенные в URL-адресе запроса POST). Убедитесь, что в списках запрещенных и разрешенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="c4e10-p102">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4e10-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c4e10-110">Permissions</span></span>
<span data-ttu-id="c4e10-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c4e10-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c4e10-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c4e10-113">Permission type</span></span>      | <span data-ttu-id="c4e10-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c4e10-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4e10-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c4e10-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c4e10-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4e10-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="c4e10-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c4e10-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4e10-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4e10-118">Not supported.</span></span>    |
|<span data-ttu-id="c4e10-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c4e10-119">Application</span></span> | <span data-ttu-id="c4e10-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c4e10-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4e10-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c4e10-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="c4e10-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c4e10-122">Request headers</span></span>
| <span data-ttu-id="c4e10-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c4e10-123">Header</span></span>       | <span data-ttu-id="c4e10-124">Значение</span><span class="sxs-lookup"><span data-stu-id="c4e10-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c4e10-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c4e10-125">Authorization</span></span>  | <span data-ttu-id="c4e10-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c4e10-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c4e10-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c4e10-128">Request body</span></span>
<span data-ttu-id="c4e10-129">Укажите в тексте запроса идентификатор объекта user или group.</span><span class="sxs-lookup"><span data-stu-id="c4e10-129">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="c4e10-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="c4e10-130">Response</span></span>
<span data-ttu-id="c4e10-131">Этот метод возвращает код отклика `204 No Content`, но не возвращает текст отклика.</span><span class="sxs-lookup"><span data-stu-id="c4e10-131">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4e10-132">Пример</span><span class="sxs-lookup"><span data-stu-id="c4e10-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="c4e10-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="c4e10-133">Request</span></span>
<span data-ttu-id="c4e10-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c4e10-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rejectedsender"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/beta/users/alexd@contoso.com"
}
```

#### <a name="response"></a><span data-ttu-id="c4e10-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="c4e10-135">Response</span></span>
<span data-ttu-id="c4e10-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c4e10-136">The following is an example of the response.</span></span>
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
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
