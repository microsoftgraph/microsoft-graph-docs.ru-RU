---
title: 'group: unsubscribeByMail'
description: 'При вызове этого метода приведет к отключению текущего пользователя, чтобы получать уведомления по электронной почте для данной группы о новых сообщений, события и файлы в эту группу. Поддерживается только в Office 365 группы. '
ms.openlocfilehash: 4891b3c4f8908c61cdbc46ce8bc43f9e51cc4e16
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077269"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="e6c44-104">group: unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="e6c44-104">group: unsubscribeByMail</span></span>

> <span data-ttu-id="e6c44-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e6c44-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6c44-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6c44-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e6c44-107">При вызове этого метода приведет к отключению текущего пользователя, чтобы получать уведомления по электронной почте для данной группы о новых сообщений, события и файлы в эту группу.</span><span class="sxs-lookup"><span data-stu-id="e6c44-107">Calling this method will disable the current user to receive email notifications for this group about new posts, events, and files in that group.</span></span> <span data-ttu-id="e6c44-108">Поддерживается только в Office 365 группы.</span><span class="sxs-lookup"><span data-stu-id="e6c44-108">Supported for Office 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="e6c44-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e6c44-109">Permissions</span></span>
<span data-ttu-id="e6c44-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e6c44-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6c44-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e6c44-112">Permission type</span></span>      | <span data-ttu-id="e6c44-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e6c44-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6c44-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e6c44-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e6c44-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6c44-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e6c44-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e6c44-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6c44-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e6c44-117">Not supported.</span></span>    |
|<span data-ttu-id="e6c44-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e6c44-118">Application</span></span> | <span data-ttu-id="e6c44-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6c44-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6c44-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e6c44-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```

## <a name="request-headers"></a><span data-ttu-id="e6c44-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e6c44-121">Request headers</span></span>
| <span data-ttu-id="e6c44-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e6c44-122">Header</span></span>       | <span data-ttu-id="e6c44-123">Значение</span><span class="sxs-lookup"><span data-stu-id="e6c44-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e6c44-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e6c44-124">Authorization</span></span>  | <span data-ttu-id="e6c44-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6c44-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e6c44-127">Prefer</span><span class="sxs-lookup"><span data-stu-id="e6c44-127">Prefer</span></span> | <span data-ttu-id="e6c44-128">return=minimal.</span><span class="sxs-lookup"><span data-stu-id="e6c44-128">return=minimal.</span></span> <span data-ttu-id="e6c44-129">Если заголовок минимального отклика включен в заголовок запроса, то в отклике об успешном выполнении возвращается код `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e6c44-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="e6c44-130">Необязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="e6c44-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="e6c44-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e6c44-131">Request body</span></span>
 <span data-ttu-id="e6c44-132">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e6c44-132">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="e6c44-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="e6c44-133">Response</span></span>
<span data-ttu-id="e6c44-p107">В случае успешного выполнения этот метод возвращает код отклика `200 OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="e6c44-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6c44-136">Пример</span><span class="sxs-lookup"><span data-stu-id="e6c44-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e6c44-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="e6c44-137">Request</span></span>
<span data-ttu-id="e6c44-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e6c44-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/unsubscribeByMail
```

#### <a name="response"></a><span data-ttu-id="e6c44-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="e6c44-139">Response</span></span>
<span data-ttu-id="e6c44-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e6c44-140">The following is an example of the response.</span></span> 
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
  "description": "group: unsubscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->