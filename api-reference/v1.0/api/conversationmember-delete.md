---
title: Удаление conversationMember
description: Удаление conversationMember из канала.
author: akjo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 2b0489387f4822296788c417536332c2fef387ad
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060593"
---
# <a name="delete-conversationmember"></a><span data-ttu-id="c2851-103">Удаление conversationMember</span><span class="sxs-lookup"><span data-stu-id="c2851-103">Delete conversationMember</span></span>

<span data-ttu-id="c2851-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2851-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c2851-105">Удаление [conversationMember из](../resources/conversationmember.md) [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="c2851-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="c2851-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2851-106">Permissions</span></span>

<span data-ttu-id="c2851-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2851-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2851-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2851-109">Permission Type</span></span>|<span data-ttu-id="c2851-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2851-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="c2851-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2851-111">Delegated (work or school account)</span></span>| <span data-ttu-id="c2851-112">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2851-112">ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="c2851-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2851-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2851-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2851-114">Not supported.</span></span>|
|<span data-ttu-id="c2851-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="c2851-115">Application</span></span>| <span data-ttu-id="c2851-116">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2851-116">ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2851-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2851-117">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="c2851-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2851-118">Request headers</span></span>

| <span data-ttu-id="c2851-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c2851-119">Header</span></span>       | <span data-ttu-id="c2851-120">Значение</span><span class="sxs-lookup"><span data-stu-id="c2851-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c2851-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2851-121">Authorization</span></span>  | <span data-ttu-id="c2851-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c2851-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c2851-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c2851-124">Request body</span></span>

<span data-ttu-id="c2851-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="c2851-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2851-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2851-126">Response</span></span>

<span data-ttu-id="c2851-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c2851-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c2851-128">Пример</span><span class="sxs-lookup"><span data-stu-id="c2851-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2851-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2851-129">Request</span></span>

<span data-ttu-id="c2851-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2851-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c2851-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2851-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/V1.0/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="c2851-132">C#</span><span class="sxs-lookup"><span data-stu-id="c2851-132">C#</span></span>](#tab/csharp)

# <a name="javascript"></a>[<span data-ttu-id="c2851-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2851-133">JavaScript</span></span>](#tab/javascript)

# <a name="objective-c"></a>[<span data-ttu-id="c2851-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2851-134">Objective-C</span></span>](#tab/objc)

---

### <a name="response"></a><span data-ttu-id="c2851-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2851-135">Response</span></span>

<span data-ttu-id="c2851-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c2851-136">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
