---
title: Обновление conversationMember
description: Обнови роль conversationMember в команде или канале.
author: akjo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 094027c7c62e6077c3eced8e713cfe16e84c3444
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060589"
---
# <a name="update-conversationmember"></a><span data-ttu-id="9f0ec-103">Обновление conversationMember</span><span class="sxs-lookup"><span data-stu-id="9f0ec-103">Update conversationMember</span></span>

<span data-ttu-id="9f0ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f0ec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9f0ec-105">Обновление роли [conversationMember в](../resources/conversationmember.md) [команде или](../resources/team.md) [канале.](../resources/channel.md)</span><span class="sxs-lookup"><span data-stu-id="9f0ec-105">Update the role of a [conversationMember](../resources/conversationmember.md) in a [team](../resources/team.md) or [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9f0ec-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9f0ec-106">Permissions</span></span>

<span data-ttu-id="9f0ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9f0ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f0ec-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9f0ec-109">Permission Type</span></span>|<span data-ttu-id="9f0ec-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9f0ec-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="9f0ec-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9f0ec-111">Delegated (work or school account)</span></span>| <span data-ttu-id="9f0ec-112">В командах: TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f0ec-112">In teams: TeamMember.ReadWrite.All</span></span><br/><span data-ttu-id="9f0ec-113">В каналах: ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f0ec-113">In channels: ChannelMember.ReadWrite.All</span></span>  |
|<span data-ttu-id="9f0ec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9f0ec-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f0ec-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="9f0ec-115">Not supported</span></span>|
|<span data-ttu-id="9f0ec-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="9f0ec-116">Application</span></span>| <span data-ttu-id="9f0ec-117">В командах: TeamMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f0ec-117">In teams: TeamMember.ReadWrite.All</span></span><br/><span data-ttu-id="9f0ec-118">В каналах: ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f0ec-118">In channels:  ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9f0ec-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9f0ec-119">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
PATCH /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="9f0ec-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9f0ec-120">Request headers</span></span>

| <span data-ttu-id="9f0ec-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9f0ec-121">Header</span></span>       | <span data-ttu-id="9f0ec-122">Значение</span><span class="sxs-lookup"><span data-stu-id="9f0ec-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9f0ec-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9f0ec-123">Authorization</span></span>  | <span data-ttu-id="9f0ec-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f0ec-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9f0ec-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9f0ec-126">Request body</span></span>

<span data-ttu-id="9f0ec-127">В теле запроса укажи значения для обновления соответствующих полей.</span><span class="sxs-lookup"><span data-stu-id="9f0ec-127">In the request body, supply the values for the relevant fields to update.</span></span> <span data-ttu-id="9f0ec-128">Предыдущие значения существующих свойств, не включенных в текст запроса, будут сохранены или вычислены повторно с учетом изменений, внесенных в значения других свойств.</span><span class="sxs-lookup"><span data-stu-id="9f0ec-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="9f0ec-129">Для достижения оптимальной производительности не включайте существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="9f0ec-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9f0ec-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="9f0ec-130">Property</span></span>   | <span data-ttu-id="9f0ec-131">Тип</span><span class="sxs-lookup"><span data-stu-id="9f0ec-131">Type</span></span> |<span data-ttu-id="9f0ec-132">Описание</span><span class="sxs-lookup"><span data-stu-id="9f0ec-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f0ec-133">roles</span><span class="sxs-lookup"><span data-stu-id="9f0ec-133">roles</span></span>|<span data-ttu-id="9f0ec-134">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="9f0ec-134">string collection</span></span>|<span data-ttu-id="9f0ec-135">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="9f0ec-135">The roles for that user.</span></span> <span data-ttu-id="9f0ec-136">Должно быть "владельцем" или пустым.</span><span class="sxs-lookup"><span data-stu-id="9f0ec-136">Must be "owner" or empty.</span></span> <span data-ttu-id="9f0ec-137">Гостевых пользователей всегда должны иметь роль "гость" и не может измениться.</span><span class="sxs-lookup"><span data-stu-id="9f0ec-137">Guest users must always have role "guest" and cannot change.</span></span> |

## <a name="response"></a><span data-ttu-id="9f0ec-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f0ec-138">Response</span></span>

<span data-ttu-id="9f0ec-139">В случае успеха этот метод возвращает код отклика `200 OK` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9f0ec-139">If successful, this method returns a `200 OK` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f0ec-140">Пример</span><span class="sxs-lookup"><span data-stu-id="9f0ec-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="9f0ec-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="9f0ec-141">Request</span></span>

<span data-ttu-id="9f0ec-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9f0ec-142">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_conversation_member"
} -->
```http
PATCH https://graph.microsoft.com/V1.0/teams/{id}/channels/{id}/members/{id}
content-type: application/json
content-length: 26

{
  "@odata.type":"#microsoft.graph.aadUserConversationMember",
  "roles": ["owner"]
}
```

### <a name="response"></a><span data-ttu-id="9f0ec-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="9f0ec-143">Response</span></span>

<span data-ttu-id="9f0ec-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9f0ec-144">Here is an example of the response.</span></span>

><span data-ttu-id="9f0ec-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9f0ec-145">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 475

{
  "@odata.context": "https://graph.microsoft.com/V1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "roles": ["owner"],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```
