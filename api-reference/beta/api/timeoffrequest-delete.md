---
title: Удаление Тимеоффрекуест
description: Удаление объекта Тимеоффрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f185c8a9e4c3d0b3bb4f8286e0c4f7252e13692e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981353"
---
# <a name="delete-timeoffrequest"></a><span data-ttu-id="cff3b-103">Удаление Тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="cff3b-103">Delete timeOffRequest</span></span>

<span data-ttu-id="cff3b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cff3b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cff3b-105">Удаление объекта [тимеоффрекуест](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="cff3b-105">Delete a [timeOffRequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cff3b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cff3b-106">Permissions</span></span>

<span data-ttu-id="cff3b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cff3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cff3b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cff3b-109">Permission type</span></span>                        | <span data-ttu-id="cff3b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cff3b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cff3b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cff3b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="cff3b-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cff3b-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="cff3b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cff3b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cff3b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cff3b-114">Not supported.</span></span> |
|<span data-ttu-id="cff3b-115">Для приложения</span><span class="sxs-lookup"><span data-stu-id="cff3b-115">Application</span></span> | <span data-ttu-id="cff3b-116">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="cff3b-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="cff3b-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="cff3b-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="cff3b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cff3b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="cff3b-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cff3b-119">Request headers</span></span>

| <span data-ttu-id="cff3b-120">Имя</span><span class="sxs-lookup"><span data-stu-id="cff3b-120">Name</span></span>          | <span data-ttu-id="cff3b-121">Описание</span><span class="sxs-lookup"><span data-stu-id="cff3b-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="cff3b-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cff3b-122">Authorization</span></span> | <span data-ttu-id="cff3b-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cff3b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cff3b-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cff3b-125">Request body</span></span>

<span data-ttu-id="cff3b-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cff3b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cff3b-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="cff3b-127">Response</span></span>

<span data-ttu-id="cff3b-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="cff3b-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cff3b-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="cff3b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cff3b-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cff3b-131">Request</span></span>

<span data-ttu-id="cff3b-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cff3b-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cff3b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="cff3b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_timeoffrequest"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="cff3b-134">C#</span><span class="sxs-lookup"><span data-stu-id="cff3b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cff3b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cff3b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cff3b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cff3b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cff3b-137">Java</span><span class="sxs-lookup"><span data-stu-id="cff3b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-timeoffrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cff3b-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="cff3b-138">Response</span></span>

<span data-ttu-id="cff3b-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="cff3b-139">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete timeOffRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


