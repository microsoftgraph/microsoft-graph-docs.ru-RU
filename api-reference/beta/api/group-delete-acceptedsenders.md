---
title: Удаление объекта acceptedSender
description: 'Удаление пользователя или группы из списка принятых отправителей. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 341f887de0252dd6ae1ebc9f899263c67716658f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954034"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="a2cf2-103">Удаление объекта acceptedSender</span><span class="sxs-lookup"><span data-stu-id="a2cf2-103">Remove acceptedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a2cf2-104">Удаление пользователя или группы из списка принятых отправителей для указанной группы.</span><span class="sxs-lookup"><span data-stu-id="a2cf2-104">Remove a user or group from the accepted-senders list of the specified group.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a2cf2-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a2cf2-105">Permissions</span></span>
<span data-ttu-id="a2cf2-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2cf2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a2cf2-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a2cf2-108">Permission type</span></span>                        | <span data-ttu-id="a2cf2-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a2cf2-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="a2cf2-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a2cf2-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="a2cf2-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2cf2-111">Group.ReadWrite.All</span></span>    |
| <span data-ttu-id="a2cf2-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a2cf2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a2cf2-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2cf2-113">Not supported.</span></span>|
| <span data-ttu-id="a2cf2-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a2cf2-114">Application</span></span>                            | <span data-ttu-id="a2cf2-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a2cf2-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2cf2-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a2cf2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="a2cf2-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a2cf2-117">Request headers</span></span>
| <span data-ttu-id="a2cf2-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a2cf2-118">Header</span></span>         | <span data-ttu-id="a2cf2-119">Значение</span><span class="sxs-lookup"><span data-stu-id="a2cf2-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="a2cf2-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a2cf2-120">Authorization</span></span>  | <span data-ttu-id="a2cf2-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a2cf2-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="a2cf2-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a2cf2-123">Request body</span></span>
<span data-ttu-id="a2cf2-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a2cf2-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a2cf2-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="a2cf2-125">Response</span></span>
<span data-ttu-id="a2cf2-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a2cf2-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a2cf2-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="a2cf2-128">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="a2cf2-129">Пример 1: Удаление пользователя из списка обслуживаемых отправителей для группы.</span><span class="sxs-lookup"><span data-stu-id="a2cf2-129">Example 1: Remove a user from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="a2cf2-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2cf2-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_user_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{user-id}
```

#### <a name="response"></a><span data-ttu-id="a2cf2-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2cf2-131">Response</span></span>
<span data-ttu-id="a2cf2-132">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a2cf2-132">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "remove_user_from_acceptedsenderslist_of_group",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="a2cf2-133">Пример 2: Удаление группы из списка обслуживаемых отправителей для группы.</span><span class="sxs-lookup"><span data-stu-id="a2cf2-133">Example 2: Remove a group from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="a2cf2-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="a2cf2-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_group_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```

#### <a name="response"></a><span data-ttu-id="a2cf2-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="a2cf2-135">Response</span></span>
<span data-ttu-id="a2cf2-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a2cf2-136">The following is an example of the response.</span></span> 

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
