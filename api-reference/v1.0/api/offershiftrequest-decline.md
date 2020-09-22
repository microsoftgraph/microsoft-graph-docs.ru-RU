---
title: 'Оффершифтрекуест: отклонить'
description: Отклонить запрос на смену предложения.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8368935da77d178c7e1165da4b9ac418a9016f0e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087147"
---
# <a name="offershiftrequest-decline"></a><span data-ttu-id="3a33a-103">Оффершифтрекуест: отклонить</span><span class="sxs-lookup"><span data-stu-id="3a33a-103">offerShiftRequest: decline</span></span>

<span data-ttu-id="3a33a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a33a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3a33a-105">Отклонить объект [оффершифтрекуест](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="3a33a-105">Decline an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3a33a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3a33a-106">Permissions</span></span>

<span data-ttu-id="3a33a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3a33a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3a33a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3a33a-109">Permission type</span></span>                        | <span data-ttu-id="3a33a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3a33a-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3a33a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3a33a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3a33a-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="3a33a-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="3a33a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3a33a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3a33a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3a33a-114">Not supported.</span></span> |
| <span data-ttu-id="3a33a-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="3a33a-115">Application</span></span>                            | <span data-ttu-id="3a33a-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a33a-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="3a33a-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="3a33a-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3a33a-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="3a33a-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3a33a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3a33a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="3a33a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3a33a-120">Request headers</span></span>

| <span data-ttu-id="3a33a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3a33a-121">Name</span></span>          | <span data-ttu-id="3a33a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3a33a-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="3a33a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3a33a-123">Authorization</span></span> | <span data-ttu-id="3a33a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a33a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3a33a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3a33a-126">Content-type</span></span> | <span data-ttu-id="3a33a-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3a33a-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3a33a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3a33a-129">Request body</span></span>

<span data-ttu-id="3a33a-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="3a33a-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3a33a-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="3a33a-131">Parameter</span></span>    | <span data-ttu-id="3a33a-132">Тип</span><span class="sxs-lookup"><span data-stu-id="3a33a-132">Type</span></span>        | <span data-ttu-id="3a33a-133">Описание</span><span class="sxs-lookup"><span data-stu-id="3a33a-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3a33a-134">message</span><span class="sxs-lookup"><span data-stu-id="3a33a-134">message</span></span>|<span data-ttu-id="3a33a-135">String</span><span class="sxs-lookup"><span data-stu-id="3a33a-135">String</span></span>|<span data-ttu-id="3a33a-136">Настраиваемое сообщение, отправленное при отклонении.</span><span class="sxs-lookup"><span data-stu-id="3a33a-136">Custom message sent on decline.</span></span>|

## <a name="response"></a><span data-ttu-id="3a33a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a33a-137">Response</span></span>

<span data-ttu-id="3a33a-p105">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3a33a-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3a33a-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="3a33a-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3a33a-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="3a33a-141">Request</span></span>

<span data-ttu-id="3a33a-142">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3a33a-142">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="3a33a-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="3a33a-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/decline
Content-type: application/json

{
  "message": "Sorry, you can't offer this shift."
}
```
# <a name="c"></a>[<span data-ttu-id="3a33a-144">C#</span><span class="sxs-lookup"><span data-stu-id="3a33a-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/offershiftrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3a33a-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3a33a-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3a33a-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3a33a-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/offershiftrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3a33a-147">Java</span><span class="sxs-lookup"><span data-stu-id="3a33a-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/offershiftrequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="3a33a-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="3a33a-148">Response</span></span>

<span data-ttu-id="3a33a-149">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3a33a-149">The following example shows the response.</span></span>
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
  "description": "offerShiftRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

