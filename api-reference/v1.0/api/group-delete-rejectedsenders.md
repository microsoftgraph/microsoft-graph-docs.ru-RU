---
title: Удаление объекта rejectedSender
description: Удаление пользователя или группы из списка отклоненных отправителей.
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 63e34e39d25ea3e3cc4d352d7caf6a71c86a5a57
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334487"
---
# <a name="remove-rejectedsender"></a><span data-ttu-id="a8e23-103">Удаление объекта rejectedSender</span><span class="sxs-lookup"><span data-stu-id="a8e23-103">Remove rejectedSender</span></span>
<span data-ttu-id="a8e23-104">Удаление пользователя или группы из списка отклоненных отправителей.</span><span class="sxs-lookup"><span data-stu-id="a8e23-104">Remove a user or group from the rejected-senders list.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8e23-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a8e23-105">Permissions</span></span>
<span data-ttu-id="a8e23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a8e23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a8e23-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a8e23-108">Permission type</span></span>                        | <span data-ttu-id="a8e23-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a8e23-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="a8e23-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a8e23-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8e23-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8e23-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="a8e23-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a8e23-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8e23-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8e23-113">Not supported.</span></span> |
| <span data-ttu-id="a8e23-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a8e23-114">Application</span></span>                            | <span data-ttu-id="a8e23-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a8e23-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a8e23-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a8e23-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
DELETE /groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/groups/{other-group-id}
```

## <a name="request-headers"></a><span data-ttu-id="a8e23-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a8e23-117">Request headers</span></span>

| <span data-ttu-id="a8e23-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a8e23-118">Header</span></span>         | <span data-ttu-id="a8e23-119">Значение</span><span class="sxs-lookup"><span data-stu-id="a8e23-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="a8e23-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a8e23-120">Authorization</span></span>  | <span data-ttu-id="a8e23-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a8e23-p102">Bearer {token}. Required.</span></span> 

## <a name="request-body"></a><span data-ttu-id="a8e23-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a8e23-123">Request body</span></span>
<span data-ttu-id="a8e23-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a8e23-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a8e23-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="a8e23-125">Response</span></span>
<span data-ttu-id="a8e23-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a8e23-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8e23-128">Пример</span><span class="sxs-lookup"><span data-stu-id="a8e23-128">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a8e23-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="a8e23-129">Request</span></span>
<span data-ttu-id="a8e23-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a8e23-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "remove_rejectedSender_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/rejectedSenders/$ref?$id=https://graph.microsoft.com/v1.0/users/{user-id}
```

#### <a name="response"></a><span data-ttu-id="a8e23-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a8e23-131">Response</span></span>
<span data-ttu-id="a8e23-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a8e23-132">The following is an example of the response.</span></span> 
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
