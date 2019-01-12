---
title: Создание объекта acceptedSender
description: Добавление пользователя или группы в список объектов acceptedSender.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 650e0902b7968cd920e4148fddd0fd627e138b4c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955564"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="d74e6-103">Создание объекта acceptedSender</span><span class="sxs-lookup"><span data-stu-id="d74e6-103">Create acceptedSender</span></span>

> <span data-ttu-id="d74e6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d74e6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d74e6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d74e6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d74e6-106">Добавление пользователя или группы в список объектов acceptedSender.</span><span class="sxs-lookup"><span data-stu-id="d74e6-106">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="d74e6-p102">Укажите пользователя или группу с помощью параметра `@odata.id` в тексте запроса. Пользователи из списка разрешенных отправителей могут отправлять записи в беседы группы. Убедитесь, что в списках разрешенных и запрещенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="d74e6-p102">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="d74e6-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d74e6-110">Permissions</span></span>
<span data-ttu-id="d74e6-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d74e6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d74e6-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d74e6-113">Permission type</span></span>      | <span data-ttu-id="d74e6-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d74e6-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d74e6-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d74e6-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d74e6-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d74e6-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d74e6-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d74e6-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d74e6-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d74e6-118">Not supported.</span></span>    |
|<span data-ttu-id="d74e6-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d74e6-119">Application</span></span> | <span data-ttu-id="d74e6-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d74e6-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d74e6-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d74e6-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="d74e6-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d74e6-122">Request headers</span></span>
| <span data-ttu-id="d74e6-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d74e6-123">Header</span></span>       | <span data-ttu-id="d74e6-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d74e6-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d74e6-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d74e6-125">Authorization</span></span>  | <span data-ttu-id="d74e6-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d74e6-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d74e6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d74e6-128">Request body</span></span>
<span data-ttu-id="d74e6-129">Укажите в тексте запроса идентификатор объекта user или group.</span><span class="sxs-lookup"><span data-stu-id="d74e6-129">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="d74e6-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d74e6-130">Response</span></span>
<span data-ttu-id="d74e6-131">Этот метод возвращает код отклика `204 No Content`, но не возвращает текст отклика.</span><span class="sxs-lookup"><span data-stu-id="d74e6-131">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="d74e6-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d74e6-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d74e6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d74e6-133">Request</span></span>
<span data-ttu-id="d74e6-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d74e6-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_acceptedsender"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/beta/users/alexd@contoso.com"
}
```

#### <a name="response"></a><span data-ttu-id="d74e6-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="d74e6-135">Response</span></span>
<span data-ttu-id="d74e6-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d74e6-136">The following is an example of the response.</span></span>
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
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
