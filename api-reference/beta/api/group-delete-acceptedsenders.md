---
title: Удаление объекта acceptedSender
description: 'Удалите пользователя или группу из списка принятых отправителей. '
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: f06e44853c7b78e50ff41a2569f4509ee232b6a3
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681874"
---
# <a name="remove-acceptedsender"></a><span data-ttu-id="7902a-103">Удаление объекта acceptedSender</span><span class="sxs-lookup"><span data-stu-id="7902a-103">Remove acceptedSender</span></span>

<span data-ttu-id="7902a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7902a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7902a-105">Удалите пользователя или группу из списка принятых отправителей указанной группы.</span><span class="sxs-lookup"><span data-stu-id="7902a-105">Remove a user or group from the accepted-senders list of the specified group.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7902a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7902a-106">Permissions</span></span>
<span data-ttu-id="7902a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7902a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7902a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7902a-109">Permission type</span></span>                        | <span data-ttu-id="7902a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7902a-110">Permissions (from least to most privileged)</span></span>  |
|:---------------------------------------|:-------------------------------------------- |
| <span data-ttu-id="7902a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7902a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7902a-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7902a-112">Group.ReadWrite.All</span></span>    |
| <span data-ttu-id="7902a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7902a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7902a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7902a-114">Not supported.</span></span>|
| <span data-ttu-id="7902a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7902a-115">Application</span></span>                            | <span data-ttu-id="7902a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7902a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7902a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7902a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/acceptedSenders/$ref?$id={id}
```

## <a name="request-headers"></a><span data-ttu-id="7902a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7902a-118">Request headers</span></span>
| <span data-ttu-id="7902a-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7902a-119">Header</span></span>         | <span data-ttu-id="7902a-120">Значение</span><span class="sxs-lookup"><span data-stu-id="7902a-120">Value</span></span>                      |
|:---------------|:---------------------------|
| <span data-ttu-id="7902a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7902a-121">Authorization</span></span>  | <span data-ttu-id="7902a-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7902a-p102">Bearer {token}. Required.</span></span>  

## <a name="request-body"></a><span data-ttu-id="7902a-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="7902a-124">Request body</span></span>
<span data-ttu-id="7902a-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7902a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7902a-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="7902a-126">Response</span></span>
<span data-ttu-id="7902a-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="7902a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7902a-129">Примеры</span><span class="sxs-lookup"><span data-stu-id="7902a-129">Examples</span></span>
### <a name="example-1-remove-a-user-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="7902a-130">Пример 1. Удаление пользователя из списка принятых отправителей для группы.</span><span class="sxs-lookup"><span data-stu-id="7902a-130">Example 1: Remove a user from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="7902a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="7902a-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_user_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/users/{user-id}
```

#### <a name="response"></a><span data-ttu-id="7902a-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7902a-132">Response</span></span>
<span data-ttu-id="7902a-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7902a-133">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "name": "remove_user_from_acceptedsenderslist_of_group",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2-remove-a-group-from-the-accepted-senders-list-for-the-group"></a><span data-ttu-id="7902a-134">Пример 2. Удаление группы из списка принятых отправителей для группы.</span><span class="sxs-lookup"><span data-stu-id="7902a-134">Example 2: Remove a group from the accepted-senders list for the group.</span></span>
#### <a name="request"></a><span data-ttu-id="7902a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="7902a-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "remove_group_from_acceptedsenderslist_of_group"
}-->
```http
DELETE https://graph/microsoft.com/beta/groups/{id}/acceptedSenders/$ref?$id=https://graph.microsoft.com/beta/groups/{other-group-id}
```

#### <a name="response"></a><span data-ttu-id="7902a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="7902a-136">Response</span></span>
<span data-ttu-id="7902a-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="7902a-137">The following is an example of the response.</span></span> 

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


