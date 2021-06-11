---
title: Обновление чата
description: Обновление свойств объекта чата.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cd906d473977987fc3859aee05d9b88b321cac60
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896475"
---
# <a name="update-chat"></a><span data-ttu-id="6dcf6-103">Обновление чата</span><span class="sxs-lookup"><span data-stu-id="6dcf6-103">Update chat</span></span>
<span data-ttu-id="6dcf6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dcf6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dcf6-105">Обновление свойств объекта [чата.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="6dcf6-105">Update the properties of a [chat](../resources/chat.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6dcf6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6dcf6-106">Permissions</span></span>
<span data-ttu-id="6dcf6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6dcf6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6dcf6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6dcf6-109">Permission type</span></span>|<span data-ttu-id="6dcf6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6dcf6-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6dcf6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6dcf6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6dcf6-112">Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6dcf6-112">Chat.ReadWrite</span></span>|
|<span data-ttu-id="6dcf6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6dcf6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dcf6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dcf6-114">Not supported.</span></span> |
|<span data-ttu-id="6dcf6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6dcf6-115">Application</span></span> | <span data-ttu-id="6dcf6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6dcf6-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6dcf6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6dcf6-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /chats/{chat-id}
```

## <a name="request-headers"></a><span data-ttu-id="6dcf6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6dcf6-118">Request headers</span></span>
|<span data-ttu-id="6dcf6-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6dcf6-119">Name</span></span>|<span data-ttu-id="6dcf6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6dcf6-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6dcf6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6dcf6-121">Authorization</span></span>|<span data-ttu-id="6dcf6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6dcf6-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6dcf6-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6dcf6-124">Content-Type</span></span>|<span data-ttu-id="6dcf6-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6dcf6-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6dcf6-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6dcf6-127">Request body</span></span>
<span data-ttu-id="6dcf6-128">В теле запроса поставляем JSON-представление объекта [чата.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="6dcf6-128">In the request body, supply a JSON representation of the [chat](../resources/chat.md) object.</span></span>

<span data-ttu-id="6dcf6-129">В следующей таблице показаны свойства, которые можно использовать в этом действии.</span><span class="sxs-lookup"><span data-stu-id="6dcf6-129">The following table shows the properties that can be used with this action.</span></span>

|<span data-ttu-id="6dcf6-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="6dcf6-130">Property</span></span>|<span data-ttu-id="6dcf6-131">Тип</span><span class="sxs-lookup"><span data-stu-id="6dcf6-131">Type</span></span>|<span data-ttu-id="6dcf6-132">Описание</span><span class="sxs-lookup"><span data-stu-id="6dcf6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dcf6-133">topic</span><span class="sxs-lookup"><span data-stu-id="6dcf6-133">topic</span></span>|<span data-ttu-id="6dcf6-134">String</span><span class="sxs-lookup"><span data-stu-id="6dcf6-134">String</span></span>|<span data-ttu-id="6dcf6-135">Название чата.</span><span class="sxs-lookup"><span data-stu-id="6dcf6-135">The title of the chat.</span></span> <span data-ttu-id="6dcf6-136">Это может быть установлено только для чата со **значением chatType** `group` .</span><span class="sxs-lookup"><span data-stu-id="6dcf6-136">This can only be set for a chat with a **chatType** value of `group`.</span></span>|


## <a name="response"></a><span data-ttu-id="6dcf6-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dcf6-137">Response</span></span>

<span data-ttu-id="6dcf6-138">В случае успешного использования этот метод возвращает код и обновленный ресурс `200 OK response` чата в тексте  отклика.</span><span class="sxs-lookup"><span data-stu-id="6dcf6-138">If successful, this method returns a `200 OK response` code and the updated **chat** resource in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6dcf6-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="6dcf6-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6dcf6-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="6dcf6-140">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6dcf6-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="6dcf6-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chat"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/chats/19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2
Content-Type: application/json

{
    "topic": "Group chat title update"
}
```
# <a name="c"></a>[<span data-ttu-id="6dcf6-142">C#</span><span class="sxs-lookup"><span data-stu-id="6dcf6-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6dcf6-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6dcf6-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6dcf6-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6dcf6-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6dcf6-145">Java</span><span class="sxs-lookup"><span data-stu-id="6dcf6-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6dcf6-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="6dcf6-146">Response</span></span>
><span data-ttu-id="6dcf6-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6dcf6-147">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chat"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats/$entity",
    "id": "19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2",
    "topic": "Group chat title update",
    "createdDateTime": "2020-12-04T23:11:16.175Z",
    "lastUpdatedDateTime": "2020-12-04T23:12:19.943Z",
    "chatType": "group",
    "webUrl": "https://teams.microsoft.com/l/chat/19%3A1c5b01696d2e4a179c292bc9cf04e63b@thread.v2/0?tenantId=b33cbe9f-8ebe-4f2a-912b-7e2a427f477f"
}
```

