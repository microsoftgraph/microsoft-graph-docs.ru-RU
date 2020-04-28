---
title: Удаление объекта acceptedSender
description: 'Удаление пользователя или группы из списка принятых отправителей. '
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2274d3f5e8dfab42b1df9d6da0510ae7d22de463
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123897"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="2a977-103">Удаление объекта acceptedSender</span><span class="sxs-lookup"><span data-stu-id="2a977-103">Remove acceptedSender</span></span>

<span data-ttu-id="2a977-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a977-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a977-105">Удаление пользователя или группы из списка принятых отправителей для указанной группы.</span><span class="sxs-lookup"><span data-stu-id="2a977-105">Remove a user or group from the accepted-senders list of the specified group.</span></span> 

## <a name="permissions"></a><span data-ttu-id="2a977-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a977-106">Permissions</span></span>
<span data-ttu-id="2a977-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a977-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a977-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a977-109">Permission type</span></span>                        | <span data-ttu-id="2a977-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a977-110">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="2a977-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a977-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a977-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a977-112">Group.ReadWrite.All</span></span>    |
| <span data-ttu-id="2a977-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a977-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a977-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a977-114">Not supported.</span></span>|
| <span data-ttu-id="2a977-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a977-115">Application</span></span>                            | <span data-ttu-id="2a977-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a977-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a977-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a977-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="2a977-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a977-118">Request headers</span></span>
| <span data-ttu-id="2a977-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a977-119">Header</span></span>         | <span data-ttu-id="2a977-120">Значение</span><span class="sxs-lookup"><span data-stu-id="2a977-120">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="2a977-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a977-121">Authorization</span></span>  | <span data-ttu-id="2a977-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a977-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="2a977-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2a977-124">Request body</span></span>
<span data-ttu-id="2a977-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2a977-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a977-126">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a977-126">Response</span></span>
<span data-ttu-id="2a977-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2a977-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a977-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="2a977-129">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="2a977-130">Пример 1: Удаление пользователя из списка обслуживаемых отправителей для группы.</span><span class="sxs-lookup"><span data-stu-id="2a977-130">Example 1: Remove a user from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="2a977-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a977-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_user_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{user-id}
```

#### <a name="response"></a><span data-ttu-id="2a977-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a977-132">Response</span></span>
<span data-ttu-id="2a977-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2a977-133">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "remove_user_from_acceptedsenderslist_of_group",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="2a977-134">Пример 2: Удаление группы из списка обслуживаемых отправителей для группы.</span><span class="sxs-lookup"><span data-stu-id="2a977-134">Example 2: Remove a group from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="2a977-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a977-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_group_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```

#### <a name="response"></a><span data-ttu-id="2a977-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="2a977-136">Response</span></span>
<span data-ttu-id="2a977-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2a977-137">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "remove_group_from_acceptedsenderslist_of_group",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Remove acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
