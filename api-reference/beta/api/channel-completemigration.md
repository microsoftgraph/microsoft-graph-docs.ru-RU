---
title: 'канал: completeMigration'
description: Завершите миграцию внешних сообщений, удалив режим миграции из канала.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fb56abf4a30bfe55021535526e86b0e34ebe4bbb
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508782"
---
# <a name="channel-completemigration"></a><span data-ttu-id="90d26-103">канал: completeMigration</span><span class="sxs-lookup"><span data-stu-id="90d26-103">channel: completeMigration</span></span>

<span data-ttu-id="90d26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90d26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90d26-105">Завершите процесс миграции сообщений, `migration mode` удалив [канал](../resources/channel.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="90d26-105">Complete the message migration process by removing `migration mode` from a [channel](../resources/channel.md) in a team.</span></span> <span data-ttu-id="90d26-106">`Migration mode` это специальное состояние, которое предотвращает определенные операции, например отправку сообщений и добавление участников, во время процесса миграции данных.</span><span class="sxs-lookup"><span data-stu-id="90d26-106">`Migration mode` is a special state that prevents certain operations, like sending messages and adding members, during the data migration process.</span></span>

<span data-ttu-id="90d26-107">После выполнения **запроса completeMigration** вы не можете импортировать дополнительные сообщения в команду.</span><span class="sxs-lookup"><span data-stu-id="90d26-107">After a **completeMigration** request is made, you cannot import additional messages into the team.</span></span> <span data-ttu-id="90d26-108">Вы можете добавить членов в команду после успешного ответа на запрос.</span><span class="sxs-lookup"><span data-stu-id="90d26-108">You can add members to the team after the request returns a successful response.</span></span>

## <a name="permissions"></a><span data-ttu-id="90d26-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90d26-109">Permissions</span></span>

<span data-ttu-id="90d26-110">Для вызова этого API требуется следующее разрешение.</span><span class="sxs-lookup"><span data-stu-id="90d26-110">The following permission is required to call this API.</span></span> <span data-ttu-id="90d26-111">Дополнительные дополнительные новости *см. в см. в* ["Разрешениях".](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="90d26-111">To learn more, *see* [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90d26-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90d26-112">Permission type</span></span>      | <span data-ttu-id="90d26-113">Разрешение</span><span class="sxs-lookup"><span data-stu-id="90d26-113">Permission</span></span>  |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="90d26-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90d26-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="90d26-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90d26-115">Not supported.</span></span>|
| <span data-ttu-id="90d26-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90d26-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90d26-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90d26-117">Not supported.</span></span> |
|<span data-ttu-id="90d26-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90d26-118">Application</span></span> | <span data-ttu-id="90d26-119">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="90d26-119">Teamwork.Migrate.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90d26-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90d26-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels/{channel-id}/completeMigration
```

## <a name="request-headers"></a><span data-ttu-id="90d26-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90d26-121">Request headers</span></span>

| <span data-ttu-id="90d26-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="90d26-122">Header</span></span>       | <span data-ttu-id="90d26-123">Значение</span><span class="sxs-lookup"><span data-stu-id="90d26-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="90d26-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="90d26-124">Authorization</span></span>  | <span data-ttu-id="90d26-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90d26-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="90d26-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="90d26-127">Request body</span></span>

<span data-ttu-id="90d26-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90d26-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90d26-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="90d26-129">Response</span></span>

<span data-ttu-id="90d26-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="90d26-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90d26-132">Пример</span><span class="sxs-lookup"><span data-stu-id="90d26-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="90d26-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="90d26-133">Request</span></span>

<span data-ttu-id="90d26-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90d26-134">The following is an example of the request.</span></span>
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD022 -->



# <a name="http"></a>[<span data-ttu-id="90d26-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="90d26-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "completeMigration_channel"
}-->

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels/19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2/completeMigration
```
# <a name="c"></a>[<span data-ttu-id="90d26-136">C#</span><span class="sxs-lookup"><span data-stu-id="90d26-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/completemigration-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90d26-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90d26-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/completemigration-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90d26-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90d26-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/completemigration-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90d26-139">Java</span><span class="sxs-lookup"><span data-stu-id="90d26-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/completemigration-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="90d26-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="90d26-140">Response</span></span>

<span data-ttu-id="90d26-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="90d26-141">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 5793eec6-0e5a-11eb-adc1-0242ac120002
2020-10-14 20:22:11 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "completeMigration_ channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
