---
title: 'канал: Комплетемигратион'
description: Завершите Перенос внешних сообщений, удалив режим миграции из канала.
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 46d93265721924181030fbb9cd95bf71cef38d8d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48959354"
---
# <a name="channel-completemigration"></a><span data-ttu-id="2f066-103">канал: Комплетемигратион</span><span class="sxs-lookup"><span data-stu-id="2f066-103">channel: completeMigration</span></span>

<span data-ttu-id="2f066-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f066-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f066-105">Завершите процесс переноса сообщений, удалив `migration mode` из [канала](../resources/channel.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="2f066-105">Complete the message migration process by removing `migration mode` from a [channel](../resources/channel.md) in a team.</span></span> <span data-ttu-id="2f066-106">`Migration mode` — Это специальное состояние, которое предотвращает некоторые операции, например отправку сообщений и добавление участников, в процессе переноса данных.</span><span class="sxs-lookup"><span data-stu-id="2f066-106">`Migration mode` is a special state that prevents certain operations, like sending messages and adding members, during the data migration process.</span></span>

<span data-ttu-id="2f066-107">После выполнения запроса **комплетемигратион** вы не можете импортировать в команду Дополнительные сообщения.</span><span class="sxs-lookup"><span data-stu-id="2f066-107">After a **completeMigration** request is made, you cannot import additional messages into the team.</span></span> <span data-ttu-id="2f066-108">Вы можете добавлять участников в команду после того, как запрос возвращает успешный ответ.</span><span class="sxs-lookup"><span data-stu-id="2f066-108">You can add members to the team after the request returns a successful response.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f066-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2f066-109">Permissions</span></span>

<span data-ttu-id="2f066-110">Для вызова этого API требуется следующее разрешение.</span><span class="sxs-lookup"><span data-stu-id="2f066-110">The following permission is required to call this API.</span></span> <span data-ttu-id="2f066-111">Чтобы узнать больше, *Ознакомьтесь* с [разрешениями](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2f066-111">To learn more, *see* [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f066-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2f066-112">Permission type</span></span>      | <span data-ttu-id="2f066-113">Разрешение</span><span class="sxs-lookup"><span data-stu-id="2f066-113">Permission</span></span>  |
|:--------------------|:---------------------------------------------------------|
| <span data-ttu-id="2f066-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2f066-114">Delegated (work or school account)</span></span>  | <span data-ttu-id="2f066-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f066-115">Not supported.</span></span>|
| <span data-ttu-id="2f066-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2f066-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2f066-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2f066-117">Not supported.</span></span> |
|<span data-ttu-id="2f066-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2f066-118">Application</span></span> | <span data-ttu-id="2f066-119">Teamwork.Migrate.All</span><span class="sxs-lookup"><span data-stu-id="2f066-119">Teamwork.Migrate.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f066-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2f066-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{teamId}/channels/{channelId}/completeMigration
```

## <a name="request-headers"></a><span data-ttu-id="2f066-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2f066-121">Request headers</span></span>

| <span data-ttu-id="2f066-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2f066-122">Header</span></span>       | <span data-ttu-id="2f066-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2f066-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2f066-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2f066-124">Authorization</span></span>  | <span data-ttu-id="2f066-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f066-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f066-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2f066-127">Request body</span></span>

<span data-ttu-id="2f066-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2f066-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2f066-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f066-129">Response</span></span>

<span data-ttu-id="2f066-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2f066-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f066-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2f066-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f066-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2f066-133">Request</span></span>

<span data-ttu-id="2f066-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2f066-134">The following is an example of the request.</span></span>
<!-- markdownlint-disable MD025 -->
<!-- markdownlint-disable MD022 -->


# <a name="http"></a>[<span data-ttu-id="2f066-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2f066-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "completeMigration_channel"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/completeMigration
```
# <a name="c"></a>[<span data-ttu-id="2f066-136">C#</span><span class="sxs-lookup"><span data-stu-id="2f066-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/completemigration-channel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2f066-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2f066-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/completemigration-channel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2f066-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2f066-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/completemigration-channel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2f066-139">Java</span><span class="sxs-lookup"><span data-stu-id="2f066-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/completemigration-channel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
### <a name="response"></a><span data-ttu-id="2f066-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2f066-140">Response</span></span>

<span data-ttu-id="2f066-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2f066-141">The following is an example of the response.</span></span>
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
