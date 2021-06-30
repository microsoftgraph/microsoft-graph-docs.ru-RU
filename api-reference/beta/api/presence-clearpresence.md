---
title: 'присутствие: clearPresence'
description: Очистка сведений о присутствии для сеанса присутствия приложения пользователя.
author: jsandoval-msft
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 984c7667ceb2a28de189230952e5333f273cce24
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208264"
---
# <a name="presence-clearpresence"></a><span data-ttu-id="ef3a6-103">присутствие: clearPresence</span><span class="sxs-lookup"><span data-stu-id="ef3a6-103">presence: clearPresence</span></span>

<span data-ttu-id="ef3a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef3a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef3a6-105">Очистить сеанс присутствия приложения для пользователя.</span><span class="sxs-lookup"><span data-stu-id="ef3a6-105">Clear the application's presence session for a user.</span></span> <span data-ttu-id="ef3a6-106">Если это единственный сеанс присутствия пользователя, его присутствие изменится на `Offline/Offline` .</span><span class="sxs-lookup"><span data-stu-id="ef3a6-106">If it is the user's only presence session, the user's presence will change to `Offline/Offline`.</span></span>

<span data-ttu-id="ef3a6-107">Сведения о сеансах присутствия см. в материале [presence: setPresence.](presence-setpresence.md#presence-sessions)</span><span class="sxs-lookup"><span data-stu-id="ef3a6-107">For details about presences sessions, see [presence: setPresence](presence-setpresence.md#presence-sessions).</span></span>

## <a name="permissions"></a><span data-ttu-id="ef3a6-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ef3a6-108">Permissions</span></span>
<span data-ttu-id="ef3a6-109">Для вызова API требуется следующее разрешение.</span><span class="sxs-lookup"><span data-stu-id="ef3a6-109">The following permission is required to call the API.</span></span> <span data-ttu-id="ef3a6-110">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ef3a6-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ef3a6-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ef3a6-111">Permission type</span></span>                        | <span data-ttu-id="ef3a6-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ef3a6-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="ef3a6-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ef3a6-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="ef3a6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef3a6-114">Not Supported.</span></span>                              |
| <span data-ttu-id="ef3a6-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ef3a6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ef3a6-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ef3a6-116">Not Supported.</span></span>                              |
| <span data-ttu-id="ef3a6-117">Приложение</span><span class="sxs-lookup"><span data-stu-id="ef3a6-117">Application</span></span>                            | <span data-ttu-id="ef3a6-118">Presence.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef3a6-118">Presence.ReadWrite.All</span></span>                      |

## <a name="http-request"></a><span data-ttu-id="ef3a6-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ef3a6-119">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{userId}/presence/clearPresence
```

## <a name="request-headers"></a><span data-ttu-id="ef3a6-120">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="ef3a6-120">Request headers</span></span>
| <span data-ttu-id="ef3a6-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ef3a6-121">Name</span></span>          | <span data-ttu-id="ef3a6-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ef3a6-122">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="ef3a6-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ef3a6-123">Authorization</span></span> | <span data-ttu-id="ef3a6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef3a6-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="ef3a6-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ef3a6-126">Content-Type</span></span>  | <span data-ttu-id="ef3a6-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ef3a6-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ef3a6-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ef3a6-129">Request body</span></span>

<span data-ttu-id="ef3a6-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ef3a6-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ef3a6-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="ef3a6-131">Parameter</span></span> | <span data-ttu-id="ef3a6-132">Тип</span><span class="sxs-lookup"><span data-stu-id="ef3a6-132">Type</span></span>   | <span data-ttu-id="ef3a6-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ef3a6-133">Description</span></span>                                   |
| :-------- | :----- | :-------------------------------------------- |
| <span data-ttu-id="ef3a6-134">sessionId</span><span class="sxs-lookup"><span data-stu-id="ef3a6-134">sessionId</span></span> | <span data-ttu-id="ef3a6-135">строка</span><span class="sxs-lookup"><span data-stu-id="ef3a6-135">string</span></span> | <span data-ttu-id="ef3a6-136">ID сеанса присутствия приложения.</span><span class="sxs-lookup"><span data-stu-id="ef3a6-136">The ID of the application's presence session.</span></span> |


> [!IMPORTANT]
> 
> <span data-ttu-id="ef3a6-137">Предоставление ID приложения, как `sessionId` и в запросе.</span><span class="sxs-lookup"><span data-stu-id="ef3a6-137">Provide the ID of the application as `sessionId` in the request.</span></span>

## <a name="response"></a><span data-ttu-id="ef3a6-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef3a6-138">Response</span></span>
<span data-ttu-id="ef3a6-139">В случае успешного выполнения этот метод возвращает код отклика `200 OK`.</span><span class="sxs-lookup"><span data-stu-id="ef3a6-139">If successful, this method returns a `200 OK` response code.</span></span>

<span data-ttu-id="ef3a6-140">Если сеанс присутствия не существует, этот метод возвращает код `404 NotFound` ответа.</span><span class="sxs-lookup"><span data-stu-id="ef3a6-140">If the presence session doesn't exist, this method returns a `404 NotFound` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="ef3a6-141">Примеры</span><span class="sxs-lookup"><span data-stu-id="ef3a6-141">Examples</span></span>
<span data-ttu-id="ef3a6-142">В следующем запросе показано приложение с ИД, которое очищает `22553876-f5ab-4529-bffb-cfe50aa89f87` сеанс присутствия для `fa8bf3dc-eca7-46b7-bad1-db199b62afc3` пользователя.</span><span class="sxs-lookup"><span data-stu-id="ef3a6-142">The following request shows the application with ID `22553876-f5ab-4529-bffb-cfe50aa89f87` that clears its presence session for user `fa8bf3dc-eca7-46b7-bad1-db199b62afc3`.</span></span>

### <a name="request"></a><span data-ttu-id="ef3a6-143">Запрос</span><span class="sxs-lookup"><span data-stu-id="ef3a6-143">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ef3a6-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="ef3a6-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "clear--presence"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/users/fa8bf3dc-eca7-46b7-bad1-db199b62afc3/presence/clearPresence
Content-Type: application/json

{
  "sessionId": "22553876-f5ab-4529-bffb-cfe50aa89f87"
}
```
# <a name="c"></a>[<span data-ttu-id="ef3a6-145">C#</span><span class="sxs-lookup"><span data-stu-id="ef3a6-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/clear--presence-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ef3a6-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ef3a6-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/clear--presence-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ef3a6-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ef3a6-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/clear--presence-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ef3a6-148">Java</span><span class="sxs-lookup"><span data-stu-id="ef3a6-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/clear--presence-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ef3a6-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="ef3a6-149">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
