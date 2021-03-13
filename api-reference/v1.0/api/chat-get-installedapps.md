---
title: Получение установленного приложения в чате
description: Получение установленного приложения в чате.
author: subray
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 124f1811516e9ea5de87c41bcb154c4001e74fed
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777582"
---
# <a name="get-installed-app-in-chat"></a><span data-ttu-id="db72b-103">Получение установленного приложения в чате</span><span class="sxs-lookup"><span data-stu-id="db72b-103">Get installed app in chat</span></span>

<span data-ttu-id="db72b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db72b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="db72b-105">Получение [приложения](../resources/teamsappinstallation.md), установленного в [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="db72b-105">Get an [app](../resources/teamsappinstallation.md) installed in a [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="db72b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="db72b-106">Permissions</span></span>

<span data-ttu-id="db72b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db72b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db72b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="db72b-109">Permission type</span></span>      | <span data-ttu-id="db72b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="db72b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="db72b-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="db72b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="db72b-112">TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="db72b-112">TeamsAppInstallation.ReadForChat, TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="db72b-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="db72b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="db72b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db72b-114">Not supported.</span></span>    |
|<span data-ttu-id="db72b-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="db72b-115">Application</span></span> | <span data-ttu-id="db72b-116">TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="db72b-116">TeamsAppInstallation.ReadForChat.All, TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span>

## <a name="http-request"></a><span data-ttu-id="db72b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="db72b-117">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
GET /chats/{chat-id}/installedApps/{app-installation-id}
```

## <a name="request-headers"></a><span data-ttu-id="db72b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="db72b-118">Request headers</span></span>

|<span data-ttu-id="db72b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="db72b-119">Name</span></span>|<span data-ttu-id="db72b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="db72b-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="db72b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="db72b-121">Authorization</span></span>|<span data-ttu-id="db72b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="db72b-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="db72b-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="db72b-124">Response</span></span>

<span data-ttu-id="db72b-125">В случае успеха этот метод возвратит код отклика `200 OK` и объект [driveItem](../resources/teamsapp.md) в тексте сообщения.</span><span class="sxs-lookup"><span data-stu-id="db72b-125">If successful, this method returns a `200 OK` and a [teamsApp](../resources/teamsapp.md) object in the body.</span></span>

## <a name="example"></a><span data-ttu-id="db72b-126">Пример</span><span class="sxs-lookup"><span data-stu-id="db72b-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="db72b-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="db72b-127">Request</span></span>

<span data-ttu-id="db72b-128">В следующем примере показано, как получить приложение, установленное в указанном чате.</span><span class="sxs-lookup"><span data-stu-id="db72b-128">The following example gets an app installed in the specified chat.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_installedApps_in_chat"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/installedApps/MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=
```


### <a name="response"></a><span data-ttu-id="db72b-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="db72b-129">Response</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chats('19%3Ad65713bc498c4a428c71ef9353e6ce20%40thread.v2')/installedApps/$entity",
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
