---
title: 'Свапшифтсчанжерекуест: отклонить'
description: Отклонить запрос на замену.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 35d7d9d83dc32d7598815ed8d98e7f6f828d8b1f
ms.sourcegitcommit: 31a9b4cb3d0f905f123475a4c1a86f5b1e59b935
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2020
ms.locfileid: "42219795"
---
# <a name="swapshiftschangerequest-decline"></a><span data-ttu-id="ffafc-103">Свапшифтсчанжерекуест: отклонить</span><span class="sxs-lookup"><span data-stu-id="ffafc-103">swapShiftsChangeRequest: decline</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffafc-104">Отклонить объект [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="ffafc-104">Decline a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ffafc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ffafc-105">Permissions</span></span>

<span data-ttu-id="ffafc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ffafc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ffafc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ffafc-108">Permission type</span></span>                        | <span data-ttu-id="ffafc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ffafc-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="ffafc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ffafc-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="ffafc-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffafc-111">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="ffafc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ffafc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffafc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffafc-113">Not supported.</span></span> |
| <span data-ttu-id="ffafc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ffafc-114">Application</span></span>                            | <span data-ttu-id="ffafc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ffafc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ffafc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ffafc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="ffafc-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ffafc-117">Request headers</span></span>

| <span data-ttu-id="ffafc-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ffafc-118">Name</span></span>          | <span data-ttu-id="ffafc-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ffafc-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ffafc-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ffafc-120">Authorization</span></span> | <span data-ttu-id="ffafc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffafc-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ffafc-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ffafc-123">Content-type</span></span> | <span data-ttu-id="ffafc-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ffafc-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ffafc-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ffafc-126">Request body</span></span>

<span data-ttu-id="ffafc-127">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="ffafc-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="ffafc-128">Параметр</span><span class="sxs-lookup"><span data-stu-id="ffafc-128">Parameter</span></span>    | <span data-ttu-id="ffafc-129">Тип</span><span class="sxs-lookup"><span data-stu-id="ffafc-129">Type</span></span>        | <span data-ttu-id="ffafc-130">Описание</span><span class="sxs-lookup"><span data-stu-id="ffafc-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ffafc-131">message</span><span class="sxs-lookup"><span data-stu-id="ffafc-131">message</span></span>|<span data-ttu-id="ffafc-132">String</span><span class="sxs-lookup"><span data-stu-id="ffafc-132">String</span></span>|<span data-ttu-id="ffafc-133">Настраиваемое сообщение об отклонении.</span><span class="sxs-lookup"><span data-stu-id="ffafc-133">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="ffafc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffafc-134">Response</span></span>

<span data-ttu-id="ffafc-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ffafc-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ffafc-137">Примеры</span><span class="sxs-lookup"><span data-stu-id="ffafc-137">Examples</span></span>

<span data-ttu-id="ffafc-138">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="ffafc-138">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="ffafc-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="ffafc-139">Request</span></span>

<span data-ttu-id="ffafc-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ffafc-140">The following is an example of a request.</span></span>
<!-- {
  "blockType": "request",
  "name": "swapshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```

### <a name="response"></a><span data-ttu-id="ffafc-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ffafc-141">Response</span></span>

<span data-ttu-id="ffafc-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ffafc-142">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 NO CONTENT
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "swapShiftChangeRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
