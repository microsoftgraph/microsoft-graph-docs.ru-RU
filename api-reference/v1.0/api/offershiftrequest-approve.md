---
title: 'offerShiftRequest: утверждение'
description: Утверждение объекта offerShiftRequest.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 370e9399b7f4848209190fb771128a51ac820501
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788080"
---
# <a name="offershiftrequest-approve"></a><span data-ttu-id="8cd9f-103">offerShiftRequest: утверждение</span><span class="sxs-lookup"><span data-stu-id="8cd9f-103">offerShiftRequest: approve</span></span>

<span data-ttu-id="8cd9f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cd9f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8cd9f-105">Утверждение [объекта offerShiftRequest.](../resources/offershiftrequest.md)</span><span class="sxs-lookup"><span data-stu-id="8cd9f-105">Approve an [offerShiftRequest](../resources/offershiftrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cd9f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8cd9f-106">Permissions</span></span>

<span data-ttu-id="8cd9f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8cd9f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8cd9f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8cd9f-109">Permission type</span></span>                        | <span data-ttu-id="8cd9f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8cd9f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8cd9f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8cd9f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8cd9f-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cd9f-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span> |
| <span data-ttu-id="8cd9f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8cd9f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cd9f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8cd9f-114">Not supported.</span></span> |
| <span data-ttu-id="8cd9f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8cd9f-115">Application</span></span>                            | <span data-ttu-id="8cd9f-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cd9f-116">Schedule.ReadWrite.All</span></span> |


## <a name="http-request"></a><span data-ttu-id="8cd9f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8cd9f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="8cd9f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8cd9f-118">Request headers</span></span>

| <span data-ttu-id="8cd9f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="8cd9f-119">Name</span></span>          | <span data-ttu-id="8cd9f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="8cd9f-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8cd9f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8cd9f-121">Authorization</span></span> | <span data-ttu-id="8cd9f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8cd9f-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="8cd9f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8cd9f-124">Content-type</span></span> | <span data-ttu-id="8cd9f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8cd9f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cd9f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8cd9f-127">Request body</span></span>

<span data-ttu-id="8cd9f-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="8cd9f-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="8cd9f-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="8cd9f-129">Parameter</span></span>    | <span data-ttu-id="8cd9f-130">Тип</span><span class="sxs-lookup"><span data-stu-id="8cd9f-130">Type</span></span>        | <span data-ttu-id="8cd9f-131">Описание</span><span class="sxs-lookup"><span data-stu-id="8cd9f-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8cd9f-132">message</span><span class="sxs-lookup"><span data-stu-id="8cd9f-132">message</span></span>|<span data-ttu-id="8cd9f-133">String</span><span class="sxs-lookup"><span data-stu-id="8cd9f-133">String</span></span>|<span data-ttu-id="8cd9f-134">Настраиваемые сообщения, отправленные на утверждение.</span><span class="sxs-lookup"><span data-stu-id="8cd9f-134">Custom message sent on approval.</span></span>|

## <a name="response"></a><span data-ttu-id="8cd9f-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cd9f-135">Response</span></span>

<span data-ttu-id="8cd9f-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="8cd9f-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8cd9f-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="8cd9f-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8cd9f-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="8cd9f-139">Request</span></span>

<span data-ttu-id="8cd9f-140">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8cd9f-140">The following example shows a request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8cd9f-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="8cd9f-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="8cd9f-142">C#</span><span class="sxs-lookup"><span data-stu-id="8cd9f-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/offershiftrequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8cd9f-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8cd9f-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/offershiftrequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8cd9f-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8cd9f-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/offershiftrequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="8cd9f-145">Java</span><span class="sxs-lookup"><span data-stu-id="8cd9f-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/offershiftrequest-approve-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="8cd9f-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="8cd9f-146">Response</span></span>

<span data-ttu-id="8cd9f-147">Ниже приводится пример отклика.</span><span class="sxs-lookup"><span data-stu-id="8cd9f-147">The following example shows the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
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

