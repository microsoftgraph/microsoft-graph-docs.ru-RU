---
title: 'group: resetUnseenCount'
description: Сброс unseenCount все сообщения, которые текущий пользователь не с момента их последнего посетить. Поддерживается только в Office 365 группы.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 29102945e5a549db737cc94453ea4114b82a4dde
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853895"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="eb84c-104">group: resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="eb84c-104">group: resetUnseenCount</span></span>

> <span data-ttu-id="eb84c-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eb84c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb84c-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb84c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eb84c-107">Сброс unseenCount все сообщения, которые текущий пользователь не с момента их последнего посетить.</span><span class="sxs-lookup"><span data-stu-id="eb84c-107">Reset the unseenCount of all the posts that the current user has not seen since their last visit.</span></span> <span data-ttu-id="eb84c-108">Поддерживается только в Office 365 группы.</span><span class="sxs-lookup"><span data-stu-id="eb84c-108">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="eb84c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="eb84c-109">Permissions</span></span>
<span data-ttu-id="eb84c-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb84c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb84c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="eb84c-112">Permission type</span></span>      | <span data-ttu-id="eb84c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="eb84c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb84c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="eb84c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="eb84c-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb84c-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="eb84c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="eb84c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb84c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb84c-117">Not supported.</span></span>    |
|<span data-ttu-id="eb84c-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="eb84c-118">Application</span></span> | <span data-ttu-id="eb84c-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eb84c-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb84c-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="eb84c-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="eb84c-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="eb84c-121">Request headers</span></span>
| <span data-ttu-id="eb84c-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="eb84c-122">Header</span></span>       | <span data-ttu-id="eb84c-123">Значение</span><span class="sxs-lookup"><span data-stu-id="eb84c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eb84c-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="eb84c-124">Authorization</span></span>  | <span data-ttu-id="eb84c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="eb84c-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eb84c-127">Prefer</span><span class="sxs-lookup"><span data-stu-id="eb84c-127">Prefer</span></span> | <span data-ttu-id="eb84c-128">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="eb84c-128">return=minimal.</span></span> <span data-ttu-id="eb84c-129">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="eb84c-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="eb84c-130">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="eb84c-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="eb84c-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="eb84c-131">Request body</span></span>
<span data-ttu-id="eb84c-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="eb84c-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb84c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="eb84c-133">Response</span></span>
<span data-ttu-id="eb84c-p107">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="eb84c-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb84c-136">Пример</span><span class="sxs-lookup"><span data-stu-id="eb84c-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="eb84c-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="eb84c-137">Request</span></span>
<span data-ttu-id="eb84c-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="eb84c-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/resetUnseenCount
```

#### <a name="response"></a><span data-ttu-id="eb84c-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="eb84c-139">Response</span></span>
<span data-ttu-id="eb84c-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="eb84c-140">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
