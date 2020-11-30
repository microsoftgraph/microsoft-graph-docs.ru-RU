---
title: Удаление участника из канала
description: Удаление участника из канала.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2a0e2d25368ebc8f8b5026d87ab14544ac091a5d
ms.sourcegitcommit: 2d665f916371aa9515e4c542aa67094abff2fa1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/24/2020
ms.locfileid: "49387583"
---
# <a name="remove-member-from-channel"></a><span data-ttu-id="ece99-103">Удаление участника из канала</span><span class="sxs-lookup"><span data-stu-id="ece99-103">Remove member from channel</span></span>

<span data-ttu-id="ece99-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ece99-104">Namespace: microsoft.graph</span></span>
 
[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ece99-105">Удаление [конверсатионмембер](../resources/conversationmember.md) из [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="ece99-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span> <span data-ttu-id="ece99-106">Эта операция разрешена только для каналов со значением **мембершиптипе** `private` .</span><span class="sxs-lookup"><span data-stu-id="ece99-106">This operation is allowed only for channels with a **membershipType** value of `private`.</span></span>


## <a name="permissions"></a><span data-ttu-id="ece99-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ece99-107">Permissions</span></span>

<span data-ttu-id="ece99-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ece99-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ece99-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ece99-110">Permission Type</span></span>|<span data-ttu-id="ece99-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ece99-111">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="ece99-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ece99-112">Delegated (work or school account)</span></span>| <span data-ttu-id="ece99-113">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ece99-113">ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="ece99-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ece99-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ece99-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ece99-115">Not supported.</span></span>|
|<span data-ttu-id="ece99-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="ece99-116">Application</span></span>| <span data-ttu-id="ece99-117">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ece99-117">ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ece99-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ece99-118">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->

```http
DELETE /teams/{team-id}/channels/{channel-id}/members/{membership-id}
```

## <a name="request-headers"></a><span data-ttu-id="ece99-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ece99-119">Request headers</span></span>

| <span data-ttu-id="ece99-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ece99-120">Header</span></span>       | <span data-ttu-id="ece99-121">Значение</span><span class="sxs-lookup"><span data-stu-id="ece99-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ece99-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ece99-122">Authorization</span></span>  | <span data-ttu-id="ece99-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ece99-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ece99-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ece99-125">Request body</span></span>

<span data-ttu-id="ece99-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ece99-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ece99-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ece99-127">Response</span></span>

<span data-ttu-id="ece99-128">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ece99-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ece99-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ece99-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="ece99-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="ece99-130">Request</span></span>

<span data-ttu-id="ece99-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ece99-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_channel-member"
} -->
```http
DELETE https://graph.microsoft.com/beta/teams/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19%3A56eb04e133944cf69e603c5dac2d292e%40thread.skype/members/ZWUwZjVhZTItOGJjNi00YWU1LTg0NjYtN2RhZWViYmZhMDYyIyM3Mzc2MWYwNi0yYWM5LTQ2OWMtOWYxMC0yNzlhOGNjMjY3Zjk=
```

### <a name="response"></a><span data-ttu-id="ece99-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ece99-132">Response</span></span>

<span data-ttu-id="ece99-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ece99-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="see-also"></a><span data-ttu-id="ece99-134">См. также</span><span class="sxs-lookup"><span data-stu-id="ece99-134">See also</span></span>

- [<span data-ttu-id="ece99-135">Удаление участника из группы</span><span class="sxs-lookup"><span data-stu-id="ece99-135">Remove member from team</span></span>](team-delete-members.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete_channel_member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

