---
title: Получение установленного приложения в чате
description: Получение установленного приложения в чате.
author: subray
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a83c9cf192d5c30ccdc8c3a88d5ac5c699e6d971
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775859"
---
# <a name="get-installed-app-in-chat"></a><span data-ttu-id="11722-103">Получение установленного приложения в чате</span><span class="sxs-lookup"><span data-stu-id="11722-103">Get installed app in chat</span></span>

<span data-ttu-id="11722-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11722-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11722-105">Получение [приложения](../resources/teamsappinstallation.md), установленного в [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="11722-105">Get an [app](../resources/teamsappinstallation.md) installed in a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="11722-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="11722-106">Permissions</span></span>

<span data-ttu-id="11722-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="11722-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11722-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="11722-109">Permission type</span></span>      | <span data-ttu-id="11722-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="11722-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11722-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="11722-111">Delegated (work or school account)</span></span> | <span data-ttu-id="11722-112">TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="11722-112">TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="11722-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="11722-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11722-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="11722-114">Not supported.</span></span>    |
|<span data-ttu-id="11722-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="11722-115">Application</span></span> | <span data-ttu-id="11722-116">TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="11722-116">TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span>

## <a name="http-request"></a><span data-ttu-id="11722-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="11722-117">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
GET /chats/{chat-id}/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="11722-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="11722-118">Request headers</span></span>

|<span data-ttu-id="11722-119">Имя</span><span class="sxs-lookup"><span data-stu-id="11722-119">Name</span></span>|<span data-ttu-id="11722-120">Описание</span><span class="sxs-lookup"><span data-stu-id="11722-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="11722-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="11722-121">Authorization</span></span>|<span data-ttu-id="11722-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="11722-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="11722-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="11722-124">Response</span></span>

<span data-ttu-id="11722-125">В случае успеха этот метод возвратит код отклика `200 OK` и объект [driveItem](../resources/teamsapp.md) в тексте сообщения.</span><span class="sxs-lookup"><span data-stu-id="11722-125">If successful, this method returns a `200 OK` and a [teamsApp](../resources/teamsapp.md) object in the body.</span></span>

## <a name="example"></a><span data-ttu-id="11722-126">Пример</span><span class="sxs-lookup"><span data-stu-id="11722-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="11722-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="11722-127">Request</span></span>

<span data-ttu-id="11722-128">В следующем примере показано, как получить приложение, установленное в указанном чате.</span><span class="sxs-lookup"><span data-stu-id="11722-128">The following example gets an app installed in the specified chat.</span></span>

# <a name="http"></a>[<span data-ttu-id="11722-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="11722-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_installedApps_in_chat"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/installedApps/MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=
```
# <a name="c"></a>[<span data-ttu-id="11722-130">C#</span><span class="sxs-lookup"><span data-stu-id="11722-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-installedapps-in-chat-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11722-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11722-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-installedapps-in-chat-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11722-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11722-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-installedapps-in-chat-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11722-133">Java</span><span class="sxs-lookup"><span data-stu-id="11722-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-installedapps-in-chat-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="11722-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="11722-134">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#chats('19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2')/installedApps/$entity",
    "id": "MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc="
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Chat get installedapps",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
