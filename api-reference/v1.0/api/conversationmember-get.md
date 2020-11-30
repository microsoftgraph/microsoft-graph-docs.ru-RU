---
title: Получение объекта conversationMember
description: Получение участника чата или канала.
author: laujan
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d010f19945b08a7bd127c19a0938473b73ff0fae
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377098"
---
# <a name="get-conversationmember"></a><span data-ttu-id="bf2b4-103">Получение объекта conversationMember</span><span class="sxs-lookup"><span data-stu-id="bf2b4-103">Get conversationMember</span></span>

<span data-ttu-id="bf2b4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf2b4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bf2b4-105">Получение объекта [conversationMember](../resources/conversationmember.md) из [чата](../resources/chatmessage.md) или [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="bf2b4-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chatmessage.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bf2b4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf2b4-106">Permissions</span></span>

<span data-ttu-id="bf2b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bf2b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf2b4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf2b4-109">Permission Type</span></span>|<span data-ttu-id="bf2b4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf2b4-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="bf2b4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf2b4-111">Delegated (work or school account)</span></span>| <span data-ttu-id="bf2b4-112">Для ресурса **user** или **chat**: Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf2b4-112">For **user** or **chat** resource: Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="bf2b4-113">Для ресурса **channel**: ChannelMember.Read.All, ChannelMember.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bf2b4-113">For **channel** resource: ChannelMember.Read.All, ChannelMember.ReadWrite</span></span> |
|<span data-ttu-id="bf2b4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf2b4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bf2b4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf2b4-115">Not supported.</span></span>|
|<span data-ttu-id="bf2b4-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="bf2b4-116">Application</span></span>| <span data-ttu-id="bf2b4-117">Для ресурса **user** или **chat**: не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf2b4-117">For **user** or **chat** resource: Not supported.</span></span><br/><br/><span data-ttu-id="bf2b4-118">Для ресурса **channel**: TeamMember.Read.Group\*, ChannelMember.Read.All, ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf2b4-118">For **channel** resource: TeamMember.Read.Group\*, ChannelMember.Read.All, ChannelMember.ReadWrite.All</span></span> |

> <span data-ttu-id="bf2b4-119">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="bf2b4-119">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="bf2b4-p102">Before calling this API with application permissions, you must request access. For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="bf2b4-p102">Before calling this API with application permissions, you must request access. For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="bf2b4-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf2b4-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /users/{id}/chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bf2b4-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bf2b4-123">Optional query parameters</span></span>

<span data-ttu-id="bf2b4-124">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="bf2b4-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf2b4-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf2b4-125">Request headers</span></span>

| <span data-ttu-id="bf2b4-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="bf2b4-126">Header</span></span>       | <span data-ttu-id="bf2b4-127">Значение</span><span class="sxs-lookup"><span data-stu-id="bf2b4-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bf2b4-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf2b4-128">Authorization</span></span>  | <span data-ttu-id="bf2b4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf2b4-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bf2b4-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bf2b4-131">Request body</span></span>

<span data-ttu-id="bf2b4-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bf2b4-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf2b4-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf2b4-133">Response</span></span>

<span data-ttu-id="bf2b4-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bf2b4-134">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf2b4-135">Пример</span><span class="sxs-lookup"><span data-stu-id="bf2b4-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf2b4-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf2b4-136">Request</span></span>

<span data-ttu-id="bf2b4-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bf2b4-137">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/V1.0/chats/{id}/members/{id}
```

### <a name="response"></a><span data-ttu-id="bf2b4-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf2b4-138">Response</span></span>

<span data-ttu-id="bf2b4-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bf2b4-139">Here is an example of the response.</span></span>

><span data-ttu-id="bf2b4-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bf2b4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "id": "id-value",
  "displayName": "display-name-value"
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
