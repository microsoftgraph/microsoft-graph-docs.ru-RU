---
title: 'Свапшифтсчанжерекуест: отклонить'
description: Отклонить запрос на замену.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 4814fb3ef9d416d6d3bc5be1815b746277a25426
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846186"
---
# <a name="swapshiftschangerequest-decline"></a><span data-ttu-id="b5e20-103">Свапшифтсчанжерекуест: отклонить</span><span class="sxs-lookup"><span data-stu-id="b5e20-103">swapShiftsChangeRequest: decline</span></span>

<span data-ttu-id="b5e20-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5e20-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b5e20-105">Отклонить объект [свапшифтсчанжерекуест](../resources/swapshiftschangerequest.md) .</span><span class="sxs-lookup"><span data-stu-id="b5e20-105">Decline a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5e20-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b5e20-106">Permissions</span></span>

<span data-ttu-id="b5e20-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5e20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5e20-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b5e20-109">Permission type</span></span>                        | <span data-ttu-id="b5e20-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b5e20-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b5e20-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b5e20-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5e20-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="b5e20-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="b5e20-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b5e20-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5e20-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b5e20-114">Not supported.</span></span>                              |
| <span data-ttu-id="b5e20-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b5e20-115">Application</span></span>                            | <span data-ttu-id="b5e20-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5e20-116">Schedule.ReadWrite.All</span></span>                      |

> <span data-ttu-id="b5e20-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="b5e20-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b5e20-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="b5e20-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b5e20-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b5e20-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="b5e20-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b5e20-120">Request headers</span></span>

| <span data-ttu-id="b5e20-121">Имя</span><span class="sxs-lookup"><span data-stu-id="b5e20-121">Name</span></span>          | <span data-ttu-id="b5e20-122">Описание</span><span class="sxs-lookup"><span data-stu-id="b5e20-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b5e20-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b5e20-123">Authorization</span></span> | <span data-ttu-id="b5e20-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5e20-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b5e20-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b5e20-126">Content-type</span></span> | <span data-ttu-id="b5e20-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b5e20-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5e20-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b5e20-129">Request body</span></span>

<span data-ttu-id="b5e20-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b5e20-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b5e20-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="b5e20-131">Parameter</span></span>    | <span data-ttu-id="b5e20-132">Тип</span><span class="sxs-lookup"><span data-stu-id="b5e20-132">Type</span></span>        | <span data-ttu-id="b5e20-133">Описание</span><span class="sxs-lookup"><span data-stu-id="b5e20-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b5e20-134">message</span><span class="sxs-lookup"><span data-stu-id="b5e20-134">message</span></span>|<span data-ttu-id="b5e20-135">String</span><span class="sxs-lookup"><span data-stu-id="b5e20-135">String</span></span>|<span data-ttu-id="b5e20-136">Настраиваемое сообщение об отклонении.</span><span class="sxs-lookup"><span data-stu-id="b5e20-136">A custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="b5e20-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5e20-137">Response</span></span>

<span data-ttu-id="b5e20-p105">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b5e20-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b5e20-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="b5e20-140">Examples</span></span>

<span data-ttu-id="b5e20-141">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="b5e20-141">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="b5e20-142">Запрос</span><span class="sxs-lookup"><span data-stu-id="b5e20-142">Request</span></span>

<span data-ttu-id="b5e20-143">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b5e20-143">The following is an example of a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b5e20-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5e20-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "swapshiftchangerequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="b5e20-145">C#</span><span class="sxs-lookup"><span data-stu-id="b5e20-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/swapshiftchangerequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5e20-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5e20-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/swapshiftchangerequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5e20-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5e20-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/swapshiftchangerequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5e20-148">Java</span><span class="sxs-lookup"><span data-stu-id="b5e20-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/swapshiftchangerequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="b5e20-149">Отклик</span><span class="sxs-lookup"><span data-stu-id="b5e20-149">Response</span></span>

<span data-ttu-id="b5e20-150">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b5e20-150">The following is an example of the response.</span></span>
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
