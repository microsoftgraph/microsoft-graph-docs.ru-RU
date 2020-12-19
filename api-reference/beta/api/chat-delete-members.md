---
title: Удаление участника из чата
description: Удаление conversationMember из чата.
author: AkJo
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f1ed1c4b461bebf3bcef1e5e3a4149a043dad30e
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714359"
---
# <a name="remove-member-from-chat"></a><span data-ttu-id="83d32-103">Удаление участника из чата</span><span class="sxs-lookup"><span data-stu-id="83d32-103">Remove member from chat</span></span>
<span data-ttu-id="83d32-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83d32-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="83d32-105">Удаление [conversationMember](../resources/conversationmember.md) из [чата](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="83d32-105">Remove a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="83d32-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="83d32-106">Permissions</span></span>
<span data-ttu-id="83d32-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="83d32-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83d32-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="83d32-109">Permission type</span></span>|<span data-ttu-id="83d32-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="83d32-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83d32-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="83d32-111">Delegated (work or school account)</span></span>| <span data-ttu-id="83d32-112">ChatMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83d32-112">ChatMember.ReadWrite.All</span></span> |
|<span data-ttu-id="83d32-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="83d32-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="83d32-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="83d32-114">Not supported.</span></span>    |
|<span data-ttu-id="83d32-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="83d32-115">Application</span></span>| <span data-ttu-id="83d32-116">ChatMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83d32-116">ChatMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="83d32-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="83d32-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /chats/{chat-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="83d32-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="83d32-118">Request headers</span></span>
|<span data-ttu-id="83d32-119">Имя</span><span class="sxs-lookup"><span data-stu-id="83d32-119">Name</span></span>|<span data-ttu-id="83d32-120">Описание</span><span class="sxs-lookup"><span data-stu-id="83d32-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="83d32-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="83d32-121">Authorization</span></span>|<span data-ttu-id="83d32-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="83d32-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="83d32-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="83d32-124">Request body</span></span>
<span data-ttu-id="83d32-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="83d32-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83d32-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="83d32-126">Response</span></span>

<span data-ttu-id="83d32-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="83d32-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="83d32-128">Примеры</span><span class="sxs-lookup"><span data-stu-id="83d32-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="83d32-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="83d32-129">Request</span></span>

> [!NOTE]
> <span data-ttu-id="83d32-130">С этой функцией связаны некоторые известные проблемы.</span><span class="sxs-lookup"><span data-stu-id="83d32-130">There are some known issues with this functionality.</span></span> <span data-ttu-id="83d32-131">Дополнительные сведения см. в статье [Известные проблемы](/graph/known-issues.md#unable-to-remove-members-from-chat).</span><span class="sxs-lookup"><span data-stu-id="83d32-131">For details, see [known issues](/graph/known-issues.md#unable-to-remove-members-from-chat).</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_members_from_chat"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/MCMjMjQzMmI1N2ItMGFiZC00M2RiLWFhN2ItMTZlYWRkMTE1ZDM0IyMxOTpiZDlkYTQ2MzIzYWY0MjUzOTZkMGZhNjcyMDAyODk4NEB0aHJlYWQudjIjIzQ4YmY5ZDUyLWRjYTctNGE1Zi04Mzk4LTM3Yjk1Y2M3YmQ4Mw==
```

### <a name="response"></a><span data-ttu-id="83d32-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="83d32-132">Response</span></span>
<span data-ttu-id="83d32-133">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="83d32-133">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="83d32-134">См. также</span><span class="sxs-lookup"><span data-stu-id="83d32-134">See also</span></span>

- [<span data-ttu-id="83d32-135">Удаление участника из канала</span><span class="sxs-lookup"><span data-stu-id="83d32-135">Remove member from channel</span></span>](channel-delete-members.md)
- [<span data-ttu-id="83d32-136">Удаление участника из чата</span><span class="sxs-lookup"><span data-stu-id="83d32-136">Remove member from team</span></span>](team-delete-members.md)

