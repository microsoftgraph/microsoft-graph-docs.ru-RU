---
title: Удаление объекта rejectedSender
description: Удаление пользователя или группы из списка rejectedSenders.
ms.openlocfilehash: a78a81c229e18c91e3c314ffd04816fe1505c247
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078191"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="d7d01-103">Удаление объекта rejectedSender</span><span class="sxs-lookup"><span data-stu-id="d7d01-103">Remove rejectedSender</span></span>

> <span data-ttu-id="d7d01-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d7d01-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7d01-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7d01-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d7d01-106">Удаление пользователя или группы из списка rejectedSenders.</span><span class="sxs-lookup"><span data-stu-id="d7d01-106">Remove a user or group from the rejectedSenders list.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7d01-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7d01-107">Permissions</span></span>
<span data-ttu-id="d7d01-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7d01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d7d01-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7d01-110">Permission type</span></span>                        | <span data-ttu-id="d7d01-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7d01-111">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="d7d01-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7d01-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d7d01-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7d01-113">Group.ReadWrite.All</span></span>  |  
| <span data-ttu-id="d7d01-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7d01-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7d01-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7d01-115">Not supported.</span></span> |
| <span data-ttu-id="d7d01-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7d01-116">Application</span></span>                            | <span data-ttu-id="d7d01-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7d01-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7d01-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7d01-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id=<id>
```

## <a name="request-headers"></a><span data-ttu-id="d7d01-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7d01-119">Request headers</span></span>

| <span data-ttu-id="d7d01-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d7d01-120">Header</span></span>         | <span data-ttu-id="d7d01-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d7d01-121">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="d7d01-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7d01-122">Authorization</span></span>  | <span data-ttu-id="d7d01-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7d01-p103">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="d7d01-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7d01-125">Request body</span></span>
<span data-ttu-id="d7d01-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d7d01-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7d01-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7d01-127">Response</span></span>
<span data-ttu-id="d7d01-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="d7d01-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7d01-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d7d01-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="d7d01-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7d01-131">Request</span></span>
<span data-ttu-id="d7d01-132">Ниже представлено несколько примеров запроса.</span><span class="sxs-lookup"><span data-stu-id="d7d01-132">The following are a couple of examples of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "remove_rejectedSender_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{id}

DELETE https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{id}
```

#### <a name="response"></a><span data-ttu-id="d7d01-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="d7d01-133">Response</span></span>
<span data-ttu-id="d7d01-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d7d01-134">The following is an example of the response.</span></span> 
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
  "description": "Remove rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->