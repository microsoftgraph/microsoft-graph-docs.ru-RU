---
title: Удаление участника из чата
description: Удаление conversationMember из чата.
author: AkJo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cdfc3dd78a82d4f68c7397840b7a4152db24c46f
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872907"
---
# <a name="remove-member-from-chat"></a><span data-ttu-id="607f7-103">Удаление участника из чата</span><span class="sxs-lookup"><span data-stu-id="607f7-103">Remove member from chat</span></span>
<span data-ttu-id="607f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="607f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="607f7-105">Удаление [conversationMember](../resources/conversationmember.md) из [чата](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="607f7-105">Remove a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="607f7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="607f7-106">Permissions</span></span>
<span data-ttu-id="607f7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="607f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="607f7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="607f7-109">Permission type</span></span>|<span data-ttu-id="607f7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="607f7-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="607f7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="607f7-111">Delegated (work or school account)</span></span>| <span data-ttu-id="607f7-112">ChatMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="607f7-112">ChatMember.ReadWrite.All</span></span> |
|<span data-ttu-id="607f7-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="607f7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="607f7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="607f7-114">Not supported.</span></span>    |
|<span data-ttu-id="607f7-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="607f7-115">Application</span></span>| <span data-ttu-id="607f7-116">ChatMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="607f7-116">ChatMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="607f7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="607f7-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /chats/{chat-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="607f7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="607f7-118">Request headers</span></span>
|<span data-ttu-id="607f7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="607f7-119">Name</span></span>|<span data-ttu-id="607f7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="607f7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="607f7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="607f7-121">Authorization</span></span>|<span data-ttu-id="607f7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="607f7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="607f7-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="607f7-124">Request body</span></span>
<span data-ttu-id="607f7-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="607f7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="607f7-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="607f7-126">Response</span></span>

<span data-ttu-id="607f7-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="607f7-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="607f7-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="607f7-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="607f7-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="607f7-129">Request</span></span>

> [!NOTE]
> <span data-ttu-id="607f7-130">С этой функцией связаны некоторые известные проблемы.</span><span class="sxs-lookup"><span data-stu-id="607f7-130">There are some known issues with this functionality.</span></span> <span data-ttu-id="607f7-131">Дополнительные сведения см. в статье [Известные проблемы](/graph/known-issues#unable-to-remove-members-from-chat).</span><span class="sxs-lookup"><span data-stu-id="607f7-131">For details, see [known issues](/graph/known-issues#unable-to-remove-members-from-chat).</span></span>


# <a name="http"></a>[<span data-ttu-id="607f7-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="607f7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_members_from_chat"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```
# <a name="c"></a>[<span data-ttu-id="607f7-133">C#</span><span class="sxs-lookup"><span data-stu-id="607f7-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-members-from-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="607f7-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="607f7-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-members-from-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="607f7-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="607f7-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-members-from-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="607f7-136">Java</span><span class="sxs-lookup"><span data-stu-id="607f7-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-members-from-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="607f7-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="607f7-137">Response</span></span>
<span data-ttu-id="607f7-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="607f7-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="607f7-139">См. также</span><span class="sxs-lookup"><span data-stu-id="607f7-139">See also</span></span>

- [<span data-ttu-id="607f7-140">Удаление участника из канала</span><span class="sxs-lookup"><span data-stu-id="607f7-140">Remove member from channel</span></span>](channel-delete-members.md)
- [<span data-ttu-id="607f7-141">Удаление участника из чата</span><span class="sxs-lookup"><span data-stu-id="607f7-141">Remove member from team</span></span>](team-delete-members.md)

