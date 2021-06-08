---
title: 'openShiftChangeRequest: утверждение'
description: Утверждение запроса openshift.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 769665c9a65229d33e287fcf7660157c5aa0b425
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52785958"
---
# <a name="openshiftchangerequest-approve"></a><span data-ttu-id="6b7b3-103">openShiftChangeRequest: утверждение</span><span class="sxs-lookup"><span data-stu-id="6b7b3-103">openShiftChangeRequest: approve</span></span>

<span data-ttu-id="6b7b3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b7b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b7b3-105">Утверждение [объекта openshiftchangerequest.](../resources/openshiftchangerequest.md)</span><span class="sxs-lookup"><span data-stu-id="6b7b3-105">Approve an [openshiftchangerequest](../resources/openshiftchangerequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b7b3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6b7b3-106">Permissions</span></span>

<span data-ttu-id="6b7b3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b7b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6b7b3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6b7b3-109">Permission type</span></span>                        | <span data-ttu-id="6b7b3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6b7b3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6b7b3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6b7b3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6b7b3-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b7b3-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="6b7b3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6b7b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b7b3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b7b3-114">Not supported.</span></span> |
| <span data-ttu-id="6b7b3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6b7b3-115">Application</span></span>                            | <span data-ttu-id="6b7b3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6b7b3-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b7b3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6b7b3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/approve
```

## <a name="request-headers"></a><span data-ttu-id="6b7b3-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6b7b3-118">Request headers</span></span>

| <span data-ttu-id="6b7b3-119">Имя</span><span class="sxs-lookup"><span data-stu-id="6b7b3-119">Name</span></span>          | <span data-ttu-id="6b7b3-120">Описание</span><span class="sxs-lookup"><span data-stu-id="6b7b3-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6b7b3-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6b7b3-121">Authorization</span></span> | <span data-ttu-id="6b7b3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b7b3-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6b7b3-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6b7b3-124">Content-type</span></span> | <span data-ttu-id="6b7b3-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6b7b3-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b7b3-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="6b7b3-127">Request body</span></span>

<span data-ttu-id="6b7b3-128">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="6b7b3-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6b7b3-129">Параметр</span><span class="sxs-lookup"><span data-stu-id="6b7b3-129">Parameter</span></span>    | <span data-ttu-id="6b7b3-130">Тип</span><span class="sxs-lookup"><span data-stu-id="6b7b3-130">Type</span></span>        | <span data-ttu-id="6b7b3-131">Описание</span><span class="sxs-lookup"><span data-stu-id="6b7b3-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6b7b3-132">message</span><span class="sxs-lookup"><span data-stu-id="6b7b3-132">message</span></span>|<span data-ttu-id="6b7b3-133">String</span><span class="sxs-lookup"><span data-stu-id="6b7b3-133">String</span></span>|<span data-ttu-id="6b7b3-134">Пользовательское сообщение утверждения.</span><span class="sxs-lookup"><span data-stu-id="6b7b3-134">A custom approval message.</span></span>|

## <a name="response"></a><span data-ttu-id="6b7b3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b7b3-135">Response</span></span>

<span data-ttu-id="6b7b3-p104">При успешном выполнении этот метод возвращает код отклика `200 OK`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="6b7b3-p104">If successful, this method returns a `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6b7b3-138">Примеры</span><span class="sxs-lookup"><span data-stu-id="6b7b3-138">Examples</span></span>

<span data-ttu-id="6b7b3-139">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="6b7b3-139">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="6b7b3-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="6b7b3-140">Request</span></span>

<span data-ttu-id="6b7b3-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6b7b3-141">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6b7b3-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b7b3-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "openshiftchangerequest_approve"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/approve
Content-type: application/json

{
  "message": "message-value"
}
```
# <a name="c"></a>[<span data-ttu-id="6b7b3-143">C#</span><span class="sxs-lookup"><span data-stu-id="6b7b3-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/openshiftchangerequest-approve-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b7b3-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b7b3-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/openshiftchangerequest-approve-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b7b3-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b7b3-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/openshiftchangerequest-approve-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b7b3-146">Java</span><span class="sxs-lookup"><span data-stu-id="6b7b3-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/openshiftchangerequest-approve-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6b7b3-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="6b7b3-147">Response</span></span>

<span data-ttu-id="6b7b3-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6b7b3-148">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 200 OK
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openShiftChangeRequest: approve",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


