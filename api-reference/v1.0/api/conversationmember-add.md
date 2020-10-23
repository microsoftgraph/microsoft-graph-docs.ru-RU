---
title: Добавление Конверсатионмембер
description: Добавление Конверсатионмембер к каналу.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 046c623f5f6e2eb66be063199141529ef50c2720
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733198"
---
# <a name="add-conversationmember"></a><span data-ttu-id="b2957-103">Добавление Конверсатионмембер</span><span class="sxs-lookup"><span data-stu-id="b2957-103">Add conversationMember</span></span>

<span data-ttu-id="b2957-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b2957-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b2957-105">Добавление [конверсатионмембер](../resources/conversationmember.md) к [каналу](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="b2957-105">Add a [conversationMember](../resources/conversationmember.md) to a [channel](../resources/channel.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b2957-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b2957-106">Permissions</span></span>

<span data-ttu-id="b2957-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b2957-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2957-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b2957-109">Permission Type</span></span>|<span data-ttu-id="b2957-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b2957-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="b2957-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b2957-111">Delegated (work or school account)</span></span>| <span data-ttu-id="b2957-112">Чаннелмембер. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b2957-112">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="b2957-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b2957-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2957-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2957-114">Not supported.</span></span>|
|<span data-ttu-id="b2957-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b2957-115">Application</span></span>| <span data-ttu-id="b2957-116">Чаннелмембер. ReadWrite. ALL, Group. ReadWrite. ALL, Directory. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b2957-116">ChannelMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b2957-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b2957-117">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
POST /teams/{id}/channels/{id}/members
```

## <a name="request-headers"></a><span data-ttu-id="b2957-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b2957-118">Request headers</span></span>

| <span data-ttu-id="b2957-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b2957-119">Header</span></span>       | <span data-ttu-id="b2957-120">Значение</span><span class="sxs-lookup"><span data-stu-id="b2957-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b2957-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b2957-121">Authorization</span></span>  | <span data-ttu-id="b2957-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b2957-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b2957-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b2957-124">Request body</span></span>

<span data-ttu-id="b2957-125">Включите в запрос указанные ниже свойства.</span><span class="sxs-lookup"><span data-stu-id="b2957-125">Include the following properties in the request body.</span></span>

| <span data-ttu-id="b2957-126">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2957-126">Property</span></span>   | <span data-ttu-id="b2957-127">Тип</span><span class="sxs-lookup"><span data-stu-id="b2957-127">Type</span></span> |<span data-ttu-id="b2957-128">Описание</span><span class="sxs-lookup"><span data-stu-id="b2957-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b2957-129">roles</span><span class="sxs-lookup"><span data-stu-id="b2957-129">roles</span></span>|<span data-ttu-id="b2957-130">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b2957-130">string collection</span></span>|<span data-ttu-id="b2957-131">Роли этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="b2957-131">The roles for that user.</span></span>|
|<span data-ttu-id="b2957-132">user</span><span class="sxs-lookup"><span data-stu-id="b2957-132">user</span></span>|[<span data-ttu-id="b2957-133">user</span><span class="sxs-lookup"><span data-stu-id="b2957-133">user</span></span>](../resources/user.md)|<span data-ttu-id="b2957-134">Пользователь, добавляемый в канал.</span><span class="sxs-lookup"><span data-stu-id="b2957-134">The user to add to the channel.</span></span>|

## <a name="response"></a><span data-ttu-id="b2957-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2957-135">Response</span></span>

<span data-ttu-id="b2957-136">В случае успеха этот метод возвращает код отклика `201 Created` и объект [conversationMember](../resources/conversationmember.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b2957-136">If successful, this method returns a `201 Created` response code and a [conversationMember](../resources/conversationmember.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2957-137">Пример</span><span class="sxs-lookup"><span data-stu-id="b2957-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="b2957-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b2957-138">Request</span></span>

<span data-ttu-id="b2957-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b2957-139">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_conversation_member"
} -->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels/{id}/members/
content-type: application/json
content-length: 26

{
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "roles": [],
  "user@odata.bind": "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
}
```

### <a name="response"></a><span data-ttu-id="b2957-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b2957-140">Response</span></span>

<span data-ttu-id="b2957-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b2957-141">Here is an example of the response.</span></span>

><span data-ttu-id="b2957-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b2957-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "create_conversation_member",
  "@odata.type": "microsoft.graph.conversationMember"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 468

{
  "@odata.context": "https://graph.microsoft.com/V1.0/$metadata#teams('ece6f0a1-7ca4-498b-be79-edf6c8fc4d82')/channels('19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype')/members/microsoft.graph.aadUserConversationMember/$entity",
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "roles": [],
  "displayName": "John Doe",
  "userId": "8b081ef6-4792-4def-b2c9-c363a1bf41d5",
  "email": null
}
```
