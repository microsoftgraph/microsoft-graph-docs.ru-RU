---
title: Удаление объекта rejectedSender
description: Удаление пользователя или группы из списка rejectedSenders.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 58936ee410b63f43d9c0a9e8efcf3eb5a96e76ae
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957475"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="bcfd5-103">Удаление объекта rejectedSender</span><span class="sxs-lookup"><span data-stu-id="bcfd5-103">Remove rejectedSender</span></span>
<span data-ttu-id="bcfd5-104">Удаление пользователя или группы из списка rejectedSenders.</span><span class="sxs-lookup"><span data-stu-id="bcfd5-104">Remove a user or group from the rejectedSenders list.</span></span>

## <a name="permissions"></a><span data-ttu-id="bcfd5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bcfd5-105">Permissions</span></span>
<span data-ttu-id="bcfd5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bcfd5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bcfd5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bcfd5-108">Permission type</span></span>                        | <span data-ttu-id="bcfd5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bcfd5-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="bcfd5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bcfd5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bcfd5-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bcfd5-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="bcfd5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bcfd5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bcfd5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcfd5-113">Not supported.</span></span> |
| <span data-ttu-id="bcfd5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bcfd5-114">Application</span></span>                            | <span data-ttu-id="bcfd5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bcfd5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bcfd5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bcfd5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
DELETE /groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/groups/{other-group-id}
```

## <a name="request-headers"></a><span data-ttu-id="bcfd5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bcfd5-117">Request headers</span></span>

| <span data-ttu-id="bcfd5-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bcfd5-118">Header</span></span>         | <span data-ttu-id="bcfd5-119">Значение</span><span class="sxs-lookup"><span data-stu-id="bcfd5-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="bcfd5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bcfd5-120">Authorization</span></span>  | <span data-ttu-id="bcfd5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bcfd5-p102">Bearer {token}. Required.</span></span> 

## <a name="request-body"></a><span data-ttu-id="bcfd5-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bcfd5-123">Request body</span></span>
<span data-ttu-id="bcfd5-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bcfd5-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcfd5-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="bcfd5-125">Response</span></span>
<span data-ttu-id="bcfd5-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="bcfd5-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcfd5-128">Пример</span><span class="sxs-lookup"><span data-stu-id="bcfd5-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bcfd5-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="bcfd5-129">Request</span></span>
<span data-ttu-id="bcfd5-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bcfd5-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "remove_rejectedSender_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
```

#### <a name="response"></a><span data-ttu-id="bcfd5-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="bcfd5-131">Response</span></span>
<span data-ttu-id="bcfd5-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="bcfd5-132">The following is an example of the response.</span></span> 
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
