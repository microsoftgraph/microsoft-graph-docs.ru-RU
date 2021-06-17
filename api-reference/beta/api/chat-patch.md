---
title: Обновление чата
description: Обновление свойств объекта чата.
author: bhartono
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 26ba26e65a96bac04aa418d418b4588ff53f0ffd
ms.sourcegitcommit: 99fdbd9a1806d64626423e1f39342dcde8a1eaf4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/16/2021
ms.locfileid: "52971057"
---
# <a name="update-chat"></a><span data-ttu-id="43b0c-103">Обновление чата</span><span class="sxs-lookup"><span data-stu-id="43b0c-103">Update chat</span></span>
<span data-ttu-id="43b0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43b0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43b0c-105">Обновление свойств объекта [чата.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="43b0c-105">Update the properties of a [chat](../resources/chat.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="43b0c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="43b0c-106">Permissions</span></span>
<span data-ttu-id="43b0c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="43b0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43b0c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="43b0c-109">Permission type</span></span>|<span data-ttu-id="43b0c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="43b0c-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43b0c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="43b0c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="43b0c-112">Chat.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="43b0c-112">Chat.ReadWrite</span></span>|
|<span data-ttu-id="43b0c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="43b0c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43b0c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43b0c-114">Not supported.</span></span> |
|<span data-ttu-id="43b0c-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="43b0c-115">Application</span></span> | <span data-ttu-id="43b0c-116">ChatSettings.ReadWrite.Chat\*, Chat.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43b0c-116">ChatSettings.ReadWrite.Chat\*, Chat.ReadWrite.All</span></span> |

> <span data-ttu-id="43b0c-117">**Примечание**. Разрешения, помеченные звездочкой (\*), используют [согласие для конкретных ресурсов](https://aka.ms/teams-rsc).</span><span class="sxs-lookup"><span data-stu-id="43b0c-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

## <a name="http-request"></a><span data-ttu-id="43b0c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="43b0c-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /chats/{chat-id}
```

## <a name="request-headers"></a><span data-ttu-id="43b0c-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="43b0c-119">Request headers</span></span>
|<span data-ttu-id="43b0c-120">Имя</span><span class="sxs-lookup"><span data-stu-id="43b0c-120">Name</span></span>|<span data-ttu-id="43b0c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="43b0c-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="43b0c-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="43b0c-122">Authorization</span></span>|<span data-ttu-id="43b0c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43b0c-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="43b0c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="43b0c-125">Content-Type</span></span>|<span data-ttu-id="43b0c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="43b0c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="43b0c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="43b0c-128">Request body</span></span>
<span data-ttu-id="43b0c-129">В теле запроса поставляем JSON-представление объекта [чата.](../resources/chat.md)</span><span class="sxs-lookup"><span data-stu-id="43b0c-129">In the request body, supply a JSON representation of the [chat](../resources/chat.md) object.</span></span>

<span data-ttu-id="43b0c-130">В следующей таблице показаны свойства, которые можно использовать в этом действии.</span><span class="sxs-lookup"><span data-stu-id="43b0c-130">The following table shows the properties that can be used with this action.</span></span>

|<span data-ttu-id="43b0c-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="43b0c-131">Property</span></span>|<span data-ttu-id="43b0c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="43b0c-132">Type</span></span>|<span data-ttu-id="43b0c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="43b0c-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43b0c-134">topic</span><span class="sxs-lookup"><span data-stu-id="43b0c-134">topic</span></span>|<span data-ttu-id="43b0c-135">String</span><span class="sxs-lookup"><span data-stu-id="43b0c-135">String</span></span>|<span data-ttu-id="43b0c-136">Название чата.</span><span class="sxs-lookup"><span data-stu-id="43b0c-136">The title of the chat.</span></span> <span data-ttu-id="43b0c-137">Это может быть установлено только для чата со **значением chatType** `group` .</span><span class="sxs-lookup"><span data-stu-id="43b0c-137">This can only be set for a chat with a **chatType** value of `group`.</span></span>|


## <a name="response"></a><span data-ttu-id="43b0c-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="43b0c-138">Response</span></span>

<span data-ttu-id="43b0c-139">В случае успешного использования этот метод возвращает код и обновленный ресурс `200 OK response` чата в тексте  отклика.</span><span class="sxs-lookup"><span data-stu-id="43b0c-139">If successful, this method returns a `200 OK response` code and the updated **chat** resource in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="43b0c-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="43b0c-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="43b0c-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="43b0c-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="43b0c-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="43b0c-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="43b0c-143">C#</span><span class="sxs-lookup"><span data-stu-id="43b0c-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="43b0c-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43b0c-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="43b0c-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43b0c-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="43b0c-146">Java</span><span class="sxs-lookup"><span data-stu-id="43b0c-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="43b0c-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="43b0c-147">Response</span></span>
><span data-ttu-id="43b0c-148">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="43b0c-148">**Note:** The response object shown here might be shortened for readability.</span></span>
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

