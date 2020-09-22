---
title: Удаление Тимеоффрекуест
description: Удаление объекта Тимеоффрекуест.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cd666d992c0ffc678a9dab26b5dfb1974fa12555
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010481"
---
# <a name="delete-timeoffrequest"></a><span data-ttu-id="85d8f-103">Удаление Тимеоффрекуест</span><span class="sxs-lookup"><span data-stu-id="85d8f-103">Delete timeOffRequest</span></span>

<span data-ttu-id="85d8f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85d8f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85d8f-105">Удаление объекта [тимеоффрекуест](../resources/timeoffrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="85d8f-105">Delete a [timeOffRequest](../resources/timeoffrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="85d8f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85d8f-106">Permissions</span></span>

<span data-ttu-id="85d8f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85d8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="85d8f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85d8f-109">Permission type</span></span>                        | <span data-ttu-id="85d8f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85d8f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="85d8f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85d8f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="85d8f-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85d8f-112">Group.ReadWrite.All</span></span> |
| <span data-ttu-id="85d8f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85d8f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85d8f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85d8f-114">Not supported.</span></span> |
|<span data-ttu-id="85d8f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="85d8f-115">Application</span></span> | <span data-ttu-id="85d8f-116">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="85d8f-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="85d8f-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="85d8f-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="85d8f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85d8f-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="85d8f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85d8f-119">Request headers</span></span>

| <span data-ttu-id="85d8f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="85d8f-120">Name</span></span>          | <span data-ttu-id="85d8f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="85d8f-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="85d8f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="85d8f-122">Authorization</span></span> | <span data-ttu-id="85d8f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="85d8f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="85d8f-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85d8f-125">Request body</span></span>

<span data-ttu-id="85d8f-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85d8f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85d8f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="85d8f-127">Response</span></span>

<span data-ttu-id="85d8f-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="85d8f-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="85d8f-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="85d8f-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="85d8f-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="85d8f-131">Request</span></span>

<span data-ttu-id="85d8f-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85d8f-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85d8f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="85d8f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_timeoffrequest"
}-->

```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}
```
# <a name="c"></a>[<span data-ttu-id="85d8f-134">C#</span><span class="sxs-lookup"><span data-stu-id="85d8f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-timeoffrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85d8f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85d8f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-timeoffrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85d8f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85d8f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-timeoffrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="85d8f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="85d8f-137">Response</span></span>

<span data-ttu-id="85d8f-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="85d8f-138">The following is an example of the response.</span></span>

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


