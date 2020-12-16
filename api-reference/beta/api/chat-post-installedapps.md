---
title: Добавление приложения в чат
description: Установка приложения для чата.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8d57ac677ff0a09f3be228a8daa002437a9b498d
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689796"
---
# <a name="add-app-to-chat"></a><span data-ttu-id="01e99-103">Добавление приложения в чат</span><span class="sxs-lookup"><span data-stu-id="01e99-103">Add app to chat</span></span>

<span data-ttu-id="01e99-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01e99-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01e99-105">Установка [teamsApp](../resources/teamsapp.md) в указанном [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="01e99-105">Install a [teamsApp](../resources/teamsapp.md) to the specified [chat](../resources/chat.md).</span></span>

> <span data-ttu-id="01e99-106">**Примечание.** Если чат связан с экземпляром [onlineMeeting](../resources/onlinemeeting.md), объект **teamsApp** будет установлен для собрания.</span><span class="sxs-lookup"><span data-stu-id="01e99-106">**Note**: If the chat is associated with an [onlineMeeting](../resources/onlinemeeting.md) instance, then, effectively, the **teamsApp** will get installed to the meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="01e99-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="01e99-107">Permissions</span></span>

<span data-ttu-id="01e99-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="01e99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01e99-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="01e99-110">Permission type</span></span>      | <span data-ttu-id="01e99-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="01e99-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01e99-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="01e99-112">Delegated (work or school account)</span></span> | <span data-ttu-id="01e99-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="01e99-113">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="01e99-114">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="01e99-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01e99-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01e99-115">Not supported.</span></span>    |
|<span data-ttu-id="01e99-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="01e99-116">Application</span></span> | <span data-ttu-id="01e99-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="01e99-117">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01e99-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="01e99-118">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
POST /chats/{chat-id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="01e99-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="01e99-119">Request headers</span></span>

| <span data-ttu-id="01e99-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="01e99-120">Header</span></span>       | <span data-ttu-id="01e99-121">Значение</span><span class="sxs-lookup"><span data-stu-id="01e99-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="01e99-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="01e99-122">Authorization</span></span>  | <span data-ttu-id="01e99-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01e99-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="01e99-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="01e99-125">Content-Type</span></span>  | <span data-ttu-id="01e99-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="01e99-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="01e99-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="01e99-128">Request body</span></span>

<span data-ttu-id="01e99-129">Текст запроса должен содержать идентификатор приложения, созданный приложением каталога.</span><span class="sxs-lookup"><span data-stu-id="01e99-129">The request body should contain the catalog app's generated app ID.</span></span> <span data-ttu-id="01e99-130">Дополнительные сведения см. в разделе [Свойства teamsApp](../resources/teamsapp.md#properties).</span><span class="sxs-lookup"><span data-stu-id="01e99-130">For details, see [teamsApp properties](../resources/teamsapp.md#properties).</span></span>

## <a name="response"></a><span data-ttu-id="01e99-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="01e99-131">Response</span></span>

<span data-ttu-id="01e99-132">В случае успешного выполнения этот метод возвращает код отклика `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="01e99-132">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="01e99-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="01e99-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="01e99-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="01e99-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="01e99-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="01e99-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="01e99-136">C#</span><span class="sxs-lookup"><span data-stu-id="01e99-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-app-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="01e99-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="01e99-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-app-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="01e99-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="01e99-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-app-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="01e99-139">Java</span><span class="sxs-lookup"><span data-stu-id="01e99-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-app-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="01e99-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="01e99-140">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation"
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
