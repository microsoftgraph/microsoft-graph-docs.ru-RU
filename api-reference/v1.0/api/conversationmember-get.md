---
title: Получение объекта conversationMember
description: Получение участника чата или канала.
author: laujan
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 79c38e9f8f2dbe378198e01610c57453eb7a2ba8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50515816"
---
# <a name="get-conversationmember"></a><span data-ttu-id="b8239-103">Получение объекта conversationMember</span><span class="sxs-lookup"><span data-stu-id="b8239-103">Get conversationMember</span></span>

<span data-ttu-id="b8239-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8239-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b8239-105">Получение объекта [conversationMember](../resources/conversationmember.md) из [чата](../resources/chatmessage.md) или [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="b8239-105">Retrieve a [conversationMember](../resources/conversationmember.md) from a [chat](../resources/chatmessage.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b8239-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b8239-106">Permissions</span></span>

<span data-ttu-id="b8239-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b8239-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8239-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b8239-109">Permission Type</span></span>|<span data-ttu-id="b8239-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b8239-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="b8239-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b8239-111">Delegated (work or school account)</span></span>| <span data-ttu-id="b8239-112">Для ресурса **user** или **chat**: Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8239-112">For **user** or **chat** resource: Chat.ReadBasic, Chat.Read, Chat.ReadWrite</span></span><br/><br/><span data-ttu-id="b8239-113">Для ресурса **channel**: ChannelMember.Read.All, ChannelMember.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b8239-113">For **channel** resource: ChannelMember.Read.All, ChannelMember.ReadWrite</span></span> |
|<span data-ttu-id="b8239-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b8239-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8239-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8239-115">Not supported.</span></span>|
|<span data-ttu-id="b8239-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="b8239-116">Application</span></span>| <span data-ttu-id="b8239-117">Для ресурса **user** или **chat**: не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b8239-117">For **user** or **chat** resource: Not supported.</span></span><br/><br/><span data-ttu-id="b8239-118">Для ресурса **channel**: TeamMember.Read.Group\*, ChannelMember.Read.All, ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8239-118">For **channel** resource: TeamMember.Read.Group\*, ChannelMember.Read.All, ChannelMember.ReadWrite.All</span></span> |

> <span data-ttu-id="b8239-119">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="b8239-119">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> [!NOTE]
> <span data-ttu-id="b8239-120">Перед вызовом этого API с разрешениями приложения необходимо запросить доступ.</span><span class="sxs-lookup"><span data-stu-id="b8239-120">Before calling this API with application permissions, you must request access.</span></span> <span data-ttu-id="b8239-121">Дополнительные сведения см. в статье [Защищенные APIs в Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="b8239-121">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span>

## <a name="http-request"></a><span data-ttu-id="b8239-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b8239-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /chats/{id}/members/{id}
GET /teams/{id}/channels/{id}/members/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b8239-123">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="b8239-123">Optional query parameters</span></span>

<span data-ttu-id="b8239-124">Эта операция не поддерживает [параметры запросов OData](/graph/query-parameters) для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="b8239-124">This operation does not support the [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b8239-125">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b8239-125">Request headers</span></span>

| <span data-ttu-id="b8239-126">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b8239-126">Header</span></span>       | <span data-ttu-id="b8239-127">Значение</span><span class="sxs-lookup"><span data-stu-id="b8239-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b8239-128">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b8239-128">Authorization</span></span>  | <span data-ttu-id="b8239-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b8239-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b8239-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b8239-131">Request body</span></span>

<span data-ttu-id="b8239-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b8239-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b8239-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8239-133">Response</span></span>

<span data-ttu-id="b8239-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b8239-134">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8239-135">Пример</span><span class="sxs-lookup"><span data-stu-id="b8239-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8239-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="b8239-136">Request</span></span>

<span data-ttu-id="b8239-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b8239-137">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_conversation_member"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/V1.0/chats/{id}/members/{id}
```

### <a name="response"></a><span data-ttu-id="b8239-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="b8239-138">Response</span></span>

<span data-ttu-id="b8239-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b8239-139">Here is an example of the response.</span></span>

><span data-ttu-id="b8239-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b8239-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
