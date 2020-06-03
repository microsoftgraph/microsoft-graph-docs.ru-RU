---
title: 'Тимеоффрекуест: отклонить'
description: Отклонить объект тимеоффрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9d893dcf8f5557fa650b5eb1eefd8b00704874ee
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44215929"
---
# <a name="timeoffrequest-decline"></a><span data-ttu-id="03593-103">Тимеоффрекуест: отклонить</span><span class="sxs-lookup"><span data-stu-id="03593-103">timeOffRequest: decline</span></span>

<span data-ttu-id="03593-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03593-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="03593-105">Отклонить объект [тимеоффрекуест](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="03593-105">Decline a [timeoffrequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="03593-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="03593-106">Permissions</span></span>

<span data-ttu-id="03593-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03593-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="03593-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="03593-109">Permission type</span></span>                        | <span data-ttu-id="03593-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="03593-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="03593-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="03593-111">Delegated (work or school account)</span></span> | <span data-ttu-id="03593-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="03593-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="03593-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="03593-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03593-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="03593-114">Not supported.</span></span>    |
|<span data-ttu-id="03593-115">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="03593-115">Application</span></span> | <span data-ttu-id="03593-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03593-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="03593-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="03593-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="03593-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="03593-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="03593-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="03593-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
```

## <a name="request-headers"></a><span data-ttu-id="03593-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="03593-120">Request headers</span></span>

| <span data-ttu-id="03593-121">Имя</span><span class="sxs-lookup"><span data-stu-id="03593-121">Name</span></span>          | <span data-ttu-id="03593-122">Описание</span><span class="sxs-lookup"><span data-stu-id="03593-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="03593-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="03593-123">Authorization</span></span> | <span data-ttu-id="03593-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="03593-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03593-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="03593-126">Content-type</span></span> | <span data-ttu-id="03593-127">приложение — JSON.</span><span class="sxs-lookup"><span data-stu-id="03593-127">application-json.</span></span> <span data-ttu-id="03593-128">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="03593-128">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="03593-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="03593-129">Request body</span></span>

<span data-ttu-id="03593-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="03593-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="03593-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="03593-131">Parameter</span></span>    | <span data-ttu-id="03593-132">Тип</span><span class="sxs-lookup"><span data-stu-id="03593-132">Type</span></span>        | <span data-ttu-id="03593-133">Описание</span><span class="sxs-lookup"><span data-stu-id="03593-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="03593-134">message</span><span class="sxs-lookup"><span data-stu-id="03593-134">message</span></span>|<span data-ttu-id="03593-135">String</span><span class="sxs-lookup"><span data-stu-id="03593-135">String</span></span>|<span data-ttu-id="03593-136">Настраиваемое сообщение об отклонении.</span><span class="sxs-lookup"><span data-stu-id="03593-136">Custom decline message.</span></span>|

## <a name="response"></a><span data-ttu-id="03593-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="03593-137">Response</span></span>

<span data-ttu-id="03593-p105">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="03593-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="03593-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="03593-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="03593-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="03593-141">Request</span></span>

<span data-ttu-id="03593-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="03593-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="03593-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="03593-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_decline"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="03593-144">C#</span><span class="sxs-lookup"><span data-stu-id="03593-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffrequest-decline-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03593-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03593-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-decline-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03593-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03593-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-decline-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="03593-147">Java</span><span class="sxs-lookup"><span data-stu-id="03593-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffrequest-decline-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="03593-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="03593-148">Response</span></span>

<span data-ttu-id="03593-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="03593-149">The following is an example of the response.</span></span>
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
  "description": "timeOffRequest: decline",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
