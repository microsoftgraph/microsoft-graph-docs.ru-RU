---
title: Удаление участника из чата
description: Удаление conversationMember из чата.
author: AkJo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d8696bbf255621f226409e3e91c4d6b0194f88cc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775908"
---
# <a name="remove-member-from-chat"></a><span data-ttu-id="b4413-103">Удаление участника из чата</span><span class="sxs-lookup"><span data-stu-id="b4413-103">Remove member from chat</span></span>
<span data-ttu-id="b4413-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4413-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4413-105">Удаление [conversationMember](../resources/conversationmember.md) из [чата](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="b4413-105">Remove a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b4413-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4413-106">Permissions</span></span>
<span data-ttu-id="b4413-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4413-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4413-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4413-109">Permission type</span></span>|<span data-ttu-id="b4413-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4413-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4413-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4413-111">Delegated (work or school account)</span></span>| <span data-ttu-id="b4413-112">ChatMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4413-112">ChatMember.ReadWrite.All</span></span> |
|<span data-ttu-id="b4413-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4413-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4413-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b4413-114">Not supported.</span></span>    |
|<span data-ttu-id="b4413-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b4413-115">Application</span></span>| <span data-ttu-id="b4413-116">ChatMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4413-116">ChatMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4413-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4413-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /chats/{chat-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="b4413-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b4413-118">Request headers</span></span>
|<span data-ttu-id="b4413-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b4413-119">Name</span></span>|<span data-ttu-id="b4413-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b4413-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b4413-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b4413-121">Authorization</span></span>|<span data-ttu-id="b4413-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b4413-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4413-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4413-124">Request body</span></span>
<span data-ttu-id="b4413-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b4413-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4413-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4413-126">Response</span></span>

<span data-ttu-id="b4413-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b4413-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b4413-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="b4413-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b4413-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="b4413-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="b4413-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="b4413-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_chat"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```
# <a name="c"></a>[<span data-ttu-id="b4413-131">C#</span><span class="sxs-lookup"><span data-stu-id="b4413-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-members-from-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b4413-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b4413-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-members-from-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b4413-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b4413-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-members-from-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b4413-134">Java</span><span class="sxs-lookup"><span data-stu-id="b4413-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-members-from-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b4413-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4413-135">Response</span></span>
<span data-ttu-id="b4413-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b4413-136">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="b4413-137">См. также</span><span class="sxs-lookup"><span data-stu-id="b4413-137">See also</span></span>

- [<span data-ttu-id="b4413-138">Удаление участника из канала</span><span class="sxs-lookup"><span data-stu-id="b4413-138">Remove member from channel</span></span>](channel-delete-members.md)
- [<span data-ttu-id="b4413-139">Удаление участника из чата</span><span class="sxs-lookup"><span data-stu-id="b4413-139">Remove member from team</span></span>](team-delete-members.md)

