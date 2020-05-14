---
title: 'Тимеоффрекуест: утверждение'
description: Утверждение объекта тимеоффрекуест. "
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 84e0d6ef33cd63acb283806f994ca108873f0d0f
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217936"
---
# <a name="timeoffrequest-approve"></a><span data-ttu-id="35dcf-103">Тимеоффрекуест: утверждение</span><span class="sxs-lookup"><span data-stu-id="35dcf-103">timeOffRequest: approve</span></span>

<span data-ttu-id="35dcf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35dcf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="35dcf-105">Утверждение [тимеоффрекуест](../resources/timeoffrequest.md).</span><span class="sxs-lookup"><span data-stu-id="35dcf-105">Approve a [timeoffrequest](../resources/timeoffrequest.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="35dcf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="35dcf-106">Permissions</span></span>

<span data-ttu-id="35dcf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35dcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="35dcf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="35dcf-109">Permission type</span></span>                        | <span data-ttu-id="35dcf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="35dcf-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="35dcf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="35dcf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="35dcf-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="35dcf-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="35dcf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="35dcf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35dcf-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35dcf-114">Not supported.</span></span>    |
|<span data-ttu-id="35dcf-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="35dcf-115">Application</span></span> | <span data-ttu-id="35dcf-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35dcf-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="35dcf-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="35dcf-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="35dcf-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="35dcf-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="35dcf-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="35dcf-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="35dcf-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="35dcf-120">Request headers</span></span>

| <span data-ttu-id="35dcf-121">Имя</span><span class="sxs-lookup"><span data-stu-id="35dcf-121">Name</span></span>          | <span data-ttu-id="35dcf-122">Описание</span><span class="sxs-lookup"><span data-stu-id="35dcf-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="35dcf-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="35dcf-123">Authorization</span></span> | <span data-ttu-id="35dcf-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35dcf-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="35dcf-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="35dcf-126">Content-type</span></span> | <span data-ttu-id="35dcf-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="35dcf-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35dcf-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="35dcf-129">Request body</span></span>

<span data-ttu-id="35dcf-130">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="35dcf-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="35dcf-131">Параметр</span><span class="sxs-lookup"><span data-stu-id="35dcf-131">Parameter</span></span>    | <span data-ttu-id="35dcf-132">Тип</span><span class="sxs-lookup"><span data-stu-id="35dcf-132">Type</span></span>        | <span data-ttu-id="35dcf-133">Описание</span><span class="sxs-lookup"><span data-stu-id="35dcf-133">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="35dcf-134">message</span><span class="sxs-lookup"><span data-stu-id="35dcf-134">message</span></span>|<span data-ttu-id="35dcf-135">String</span><span class="sxs-lookup"><span data-stu-id="35dcf-135">String</span></span>|<span data-ttu-id="35dcf-136">Настраиваемое сообщение утверждения.</span><span class="sxs-lookup"><span data-stu-id="35dcf-136">Custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="35dcf-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="35dcf-137">Response</span></span>

<span data-ttu-id="35dcf-p105">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="35dcf-p105">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="35dcf-140">Примеры</span><span class="sxs-lookup"><span data-stu-id="35dcf-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="35dcf-141">Запрос</span><span class="sxs-lookup"><span data-stu-id="35dcf-141">Request</span></span>

<span data-ttu-id="35dcf-142">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="35dcf-142">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="35dcf-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="35dcf-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffrequest_approve"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="35dcf-144">C#</span><span class="sxs-lookup"><span data-stu-id="35dcf-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffrequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35dcf-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35dcf-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffrequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35dcf-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35dcf-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffrequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="35dcf-147">Java</span><span class="sxs-lookup"><span data-stu-id="35dcf-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffrequest-approve-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="35dcf-148">Ответ</span><span class="sxs-lookup"><span data-stu-id="35dcf-148">Response</span></span>

<span data-ttu-id="35dcf-149">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="35dcf-149">The following is an example of the response.</span></span>
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
