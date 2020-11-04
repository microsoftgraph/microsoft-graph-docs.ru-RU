---
title: Удаление Конверсатионмембер
description: Удаление Конверсатионмембер из канала.
author: laujan
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 05dd3377e5a3161a38d9db1d56de7bba7ccf9af4
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848327"
---
# <a name="delete-conversationmember"></a><span data-ttu-id="8d6f4-103">Удаление Конверсатионмембер</span><span class="sxs-lookup"><span data-stu-id="8d6f4-103">Delete conversationMember</span></span>

<span data-ttu-id="8d6f4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d6f4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8d6f4-105">Удаление [конверсатионмембер](../resources/conversationmember.md) из [канала](../resources/channel.md).</span><span class="sxs-lookup"><span data-stu-id="8d6f4-105">Delete a [conversationMember](../resources/conversationmember.md) from a [channel](../resources/channel.md).</span></span>


## <a name="permissions"></a><span data-ttu-id="8d6f4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8d6f4-106">Permissions</span></span>

<span data-ttu-id="8d6f4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, в том числе о выборе разрешений, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8d6f4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d6f4-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8d6f4-109">Permission Type</span></span>|<span data-ttu-id="8d6f4-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8d6f4-110">Permissions (from least to most privileged)</span></span>|
|---------|-------------|
|<span data-ttu-id="8d6f4-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8d6f4-111">Delegated (work or school account)</span></span>| <span data-ttu-id="8d6f4-112">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d6f4-112">ChannelMember.ReadWrite.All</span></span> |
|<span data-ttu-id="8d6f4-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8d6f4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d6f4-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d6f4-114">Not supported.</span></span>|
|<span data-ttu-id="8d6f4-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8d6f4-115">Application</span></span>| <span data-ttu-id="8d6f4-116">ChannelMember.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d6f4-116">ChannelMember.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8d6f4-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8d6f4-117">HTTP request</span></span>
<!-- { "blockType": "ignored"} -->
```http
DELETE /teams/{id}/channels/{id}/members/{id}
```

## <a name="request-headers"></a><span data-ttu-id="8d6f4-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8d6f4-118">Request headers</span></span>

| <span data-ttu-id="8d6f4-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8d6f4-119">Header</span></span>       | <span data-ttu-id="8d6f4-120">Значение</span><span class="sxs-lookup"><span data-stu-id="8d6f4-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8d6f4-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8d6f4-121">Authorization</span></span>  | <span data-ttu-id="8d6f4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8d6f4-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8d6f4-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8d6f4-124">Request body</span></span>

<span data-ttu-id="8d6f4-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8d6f4-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8d6f4-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d6f4-126">Response</span></span>

<span data-ttu-id="8d6f4-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="8d6f4-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="8d6f4-128">Пример</span><span class="sxs-lookup"><span data-stu-id="8d6f4-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d6f4-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="8d6f4-129">Request</span></span>

<span data-ttu-id="8d6f4-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8d6f4-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8d6f4-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8d6f4-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_conversation_member"
} -->
```http
DELETE https://graph.microsoft.com/V1.0/teams/{id}/channels/{id}/members/{id}
```
# <a name="c"></a>[<span data-ttu-id="8d6f4-132">C#</span><span class="sxs-lookup"><span data-stu-id="8d6f4-132">C#</span></span>](#tab/csharp)

# <a name="javascript"></a>[<span data-ttu-id="8d6f4-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8d6f4-133">JavaScript</span></span>](#tab/javascript)

# <a name="objective-c"></a>[<span data-ttu-id="8d6f4-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8d6f4-134">Objective-C</span></span>](#tab/objc)

---

### <a name="response"></a><span data-ttu-id="8d6f4-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8d6f4-135">Response</span></span>

<span data-ttu-id="8d6f4-136">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8d6f4-136">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```
