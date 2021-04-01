---
title: 'Планировщик: дельта'
description: Извлекает изменения для объектов, на которые подписан пользователь.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 7c730630f3fd655db29c93c699e8090d3046a4d4
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473495"
---
# <a name="planner-delta"></a><span data-ttu-id="f2f6e-103">Планировщик: дельта</span><span class="sxs-lookup"><span data-stu-id="f2f6e-103">Planner: delta</span></span>

<span data-ttu-id="f2f6e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2f6e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2f6e-105">Извлекает изменения для объектов, на которые подписан [пользователь.](../resources/planner-overview.md#track-changes-using-delta-query)</span><span class="sxs-lookup"><span data-stu-id="f2f6e-105">Retrieves changes to objects that the user is [subscribed](../resources/planner-overview.md#track-changes-using-delta-query) to.</span></span>

<span data-ttu-id="f2f6e-106">Этот метод позволяет приложению отслеживать изменения в объектах, к которые пользователь может получить доступ в planner с течением времени.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-106">This method allows your application to track changes to objects that the user can access from within Planner over time.</span></span>

<span data-ttu-id="f2f6e-107">Возвращаемая стоимость этого метода может содержать гетегенные типы объектов из Planner.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-107">The return value of this method might contain hetergenous types of objects from Planner.</span></span>

<span data-ttu-id="f2f6e-108">Дополнительные сведения об отслеживании изменений в данных Microsoft Graph см. в дополнительных сведениях об использовании [delta-запроса](/graph/delta-query-overview)для отслеживания изменений в данных Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-108">For more information about tracking changes in Microsoft Graph data, see [Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="f2f6e-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f2f6e-109">Permissions</span></span>

<span data-ttu-id="f2f6e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f2f6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2f6e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f2f6e-112">Permission type</span></span>      | <span data-ttu-id="f2f6e-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f2f6e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2f6e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f2f6e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f2f6e-115">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2f6e-115">Tasks.Read, Tasks.ReadWrite, Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f2f6e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f2f6e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2f6e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-117">Not supported.</span></span>    |
|<span data-ttu-id="f2f6e-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f2f6e-118">Application</span></span> | <span data-ttu-id="f2f6e-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2f6e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f2f6e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/planner/all/delta
GET /users/{id}/planner/all/delta
```

<span data-ttu-id="f2f6e-121">Дополнительные параметры запроса (например, или ) в настоящее время не поддерживаются при выполнении планировщиком запросов `$select` `$expand` `$filter` дельты.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-121">No additional query parameters (such as `$select`, `$expand`, or `$filter`) are currently supported on Planner's implementation of delta queries.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f2f6e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f2f6e-122">Request headers</span></span>

| <span data-ttu-id="f2f6e-123">Имя</span><span class="sxs-lookup"><span data-stu-id="f2f6e-123">Name</span></span>           |<span data-ttu-id="f2f6e-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f2f6e-124">Description</span></span>                |
|:---------------|:--------------------------|
| <span data-ttu-id="f2f6e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f2f6e-125">Authorization</span></span>  | <span data-ttu-id="f2f6e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2f6e-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f2f6e-128">Request body</span></span>

<span data-ttu-id="f2f6e-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f2f6e-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2f6e-130">Response</span></span>

<span data-ttu-id="f2f6e-131">В случае успешной работы этот метод возвращает код отклика и коллекцию изменений, которые будут применены к объектам в тексте отклика, а также ссылку `200 OK` на синхронизацию delta.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-131">If successful, this method returns a `200 OK` response code and a collection of changes to be applied to objects in the response body, and a Delta Sync link to follow.</span></span>

<span data-ttu-id="f2f6e-132">Если используется недоставка вызываемой точки, эта конечная точка `deltaLink` возвращает HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-132">If the `deltaLink` that the caller uses is malformed, this endpoint will return HTTP 400.</span></span>

<span data-ttu-id="f2f6e-133">Если `deltaLink` используется слишком старый вызов, эта конечная точка возвращает HTTP 410.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-133">If the `deltaLink` that the caller uses is too old, this endpoint will return HTTP 410.</span></span>

<span data-ttu-id="f2f6e-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="f2f6e-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="f2f6e-137">Пример</span><span class="sxs-lookup"><span data-stu-id="f2f6e-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f2f6e-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="f2f6e-138">Request</span></span>

<span data-ttu-id="f2f6e-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-139">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f2f6e-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2f6e-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/planner/all/delta
```
# <a name="c"></a>[<span data-ttu-id="f2f6e-141">C#</span><span class="sxs-lookup"><span data-stu-id="f2f6e-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2f6e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2f6e-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2f6e-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2f6e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2f6e-144">Java</span><span class="sxs-lookup"><span data-stu-id="f2f6e-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f2f6e-145">Отклик</span><span class="sxs-lookup"><span data-stu-id="f2f6e-145">Response</span></span>
<span data-ttu-id="f2f6e-146">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-146">Here is an example of the response.</span></span>

><span data-ttu-id="f2f6e-147">**Примечание.** Показанный объект ответа может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-147">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="f2f6e-148">Все измененные свойства будут возвращены с фактического вызова.</span><span class="sxs-lookup"><span data-stu-id="f2f6e-148">All the changed properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_delta",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.entity)",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
cache-control: private
client-request-id: 3acb384b-e2d1-4a46-a347-e03bc6428cac
request-id: 3acb384b-e2d1-4a46-a347-e03bc6428cac
preference-applied: odata.track-changes, odata.track-changes

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.plannerDelta)",
    "@odata.deltaLink": "https://graph.microsoft.com/beta/me/planner/all/delta?$deltatoken=jVztGMFnm7qLEQ69FaXzWF5sPEJZU2YxZa32QEvnZTZ4q4C10ThM5uL7bEPm9ysqrxOY0QQIb4Uqmc9DH3rn7pczamvtCipDVJ4FivXh398.J9pSVKpytlutvx03-iBmO4ZM_3qPztOq2T9VIjHoRR0",
    "value": [
        {
            "@odata.type": "#microsoft.graph.plannerTask",
            "@odata.etag": "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBASCc=\"",
            "percentComplete": 100,
            "completedDateTime": "2018-03-13T21:31:25.778Z",
            "completedBy": {
                "user": {
                    "id": "8414b634-316f-41ba-b6a6-646a2949e3a5"
                }
            },
            "id": "5pNWKnX2XUalCKa64-oiXJUAPT1v",
            "@odata.context": "https://graph.microsoft.com/beta/$metadata#planner/tasks/$entity"
        },
        {
            "@odata.type": "#microsoft.graph.plannerTask",
            "@odata.etag": "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBATCc=\"",
            "percentComplete": 0,
            "completedDateTime": null,
            "completedBy": null,
            "id": "5pNWKnX2XUalCKa64-oiXJUAPT1v",
            "@odata.context": "https://graph.microsoft.com/beta/$metadata#planner/tasks/$entity"
        },
        {
            "@odata.type": "#microsoft.graph.plannerTask",
            "@odata.etag": "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAUCc=\"",
            "title": "Title change",
            "id": "5pNWKnX2XUalCKa64-oiXJUAPT1v",
            "@odata.context": "https://graph.microsoft.com/beta/$metadata#planner/tasks/$entity"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List changes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


