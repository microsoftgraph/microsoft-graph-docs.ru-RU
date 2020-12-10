---
title: Добавление приложения в чат
description: Установка приложения для чата.
author: nkramer
localization_priority: Priority
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ce4e7c8bee2535840b2d0f3d6fb234fb38ffbaf2
ms.sourcegitcommit: 59e79cf2693cbb550da3e61eb4f68d9e0f57faf6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2020
ms.locfileid: "49607590"
---
# <a name="add-app-to-chat"></a><span data-ttu-id="70398-103">Добавление приложения в чат</span><span class="sxs-lookup"><span data-stu-id="70398-103">Add app to chat</span></span>

<span data-ttu-id="70398-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70398-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70398-105">Установка [teamsApp](../resources/teamsapp.md) в указанном [чате](../resources/chat.md).</span><span class="sxs-lookup"><span data-stu-id="70398-105">Install a [teamsApp](../resources/teamsapp.md) to the specified [chat](../resources/chat.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="70398-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="70398-106">Permissions</span></span>

<span data-ttu-id="70398-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="70398-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70398-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="70398-109">Permission type</span></span>      | <span data-ttu-id="70398-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="70398-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="70398-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="70398-111">Delegated (work or school account)</span></span> | <span data-ttu-id="70398-112">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span><span class="sxs-lookup"><span data-stu-id="70398-112">TeamsAppInstallation.ReadWriteSelfForChat, TeamsAppInstallation.ReadWriteForChat</span></span> |
|<span data-ttu-id="70398-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="70398-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70398-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70398-114">Not supported.</span></span>    |
|<span data-ttu-id="70398-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="70398-115">Application</span></span> | <span data-ttu-id="70398-116">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span><span class="sxs-lookup"><span data-stu-id="70398-116">TeamsAppInstallation.ReadWriteSelfForChat.All, TeamsAppInstallation.ReadWriteForChat.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="70398-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="70398-117">HTTP request</span></span>

<!-- { 
"blockType": "ignored" 
} -->

```http
POST /chats/{chat-id}/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="70398-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="70398-118">Request headers</span></span>

| <span data-ttu-id="70398-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="70398-119">Header</span></span>       | <span data-ttu-id="70398-120">Значение</span><span class="sxs-lookup"><span data-stu-id="70398-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="70398-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="70398-121">Authorization</span></span>  | <span data-ttu-id="70398-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70398-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="70398-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70398-124">Content-Type</span></span>  | <span data-ttu-id="70398-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="70398-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="70398-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="70398-127">Request body</span></span>

<span data-ttu-id="70398-128">Текст запроса должен содержать идентификатор приложения, созданный приложением каталога.</span><span class="sxs-lookup"><span data-stu-id="70398-128">The request body should contain the catalog app's generated app ID.</span></span> <span data-ttu-id="70398-129">Дополнительные сведения см. в разделе [Свойства teamsApp](../resources/teamsapp.md#properties).</span><span class="sxs-lookup"><span data-stu-id="70398-129">For details, see [teamsApp properties](../resources/teamsapp.md#properties).</span></span>

## <a name="response"></a><span data-ttu-id="70398-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="70398-130">Response</span></span>

<span data-ttu-id="70398-131">В случае успешного выполнения этот метод возвращает код отклика `201 Created`.</span><span class="sxs-lookup"><span data-stu-id="70398-131">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="70398-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="70398-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="70398-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="70398-133">Request</span></span>

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

### <a name="response"></a><span data-ttu-id="70398-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="70398-134">Response</span></span>

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
