---
title: Добавление приложения в чат
description: Установка приложения для чата.
author: subray
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 53a1792f1dbfb80985078c467eaec810166d23a3
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786186"
---
# <a name="add-app-to-chat"></a><span data-ttu-id="acd98-103">Добавление приложения в чат</span><span class="sxs-lookup"><span data-stu-id="acd98-103">Add app to chat</span></span>

<span data-ttu-id="acd98-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acd98-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acd98-105">Установка [teamsApp](../resources/teamsapp.md) в указанном [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="acd98-105">Install a [teamsApp](../resources/teamsapp.md) to the specified [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="acd98-106">**Примечание.** Если чат связан с экземпляром [onlineMeeting](../resources/onlinemeeting.md), объект **teamsApp** будет установлен для собрания.</span><span class="sxs-lookup"><span data-stu-id="acd98-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the **teamsApp** will get installed to the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="acd98-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="acd98-107">Permissions</span></span>

<span data-ttu-id="acd98-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acd98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acd98-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="acd98-110">Permission type</span></span>      | <span data-ttu-id="acd98-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="acd98-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="acd98-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="acd98-112">Delegated (work or school account)</span></span> | <span data-ttu-id="acd98-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="acd98-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="acd98-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="acd98-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acd98-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acd98-115">Not supported.</span></span>    |
|<span data-ttu-id="acd98-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="acd98-116">Application</span></span> | <span data-ttu-id="acd98-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="acd98-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="acd98-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="acd98-118">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
POST /chats/{chat-id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="acd98-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="acd98-119">Request headers</span></span>

| <span data-ttu-id="acd98-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="acd98-120">Header</span></span>       | <span data-ttu-id="acd98-121">Значение</span><span class="sxs-lookup"><span data-stu-id="acd98-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="acd98-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="acd98-122">Authorization</span></span>  | <span data-ttu-id="acd98-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="acd98-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="acd98-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="acd98-125">Content-Type</span></span>  | <span data-ttu-id="acd98-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="acd98-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="acd98-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="acd98-128">Request body</span></span>

<span data-ttu-id="acd98-p104">Текст запроса должен содержать идентификатор приложения, созданный приложением каталога. Дополнительные сведения см. в разделе [Свойства teamsApp](../resources/teamsapp.md#properties).</span><span class="sxs-lookup"><span data-stu-id="acd98-p104">The request body should contain the catalog app's generated app ID. For details, see [teamsApp properties](../resources/teamsapp.md#properties).</span></span>

## <a name="response"></a><span data-ttu-id="acd98-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="acd98-131">Response</span></span>

<span data-ttu-id="acd98-132">В случае успешного выполнения этот метод возвращает код отклика `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="acd98-132">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="acd98-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="acd98-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="acd98-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="acd98-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="acd98-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="acd98-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_app_in_chat"
}-->

```http
POST https://graph.microsoft.com/beta/chats/19:ea28e88c00e94c7786b065394a61f296@thread.v2/installedApps
Content-Type: application/json

{
"teamsApp@odata.bind":"https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```
# <a name="c"></a>[<span data-ttu-id="acd98-136">C#</span><span class="sxs-lookup"><span data-stu-id="acd98-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-app-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="acd98-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="acd98-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-app-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="acd98-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="acd98-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-app-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="acd98-139">Java</span><span class="sxs-lookup"><span data-stu-id="acd98-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-app-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="acd98-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="acd98-140">Response</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chat add installedapps",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
