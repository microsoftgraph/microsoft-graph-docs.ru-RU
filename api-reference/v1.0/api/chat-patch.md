---
title: Обновление чата
description: Обновление свойств объекта чата.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 68d60a15767d35bce2d93950f0734e77891f47a2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50958281"
---
# <a name="update-chat"></a><span data-ttu-id="ad148-103">Обновление чата</span><span class="sxs-lookup"><span data-stu-id="ad148-103">Update chat</span></span>
<span data-ttu-id="ad148-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad148-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ad148-105">Обновление свойств объекта [чата.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="ad148-105">Update the properties of a [chat](../resources/chat.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ad148-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ad148-106">Permissions</span></span>
<span data-ttu-id="ad148-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ad148-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad148-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ad148-109">Permission type</span></span>|<span data-ttu-id="ad148-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ad148-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad148-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ad148-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ad148-112">Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ad148-112">Chat.ReadWrite</span></span>|
|<span data-ttu-id="ad148-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ad148-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad148-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad148-114">Not supported.</span></span> |
|<span data-ttu-id="ad148-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ad148-115">Application</span></span> | <span data-ttu-id="ad148-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ad148-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad148-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ad148-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /chats/{chat-id}
```

## <a name="request-headers"></a><span data-ttu-id="ad148-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ad148-118">Request headers</span></span>
|<span data-ttu-id="ad148-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ad148-119">Name</span></span>|<span data-ttu-id="ad148-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ad148-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ad148-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ad148-121">Authorization</span></span>|<span data-ttu-id="ad148-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad148-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ad148-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ad148-124">Content-Type</span></span>|<span data-ttu-id="ad148-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ad148-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad148-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ad148-127">Request body</span></span>
<span data-ttu-id="ad148-128">В теле запроса поставляем JSON-представление объекта [чата.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="ad148-128">In the request body, supply a JSON representation of the [chat](../resources/chat.md) object.</span></span>

<span data-ttu-id="ad148-129">В следующей таблице показаны свойства, которые можно использовать в этом действии.</span><span class="sxs-lookup"><span data-stu-id="ad148-129">The following table shows the properties that can be used with this action.</span></span>

|<span data-ttu-id="ad148-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad148-130">Property</span></span>|<span data-ttu-id="ad148-131">Тип</span><span class="sxs-lookup"><span data-stu-id="ad148-131">Type</span></span>|<span data-ttu-id="ad148-132">Описание</span><span class="sxs-lookup"><span data-stu-id="ad148-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad148-133">topic</span><span class="sxs-lookup"><span data-stu-id="ad148-133">topic</span></span>|<span data-ttu-id="ad148-134">String</span><span class="sxs-lookup"><span data-stu-id="ad148-134">String</span></span>|<span data-ttu-id="ad148-135">Название чата.</span><span class="sxs-lookup"><span data-stu-id="ad148-135">The title of the chat.</span></span> <span data-ttu-id="ad148-136">Это может быть установлено только для чата со **значением chatType** `group` .</span><span class="sxs-lookup"><span data-stu-id="ad148-136">This can only be set for a chat with a **chatType** value of `group`.</span></span>|


## <a name="response"></a><span data-ttu-id="ad148-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad148-137">Response</span></span>

<span data-ttu-id="ad148-138">В случае успешного использования этот метод возвращает код и обновленный ресурс `200 OK response` чата в тексте  отклика.</span><span class="sxs-lookup"><span data-stu-id="ad148-138">If successful, this method returns a `200 OK response` code and the updated **chat** resource in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ad148-139">Примеры</span><span class="sxs-lookup"><span data-stu-id="ad148-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ad148-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="ad148-140">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ad148-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="ad148-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_chat"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/chats/19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2
Content-Type: application/json

{
    "topic": "Group chat title update"
}
```
# <a name="c"></a>[<span data-ttu-id="ad148-142">C#</span><span class="sxs-lookup"><span data-stu-id="ad148-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ad148-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ad148-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ad148-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ad148-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ad148-145">Java</span><span class="sxs-lookup"><span data-stu-id="ad148-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ad148-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="ad148-146">Response</span></span>
><span data-ttu-id="ad148-147">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ad148-147">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats/$entity",
    "id": "19:1c5b01696d2e4a179c292bc9cf04e63b@thread.v2",
    "topic": "Group chat title update",
    "createdDateTime": "2020-12-04T23:11:16.175Z",
    "lastUpdatedDateTime": "2020-12-04T23:12:19.943Z",
    "chatType": "group"
}
```

