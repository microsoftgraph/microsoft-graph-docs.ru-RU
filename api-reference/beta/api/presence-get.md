---
title: Получение сведений о присутствии
description: Получение сведений о присутствии пользователя.
author: VinodRavichandran
localization_priority: Normal
doc_type: apiPageType
ms.prod: cloud-communications
ms.openlocfilehash: 3d1b56dc8266eea42c773596c8e78e9e0ece5b6b
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844185"
---
# <a name="get-presence"></a><span data-ttu-id="4786f-103">Получение сведений о присутствии</span><span class="sxs-lookup"><span data-stu-id="4786f-103">Get presence</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4786f-104">Получение сведений о [присутствии](../resources/presence.md) пользователя.</span><span class="sxs-lookup"><span data-stu-id="4786f-104">Get a user's [presence](../resources/presence.md) information.</span></span>

## <a name="permissions"></a><span data-ttu-id="4786f-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4786f-105">Permissions</span></span>
<span data-ttu-id="4786f-106">Для вызова этих API требуется одно из следующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="4786f-106">One of the following permissions is required to call these APIs.</span></span> <span data-ttu-id="4786f-107">Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4786f-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4786f-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4786f-108">Permission type</span></span> | <span data-ttu-id="4786f-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4786f-109">Permissions (from least to most privileged)</span></span>                  |
| :-------------- | :----------------------------------------------------------- |
| <span data-ttu-id="4786f-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4786f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="4786f-111">Присутствие. Read, присутствие. Read. ALL</span><span class="sxs-lookup"><span data-stu-id="4786f-111">Presence.Read, Presence.Read.All</span></span>                         |
| <span data-ttu-id="4786f-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4786f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4786f-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4786f-113">Not Supported.</span></span>                         |
| <span data-ttu-id="4786f-114">Application</span><span class="sxs-lookup"><span data-stu-id="4786f-114">Application</span></span>                            | <span data-ttu-id="4786f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4786f-115">Not Supported.</span></span>                                  |

## <a name="http-requests"></a><span data-ttu-id="4786f-116">HTTP-запросы</span><span class="sxs-lookup"><span data-stu-id="4786f-116">HTTP Requests</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/presence
GET /users/{id}/presence
```

## <a name="request-headers"></a><span data-ttu-id="4786f-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4786f-117">Request Headers</span></span>
| <span data-ttu-id="4786f-118">Имя</span><span class="sxs-lookup"><span data-stu-id="4786f-118">Name</span></span>          | <span data-ttu-id="4786f-119">Описание</span><span class="sxs-lookup"><span data-stu-id="4786f-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="4786f-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="4786f-120">Authorization</span></span> | <span data-ttu-id="4786f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4786f-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="4786f-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4786f-123">Request body</span></span>

<span data-ttu-id="4786f-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="4786f-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4786f-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="4786f-125">Response</span></span>
<span data-ttu-id="4786f-126">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [присутствия](../resources/presence.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="4786f-126">If successful, this method returns a `200 OK` response code and a [presence](../resources/presence.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4786f-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="4786f-127">Examples</span></span>

### <a name="example-1-get-your-own-presence-information"></a><span data-ttu-id="4786f-128">Пример 1: получение собственных сведений о присутствии</span><span class="sxs-lookup"><span data-stu-id="4786f-128">Example 1: Get your own presence information</span></span>

<span data-ttu-id="4786f-129">В приведенном ниже примере показано, как получить сведения о присутствии.</span><span class="sxs-lookup"><span data-stu-id="4786f-129">The following example shows how to get your own presence information.</span></span> <span data-ttu-id="4786f-130">Для выполнения этой операции требуется разрешение на присутствие. чтение.</span><span class="sxs-lookup"><span data-stu-id="4786f-130">This operation requires the Presence.Read permission.</span></span>

#### <a name="request"></a><span data-ttu-id="4786f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="4786f-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get-your-presence"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/presence
```

#### <a name="response"></a><span data-ttu-id="4786f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="4786f-132">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-your-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{  
    "id": "fa8bf3dc-eca7-46b7-bad1-db199b62afc3",
    "availability": "Available",
    "activity": "Available"
}
```

### <a name="example-2-get-the-presence-information-of-another-user"></a><span data-ttu-id="4786f-133">Пример 2: получение сведений о присутствии другого пользователя</span><span class="sxs-lookup"><span data-stu-id="4786f-133">Example 2: Get the presence information of another user</span></span>

<span data-ttu-id="4786f-134">В приведенном ниже примере показано, как получить сведения о присутствии для другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="4786f-134">The following example shows how to get the presence information for another user.</span></span> <span data-ttu-id="4786f-135">Для выполнения этой операции требуется разрешение на присутствие. Read. ALL.</span><span class="sxs-lookup"><span data-stu-id="4786f-135">This operation requires the Presence.Read.All permission.</span></span>

#### <a name="request"></a><span data-ttu-id="4786f-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="4786f-136">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get-user-presence"
}-->
```http
GET https://graph.microsoft.com/beta/users/66825e03-7ef5-42da-9069-724602c31f6b/presence
```

#### <a name="response"></a><span data-ttu-id="4786f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4786f-137">Response</span></span>

<!-- {
  "blockType": "response",
  "name": "get-user-presence",
  "@odata.type": "microsoft.graph.presence",
  "truncated":"true"
}-->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

{
    "id": "66825e03-7ef5-42da-9069-724602c31f6b",
    "availability": "DoNotDisturb",
    "activity": "Presenting"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Presence",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
