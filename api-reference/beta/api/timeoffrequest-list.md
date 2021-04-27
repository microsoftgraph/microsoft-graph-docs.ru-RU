---
title: Список timeOffRequests
description: Извлечение списка объектов timeOffRequest в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5741a1852dfc7d5a048da7ed8fdea873bd6ce9c5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048934"
---
# <a name="list-timeoffrequest"></a><span data-ttu-id="d52ba-103">Список timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="d52ba-103">List timeOffRequest</span></span>

<span data-ttu-id="d52ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d52ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d52ba-105">Извлечение списка [объектов timeoffrequest](../resources/timeoffrequest.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="d52ba-105">Retrieve a list of [timeoffrequest](../resources/timeoffrequest.md) objects in the team.</span></span>

## <a name="permissions"></a><span data-ttu-id="d52ba-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d52ba-106">Permissions</span></span>

<span data-ttu-id="d52ba-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d52ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d52ba-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d52ba-109">Permission type</span></span>                        | <span data-ttu-id="d52ba-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d52ba-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="d52ba-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d52ba-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d52ba-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d52ba-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d52ba-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d52ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d52ba-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d52ba-114">Not supported.</span></span>    |
|<span data-ttu-id="d52ba-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="d52ba-115">Application</span></span> | <span data-ttu-id="d52ba-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="d52ba-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="d52ba-117">\***Важно:** Разрешения приложения в настоящее время доступны только в закрытом режиме и недоступны для общего пользования.</span><span class="sxs-lookup"><span data-stu-id="d52ba-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="d52ba-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="d52ba-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d52ba-119">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="d52ba-119">Global admins can access groups that they are not a member of.</span></span> 

## <a name="http-request"></a><span data-ttu-id="d52ba-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d52ba-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d52ba-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="d52ba-121">Optional query parameters</span></span>

<span data-ttu-id="d52ba-122">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="d52ba-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="d52ba-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d52ba-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="d52ba-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d52ba-124">Request headers</span></span>

| <span data-ttu-id="d52ba-125">Имя</span><span class="sxs-lookup"><span data-stu-id="d52ba-125">Name</span></span>      |<span data-ttu-id="d52ba-126">Описание</span><span class="sxs-lookup"><span data-stu-id="d52ba-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d52ba-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d52ba-127">Authorization</span></span> | <span data-ttu-id="d52ba-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d52ba-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d52ba-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d52ba-130">Request body</span></span>

<span data-ttu-id="d52ba-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d52ba-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d52ba-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="d52ba-132">Response</span></span>

<span data-ttu-id="d52ba-133">В случае успешной работы этот метод возвращает код ответа и запрашиваемую `200 OK` [объекты timeOffRequest](../resources/timeoffrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d52ba-133">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d52ba-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="d52ba-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d52ba-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="d52ba-135">Request</span></span>

<span data-ttu-id="d52ba-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d52ba-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d52ba-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="d52ba-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffRequests
```
# <a name="c"></a>[<span data-ttu-id="d52ba-138">C#</span><span class="sxs-lookup"><span data-stu-id="d52ba-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d52ba-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d52ba-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d52ba-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d52ba-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d52ba-141">Java</span><span class="sxs-lookup"><span data-stu-id="d52ba-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-timeoffrequest-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="d52ba-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="d52ba-142">Response</span></span>

<span data-ttu-id="d52ba-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d52ba-143">The following is an example of the response.</span></span>

> <span data-ttu-id="d52ba-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d52ba-144">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOffRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
        {
        "id": "0b87dd20-d5ed-4764-9c3e-cfc8516def09",
        "startDateTime": "datetime-value",
        "endDateTime": "datetime-value",
        "timeOffReasonId": "timeOffReasonId-value"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List timeOffRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


