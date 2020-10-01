---
title: 'Оффершифтрекуест: утверждение'
description: Утверждение объекта Оффершифтрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3b881d2d5efa166241147654f6dc3cc3c8b874a4
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48313683"
---
# <a name="offershiftrequest-approve"></a><span data-ttu-id="14f07-103">Оффершифтрекуест: утверждение</span><span class="sxs-lookup"><span data-stu-id="14f07-103">offerShiftRequest: approve</span></span>

<span data-ttu-id="14f07-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14f07-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="14f07-105">Утверждение объекта [оффершифтрекуест](../resources/offershiftrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="14f07-105">Approve an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="14f07-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="14f07-106">Permissions</span></span>

<span data-ttu-id="14f07-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="14f07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="14f07-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="14f07-109">Permission type</span></span>                        | <span data-ttu-id="14f07-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="14f07-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="14f07-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="14f07-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="14f07-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="14f07-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="14f07-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="14f07-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="14f07-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="14f07-114">Not supported.</span></span> |
| <span data-ttu-id="14f07-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="14f07-115">Application</span></span>                            | <span data-ttu-id="14f07-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14f07-116">Schedule.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="14f07-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="14f07-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="14f07-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="14f07-118">Request headers</span></span>

| <span data-ttu-id="14f07-119">Имя</span><span class="sxs-lookup"><span data-stu-id="14f07-119">Name</span></span>          | <span data-ttu-id="14f07-120">Описание</span><span class="sxs-lookup"><span data-stu-id="14f07-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="14f07-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="14f07-121">Authorization</span></span> | <span data-ttu-id="14f07-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14f07-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="14f07-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="14f07-124">Content-type</span></span> | <span data-ttu-id="14f07-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="14f07-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="14f07-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="14f07-127">Request body</span></span>

<span data-ttu-id="14f07-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="14f07-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="14f07-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="14f07-129">Parameter</span></span>    | <span data-ttu-id="14f07-130">Тип</span><span class="sxs-lookup"><span data-stu-id="14f07-130">Type</span></span>        | <span data-ttu-id="14f07-131">Описание</span><span class="sxs-lookup"><span data-stu-id="14f07-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="14f07-132">message</span><span class="sxs-lookup"><span data-stu-id="14f07-132">message</span></span>|<span data-ttu-id="14f07-133">String</span><span class="sxs-lookup"><span data-stu-id="14f07-133">String</span></span>|<span data-ttu-id="14f07-134">Пользовательское сообщение отправлено при утверждении.</span><span class="sxs-lookup"><span data-stu-id="14f07-134">Custom message sent on approval.</span></span>|

## <a name="response"></a><span data-ttu-id="14f07-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="14f07-135">Response</span></span>

<span data-ttu-id="14f07-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="14f07-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="14f07-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="14f07-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="14f07-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="14f07-139">Request</span></span>

<span data-ttu-id="14f07-140">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="14f07-140">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="14f07-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="14f07-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "offershiftrequest_approve"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/approve
Content-type: application/json

{
  "message": "Approved!"
}
```
# <a name="c"></a>[<span data-ttu-id="14f07-142">C#</span><span class="sxs-lookup"><span data-stu-id="14f07-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/offershiftrequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="14f07-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="14f07-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="14f07-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="14f07-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/offershiftrequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="14f07-145">Java</span><span class="sxs-lookup"><span data-stu-id="14f07-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/offershiftrequest-approve-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="14f07-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="14f07-146">Response</span></span>

<span data-ttu-id="14f07-147">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="14f07-147">The following example shows the response.</span></span>
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
  "description": "offerShiftRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

