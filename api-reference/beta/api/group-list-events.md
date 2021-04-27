---
title: Список событий
description: Получение списка, включающего объекты событий.
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: cbdb6eff39e2e7139bf8c78ac739148fb7059794
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52041640"
---
# <a name="list-events"></a><span data-ttu-id="9c09f-103">Перечисление событий</span><span class="sxs-lookup"><span data-stu-id="9c09f-103">List events</span></span>

<span data-ttu-id="9c09f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c09f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c09f-105">Получение списка объектов [event](../resources/event.md).</span><span class="sxs-lookup"><span data-stu-id="9c09f-105">Retrieve a list of [event](../resources/event.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="9c09f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c09f-106">Permissions</span></span>
<span data-ttu-id="9c09f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c09f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c09f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c09f-109">Permission type</span></span>      | <span data-ttu-id="9c09f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c09f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c09f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c09f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9c09f-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c09f-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="9c09f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c09f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c09f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c09f-114">Not supported.</span></span>    |
|<span data-ttu-id="9c09f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c09f-115">Application</span></span> | <span data-ttu-id="9c09f-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9c09f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c09f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c09f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/events
GET /groups/{id}/calendar/events
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9c09f-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="9c09f-118">Optional query parameters</span></span>
<span data-ttu-id="9c09f-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="9c09f-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9c09f-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c09f-120">Request headers</span></span>
| <span data-ttu-id="9c09f-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9c09f-121">Name</span></span>       | <span data-ttu-id="9c09f-122">Тип</span><span class="sxs-lookup"><span data-stu-id="9c09f-122">Type</span></span> | <span data-ttu-id="9c09f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9c09f-123">Description</span></span> |
|:---------------|:--------|:--------|
| <span data-ttu-id="9c09f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c09f-124">Authorization</span></span>  | <span data-ttu-id="9c09f-125">string</span><span class="sxs-lookup"><span data-stu-id="9c09f-125">string</span></span> | <span data-ttu-id="9c09f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c09f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9c09f-128">Prefer: outlook.timezone</span><span class="sxs-lookup"><span data-stu-id="9c09f-128">Prefer: outlook.timezone</span></span>  | <span data-ttu-id="9c09f-129">string</span><span class="sxs-lookup"><span data-stu-id="9c09f-129">string</span></span> | <span data-ttu-id="9c09f-130">С помощью этого заголовка вы можете задать часовой пояс для времени начала и окончания в ответе.</span><span class="sxs-lookup"><span data-stu-id="9c09f-130">Use this to specify the time zone for start and end times in the response.</span></span> <span data-ttu-id="9c09f-131">Если он не задан, эти значения времени возвращаются в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="9c09f-131">If not specified, those time values are returned in UTC.</span></span> <span data-ttu-id="9c09f-132">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="9c09f-132">Optional.</span></span> |
| <span data-ttu-id="9c09f-133">Prefer: outlook.body-content-type</span><span class="sxs-lookup"><span data-stu-id="9c09f-133">Prefer: outlook.body-content-type</span></span> | <span data-ttu-id="9c09f-134">string</span><span class="sxs-lookup"><span data-stu-id="9c09f-134">string</span></span> | <span data-ttu-id="9c09f-135">Формат возвращаемого свойства **body**.</span><span class="sxs-lookup"><span data-stu-id="9c09f-135">The format of the **body** property to be returned in.</span></span> <span data-ttu-id="9c09f-136">Возможные значения: "text" или "html".</span><span class="sxs-lookup"><span data-stu-id="9c09f-136">Values can be "text" or "html".</span></span> <span data-ttu-id="9c09f-137">Заголовок `Preference-Applied` возвращается как подтверждение, если заголовок `Prefer` указан.</span><span class="sxs-lookup"><span data-stu-id="9c09f-137">A `Preference-Applied` header is returned as confirmation if this `Prefer` header is specified.</span></span> <span data-ttu-id="9c09f-138">Если заголовок не указан, свойство **body** возвращается в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="9c09f-138">If the header is not specified, the **body** property is returned in HTML format.</span></span> <span data-ttu-id="9c09f-139">Необязательное свойство.</span><span class="sxs-lookup"><span data-stu-id="9c09f-139">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c09f-140">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9c09f-140">Request body</span></span>
<span data-ttu-id="9c09f-141">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9c09f-141">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c09f-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c09f-142">Response</span></span>
<span data-ttu-id="9c09f-143">При успешном выполнении этот метод возвращает код отклика `200 OK` и коллекцию объектов [event](../resources/event.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9c09f-143">If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c09f-144">Пример</span><span class="sxs-lookup"><span data-stu-id="9c09f-144">Example</span></span>
#### <a name="request"></a><span data-ttu-id="9c09f-145">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c09f-145">Request</span></span>
<span data-ttu-id="9c09f-146">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c09f-146">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9c09f-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="9c09f-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_group_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/groups/{id}/events
```
# <a name="c"></a>[<span data-ttu-id="9c09f-148">C#</span><span class="sxs-lookup"><span data-stu-id="9c09f-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-group-events-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9c09f-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9c09f-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-group-events-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9c09f-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9c09f-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-group-events-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9c09f-151">Java</span><span class="sxs-lookup"><span data-stu-id="9c09f-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-group-events-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9c09f-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c09f-152">Response</span></span>
<span data-ttu-id="9c09f-153">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="9c09f-153">The following is an example of the response.</span></span>
><span data-ttu-id="9c09f-154">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="9c09f-154">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 354

{
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "",
        "time": "2016-10-19T10:37:00Z"
      },
      "uid": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List group events",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


