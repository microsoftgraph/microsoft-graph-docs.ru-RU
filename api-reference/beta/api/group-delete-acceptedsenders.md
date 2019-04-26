---
title: Удаление объекта acceptedSender
description: 'Удаление пользователя или группы из списка принятых отправителей. '
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 22e81f8bbbb497b8209e6faa744a54b24029391c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329771"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="53769-103">Удаление объекта acceptedSender</span><span class="sxs-lookup"><span data-stu-id="53769-103">Remove acceptedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53769-104">Удаление пользователя или группы из списка принятых отправителей для указанной группы.</span><span class="sxs-lookup"><span data-stu-id="53769-104">Remove a user or group from the accepted-senders list of the specified group.</span></span> 

## <a name="permissions"></a><span data-ttu-id="53769-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="53769-105">Permissions</span></span>
<span data-ttu-id="53769-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="53769-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="53769-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="53769-108">Permission type</span></span>                        | <span data-ttu-id="53769-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="53769-109">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="53769-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="53769-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="53769-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53769-111">Group.ReadWrite.All</span></span>    |
| <span data-ttu-id="53769-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="53769-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53769-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53769-113">Not supported.</span></span>|
| <span data-ttu-id="53769-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="53769-114">Application</span></span>                            | <span data-ttu-id="53769-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="53769-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53769-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="53769-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="53769-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="53769-117">Request headers</span></span>
| <span data-ttu-id="53769-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="53769-118">Header</span></span>         | <span data-ttu-id="53769-119">Значение</span><span class="sxs-lookup"><span data-stu-id="53769-119">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="53769-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="53769-120">Authorization</span></span>  | <span data-ttu-id="53769-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="53769-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="53769-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="53769-123">Request body</span></span>
<span data-ttu-id="53769-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="53769-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53769-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="53769-125">Response</span></span>
<span data-ttu-id="53769-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="53769-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="53769-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="53769-128">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="53769-129">Пример 1: Удаление пользователя из списка обслуживаемых отправителей для группы.</span><span class="sxs-lookup"><span data-stu-id="53769-129">Example 1: Remove a user from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="53769-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="53769-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_user_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{user-id}
```

#### <a name="response"></a><span data-ttu-id="53769-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="53769-131">Response</span></span>
<span data-ttu-id="53769-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="53769-132">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "remove_user_from_acceptedsenderslist_of_group",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="53769-133">Пример 2: Удаление группы из списка обслуживаемых отправителей для группы.</span><span class="sxs-lookup"><span data-stu-id="53769-133">Example 2: Remove a group from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="53769-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="53769-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_group_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```

#### <a name="response"></a><span data-ttu-id="53769-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="53769-135">Response</span></span>
<span data-ttu-id="53769-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="53769-136">The following is an example of the response.</span></span> 

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
