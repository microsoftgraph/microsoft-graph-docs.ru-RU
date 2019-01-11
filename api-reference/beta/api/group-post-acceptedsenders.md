---
title: Создание объекта acceptedSender
description: Добавление пользователя или группы в список объектов acceptedSender.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: d450d7441429f6e40477570609a9b9689ebc0a28
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843465"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="b7d18-103">Создание объекта acceptedSender</span><span class="sxs-lookup"><span data-stu-id="b7d18-103">Create acceptedSender</span></span>

> <span data-ttu-id="b7d18-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b7d18-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b7d18-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7d18-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b7d18-106">Добавление пользователя или группы в список объектов acceptedSender.</span><span class="sxs-lookup"><span data-stu-id="b7d18-106">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="b7d18-p102">Укажите пользователя или группу с помощью параметра `@odata.id` в тексте запроса. Пользователи из списка разрешенных отправителей могут отправлять записи в беседы группы. Убедитесь, что в списках разрешенных и запрещенных отправителей не указаны одни и те же пользователи или группы. В противном случае возникнет ошибка.</span><span class="sxs-lookup"><span data-stu-id="b7d18-p102">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="b7d18-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7d18-110">Permissions</span></span>
<span data-ttu-id="b7d18-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7d18-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7d18-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7d18-113">Permission type</span></span>      | <span data-ttu-id="b7d18-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7d18-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7d18-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7d18-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b7d18-116">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7d18-116">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b7d18-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7d18-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7d18-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7d18-118">Not supported.</span></span>    |
|<span data-ttu-id="b7d18-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7d18-119">Application</span></span> | <span data-ttu-id="b7d18-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7d18-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b7d18-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7d18-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="b7d18-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7d18-122">Request headers</span></span>
| <span data-ttu-id="b7d18-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b7d18-123">Header</span></span>       | <span data-ttu-id="b7d18-124">Значение</span><span class="sxs-lookup"><span data-stu-id="b7d18-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b7d18-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7d18-125">Authorization</span></span>  | <span data-ttu-id="b7d18-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b7d18-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b7d18-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7d18-128">Request body</span></span>
<span data-ttu-id="b7d18-129">Укажите в тексте запроса идентификатор объекта user или group.</span><span class="sxs-lookup"><span data-stu-id="b7d18-129">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="b7d18-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7d18-130">Response</span></span>
<span data-ttu-id="b7d18-131">Этот метод возвращает код отклика `204 No Content`, но не возвращает текст отклика.</span><span class="sxs-lookup"><span data-stu-id="b7d18-131">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7d18-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b7d18-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b7d18-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7d18-133">Request</span></span>
<span data-ttu-id="b7d18-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7d18-134">The following is an example of the request.</span></span>
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

#### <a name="response"></a><span data-ttu-id="b7d18-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="b7d18-135">Response</span></span>
<span data-ttu-id="b7d18-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b7d18-136">The following is an example of the response.</span></span>
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
