---
title: 'Тимеоффрекуест: утверждение'
description: Утверждение тимеоффрекуест ".
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 631461eba5bab8f15bc392d59e9800f1b65be5a3
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895805"
---
# <a name="timeoffrequest-approve"></a><span data-ttu-id="f5d7e-103">Тимеоффрекуест: утверждение</span><span class="sxs-lookup"><span data-stu-id="f5d7e-103">timeOffRequest: approve</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5d7e-104">Утверждение [тимеоффрекуест](../resources/timeoffrequest.md).</span><span class="sxs-lookup"><span data-stu-id="f5d7e-104">Approve a [timeoffrequest](../resources/timeoffrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f5d7e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f5d7e-105">Permissions</span></span>

<span data-ttu-id="f5d7e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5d7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f5d7e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f5d7e-108">Permission type</span></span>                        | <span data-ttu-id="f5d7e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f5d7e-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f5d7e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f5d7e-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="f5d7e-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5d7e-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="f5d7e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f5d7e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5d7e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5d7e-113">Not supported.</span></span> |
| <span data-ttu-id="f5d7e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f5d7e-114">Application</span></span>                            | <span data-ttu-id="f5d7e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f5d7e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5d7e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f5d7e-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/timeOffRequests/approve
```

## <a name="request-headers"></a><span data-ttu-id="f5d7e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f5d7e-117">Request headers</span></span>

| <span data-ttu-id="f5d7e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="f5d7e-118">Name</span></span>          | <span data-ttu-id="f5d7e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="f5d7e-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="f5d7e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f5d7e-120">Authorization</span></span> | <span data-ttu-id="f5d7e-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="f5d7e-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f5d7e-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f5d7e-122">Request body</span></span>

<span data-ttu-id="f5d7e-123">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="f5d7e-123">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f5d7e-124">Параметр</span><span class="sxs-lookup"><span data-stu-id="f5d7e-124">Parameter</span></span>    | <span data-ttu-id="f5d7e-125">Тип</span><span class="sxs-lookup"><span data-stu-id="f5d7e-125">Type</span></span>        | <span data-ttu-id="f5d7e-126">Описание</span><span class="sxs-lookup"><span data-stu-id="f5d7e-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f5d7e-127">message</span><span class="sxs-lookup"><span data-stu-id="f5d7e-127">message</span></span>|<span data-ttu-id="f5d7e-128">String</span><span class="sxs-lookup"><span data-stu-id="f5d7e-128">String</span></span>|<span data-ttu-id="f5d7e-129">Настраиваемое сообщение утверждения.</span><span class="sxs-lookup"><span data-stu-id="f5d7e-129">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="f5d7e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5d7e-130">Response</span></span>

<span data-ttu-id="f5d7e-p102">В случае успешного выполнения этот метод возвращает код отклика `200, OK`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="f5d7e-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f5d7e-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="f5d7e-133">Examples</span></span>

<span data-ttu-id="f5d7e-134">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="f5d7e-134">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="f5d7e-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="f5d7e-135">Request</span></span>

<span data-ttu-id="f5d7e-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f5d7e-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/timeOffRequests/approve
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="f5d7e-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f5d7e-137">Response</span></span>

<span data-ttu-id="f5d7e-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="f5d7e-138">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "timeOffRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
