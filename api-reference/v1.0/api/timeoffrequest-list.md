---
title: Список timeOffRequest
description: Извлечение списка объектов timeOffRequest в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8784cacb090a1c5a877cc7d4aa1142c50661cfa9
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053792"
---
# <a name="list-timeoffrequest"></a><span data-ttu-id="acf15-103">Список timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="acf15-103">List timeOffRequest</span></span>

<span data-ttu-id="acf15-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acf15-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="acf15-105">Извлечение списка [объектов timeOffRequest](../resources/timeoffrequest.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="acf15-105">Retrieve a list of [timeOffRequest](../resources/timeoffrequest.md) objects in the team.</span></span>

## <a name="permissions"></a><span data-ttu-id="acf15-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="acf15-106">Permissions</span></span>

<span data-ttu-id="acf15-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acf15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="acf15-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="acf15-109">Permission type</span></span>                        | <span data-ttu-id="acf15-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="acf15-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="acf15-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="acf15-111">Delegated (work or school account)</span></span> | <span data-ttu-id="acf15-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acf15-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="acf15-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="acf15-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acf15-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acf15-114">Not supported.</span></span>    |
|<span data-ttu-id="acf15-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="acf15-115">Application</span></span> | <span data-ttu-id="acf15-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acf15-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="acf15-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="acf15-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="acf15-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="acf15-118">Global admins can access groups that they are not a member of.</span></span> <span data-ttu-id="acf15-119">в настоящее время только в закрытом предварительном просмотре и недоступны для общего пользования.</span><span class="sxs-lookup"><span data-stu-id="acf15-119">currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="acf15-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="acf15-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="acf15-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="acf15-121">Optional query parameters</span></span>

<span data-ttu-id="acf15-122">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="acf15-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="acf15-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="acf15-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="acf15-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="acf15-124">Request headers</span></span>

| <span data-ttu-id="acf15-125">Имя</span><span class="sxs-lookup"><span data-stu-id="acf15-125">Name</span></span>      |<span data-ttu-id="acf15-126">Описание</span><span class="sxs-lookup"><span data-stu-id="acf15-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="acf15-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="acf15-127">Authorization</span></span> | <span data-ttu-id="acf15-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="acf15-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="acf15-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="acf15-130">Request body</span></span>

<span data-ttu-id="acf15-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="acf15-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acf15-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="acf15-132">Response</span></span>

<span data-ttu-id="acf15-133">В случае успешной работы этот метод возвращает код ответа и запрашиваемую `200 OK` [объекты timeOffRequest](../resources/timeoffrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="acf15-133">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="acf15-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="acf15-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="acf15-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="acf15-135">Request</span></span>

<span data-ttu-id="acf15-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="acf15-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="acf15-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="acf15-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests
```
# <a name="c"></a>[<span data-ttu-id="acf15-138">C#</span><span class="sxs-lookup"><span data-stu-id="acf15-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="acf15-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="acf15-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="acf15-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="acf15-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="acf15-141">Java</span><span class="sxs-lookup"><span data-stu-id="acf15-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-timeoffrequest-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="acf15-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="acf15-142">Response</span></span>

<span data-ttu-id="acf15-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="acf15-143">The following is an example of the response.</span></span>

> <span data-ttu-id="acf15-144">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="acf15-144">**Note:** The response object shown here might be shortened for readability.</span></span>

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

