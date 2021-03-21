---
title: Список timeOffRequest
description: Извлечение списка объектов timeOffRequest в команде.
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7e04fb8dba357328247434fb0bfb63598a96fde9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963551"
---
# <a name="list-timeoffrequest"></a><span data-ttu-id="ce77f-103">Список timeOffRequest</span><span class="sxs-lookup"><span data-stu-id="ce77f-103">List timeOffRequest</span></span>

<span data-ttu-id="ce77f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce77f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ce77f-105">Извлечение списка [объектов timeOffRequest](../resources/timeoffrequest.md) в команде.</span><span class="sxs-lookup"><span data-stu-id="ce77f-105">Retrieve a list of [timeOffRequest](../resources/timeoffrequest.md) objects in the team.</span></span>

## <a name="permissions"></a><span data-ttu-id="ce77f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ce77f-106">Permissions</span></span>

<span data-ttu-id="ce77f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ce77f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ce77f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ce77f-109">Permission type</span></span>                        | <span data-ttu-id="ce77f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ce77f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
|<span data-ttu-id="ce77f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ce77f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ce77f-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce77f-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ce77f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ce77f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ce77f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce77f-114">Not supported.</span></span>    |
|<span data-ttu-id="ce77f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ce77f-115">Application</span></span> | <span data-ttu-id="ce77f-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce77f-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="ce77f-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="ce77f-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ce77f-118">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="ce77f-118">Global admins can access groups that they are not a member of.</span></span> <span data-ttu-id="ce77f-119">в настоящее время только в закрытом предварительном просмотре и недоступны для общего пользования.</span><span class="sxs-lookup"><span data-stu-id="ce77f-119">currently in private preview only and are not available for public use.</span></span>

## <a name="http-request"></a><span data-ttu-id="ce77f-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ce77f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timeOffRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ce77f-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="ce77f-121">Optional query parameters</span></span>

<span data-ttu-id="ce77f-122">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="ce77f-122">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="ce77f-123">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="ce77f-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ce77f-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ce77f-124">Request headers</span></span>

| <span data-ttu-id="ce77f-125">Имя</span><span class="sxs-lookup"><span data-stu-id="ce77f-125">Name</span></span>      |<span data-ttu-id="ce77f-126">Описание</span><span class="sxs-lookup"><span data-stu-id="ce77f-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ce77f-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ce77f-127">Authorization</span></span> | <span data-ttu-id="ce77f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ce77f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ce77f-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ce77f-130">Request body</span></span>

<span data-ttu-id="ce77f-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ce77f-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ce77f-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce77f-132">Response</span></span>

<span data-ttu-id="ce77f-133">В случае успешной работы этот метод возвращает код ответа и запрашиваемую `200 OK` [объекты timeOffRequest](../resources/timeoffrequest.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ce77f-133">If successful, this method returns a `200 OK` response code and the requested [timeOffRequest](../resources/timeoffrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ce77f-134">Примеры</span><span class="sxs-lookup"><span data-stu-id="ce77f-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ce77f-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ce77f-135">Request</span></span>

<span data-ttu-id="ce77f-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ce77f-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="ce77f-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ce77f-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_timeoffrequest_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffRequests
```
# <a name="c"></a>[<span data-ttu-id="ce77f-138">C#</span><span class="sxs-lookup"><span data-stu-id="ce77f-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-timeoffrequest-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ce77f-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ce77f-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-timeoffrequest-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ce77f-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ce77f-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-timeoffrequest-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ce77f-141">Java</span><span class="sxs-lookup"><span data-stu-id="ce77f-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-timeoffrequest-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---

### <a name="response"></a><span data-ttu-id="ce77f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="ce77f-142">Response</span></span>

<span data-ttu-id="ce77f-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ce77f-143">The following is an example of the response.</span></span>

> <span data-ttu-id="ce77f-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ce77f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

