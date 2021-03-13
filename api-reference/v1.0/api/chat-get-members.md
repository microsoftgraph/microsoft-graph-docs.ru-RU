---
title: Получение объекта conversationMember в чате
description: Получение участника чата.
author: bhartono
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b24b302565c62ee4a422d753160431099a81342d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777575"
---
# <a name="get-conversationmember-in-a-chat"></a><span data-ttu-id="86626-103">Получение объекта conversationMember в чате</span><span class="sxs-lookup"><span data-stu-id="86626-103">Get conversationMember in a chat</span></span>

<span data-ttu-id="86626-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86626-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="86626-105">Получение объекта [conversationMember](../resources/conversationmember.md) из [чата](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="86626-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="86626-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="86626-106">Permissions</span></span>

<span data-ttu-id="86626-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86626-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86626-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="86626-109">Permission Type</span></span>|<span data-ttu-id="86626-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="86626-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="86626-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="86626-111">Delegated (work or school account)</span></span>| <span data-ttu-id="86626-112">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86626-112">ChatMember.Read, ChatMember.ReadWrite, Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span> |
|<span data-ttu-id="86626-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="86626-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86626-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86626-114">Not supported.</span></span>|
|<span data-ttu-id="86626-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="86626-115">Application</span></span>| <span data-ttu-id="86626-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="86626-116">Not supported.</span></span> |

> <span data-ttu-id="86626-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="86626-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="86626-118">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="86626-118">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="86626-119">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="86626-119">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="86626-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="86626-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{chat-id}/members/{membership-id}
GET /users/{user-id}/chats/{chat-id}/members/{membership-id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="86626-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="86626-121">Optional query parameters</span></span>

<span data-ttu-id="86626-122">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="86626-122">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="86626-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="86626-123">Request headers</span></span>

| <span data-ttu-id="86626-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="86626-124">Header</span></span>       | <span data-ttu-id="86626-125">Значение</span><span class="sxs-lookup"><span data-stu-id="86626-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="86626-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="86626-126">Authorization</span></span>  | <span data-ttu-id="86626-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="86626-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="86626-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="86626-129">Request body</span></span>

<span data-ttu-id="86626-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="86626-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86626-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="86626-131">Response</span></span>

<span data-ttu-id="86626-132">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="86626-132">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

> [!NOTE]
> <span data-ttu-id="86626-133">С этой функцией связаны некоторые известные проблемы.</span><span class="sxs-lookup"><span data-stu-id="86626-133">There are some known issues with this functionality.</span></span> <span data-ttu-id="86626-134">Дополнительные сведения см. в статье [Известные проблемы](/graph/known-issues#missing-properties-for-chat-members).</span><span class="sxs-lookup"><span data-stu-id="86626-134">For details, see [known issues](/graph/known-issues#missing-properties-for-chat-members).</span></span>

## <a name="example"></a><span data-ttu-id="86626-135">Пример</span><span class="sxs-lookup"><span data-stu-id="86626-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="86626-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="86626-136">Request</span></span>

<span data-ttu-id="86626-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="86626-137">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members/141c574c-dd90-4131-b173-baf4bb0e894e
```


### <a name="response"></a><span data-ttu-id="86626-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="86626-138">Response</span></span>

<span data-ttu-id="86626-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="86626-139">Here is an example of the response.</span></span>

><span data-ttu-id="86626-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="86626-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- 
{
 "blockType": "response",
  "truncated": true,
  "name": "get_conversation_member",
  "@odata.type": "microsoft.graph.conversationMember"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.type": "#microsoft.graph.aadUserConversationMember",
    "id": "07ad17ad-ada5-4f1f-a650-7a963886a8a7",
    "roles": [ "owner" ],
    "displayName": "Minna Pham",
    "userId": "07ad17ad-ada5-4f1f-a650-7a963886a8a7",
    "email": null,
    "tenantId": "6e5147da-6a35-4275-b3f3-fc069456b6eb",
    "visibleHistoryStartDateTime": "2019-04-18T23:51:43.255Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversation: member get",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


