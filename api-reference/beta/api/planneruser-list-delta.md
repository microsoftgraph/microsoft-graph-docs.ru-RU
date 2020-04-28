---
title: 'Планировщик: Дельта'
description: Извлекает изменения объектов, на которые подписан пользователь.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 867aa4f2b143da1014c9485c0fac00872193e140
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455593"
---
# <a name="planner-delta"></a><span data-ttu-id="d8456-103">Планировщик: Дельта</span><span class="sxs-lookup"><span data-stu-id="d8456-103">Planner: delta</span></span>

<span data-ttu-id="d8456-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8456-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8456-105">Извлекает изменения объектов, на которые [подписан](../resources/planner-overview.md#track-changes-using-delta-query) пользователь.</span><span class="sxs-lookup"><span data-stu-id="d8456-105">Retrieves changes to objects that the user is [subscribed](../resources/planner-overview.md#track-changes-using-delta-query) to.</span></span>

<span data-ttu-id="d8456-106">Этот метод позволяет приложению отслеживать изменения объектов, к которым пользователь может получить доступ из планировщика, с течением времени.</span><span class="sxs-lookup"><span data-stu-id="d8456-106">This method allows your application to track changes to objects that the user can access from within Planner over time.</span></span>

<span data-ttu-id="d8456-107">Возвращаемое значение этого метода может содержать гетерогенной типы объектов из планировщика.</span><span class="sxs-lookup"><span data-stu-id="d8456-107">The return value of this method might contain hetergenous types of objects from Planner.</span></span>

<span data-ttu-id="d8456-108">Дополнительные сведения об отслеживании изменений в данных Microsoft Graph приведены в [статье Использование разностного запроса для отслеживания изменений в данных Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="d8456-108">For more information about tracking changes in Microsoft Graph data, see [Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="d8456-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d8456-109">Permissions</span></span>

<span data-ttu-id="d8456-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8456-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8456-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d8456-112">Permission type</span></span>      | <span data-ttu-id="d8456-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d8456-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8456-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d8456-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d8456-115">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8456-115">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d8456-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d8456-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8456-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8456-117">Not supported.</span></span>    |
|<span data-ttu-id="d8456-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d8456-118">Application</span></span> | <span data-ttu-id="d8456-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d8456-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8456-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d8456-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/planner/all/delta
GET /users/{id}/planner/all/delta
```

<span data-ttu-id="d8456-121">В настоящее время дополнительные параметры запросов ( `$select`например `$expand`,, `$filter`или) не поддерживаются в реализациях разностных запросов в планировщике.</span><span class="sxs-lookup"><span data-stu-id="d8456-121">No additional query parameters (such as `$select`, `$expand`, or `$filter`) are currently supported on Planner's implementation of delta queries.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d8456-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d8456-122">Request headers</span></span>

| <span data-ttu-id="d8456-123">Имя</span><span class="sxs-lookup"><span data-stu-id="d8456-123">Name</span></span>           |<span data-ttu-id="d8456-124">Описание</span><span class="sxs-lookup"><span data-stu-id="d8456-124">Description</span></span>                |
|:---------------|:--------------------------|
| <span data-ttu-id="d8456-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d8456-125">Authorization</span></span>  | <span data-ttu-id="d8456-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d8456-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8456-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d8456-128">Request body</span></span>

<span data-ttu-id="d8456-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d8456-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8456-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d8456-130">Response</span></span>

<span data-ttu-id="d8456-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию изменений, которые необходимо применить к объектам в тексте отклика, и ссылку на разностную синхронизацию, которую необходимо выполнить.</span><span class="sxs-lookup"><span data-stu-id="d8456-131">If successful, this method returns a `200 OK` response code and a collection of changes to be applied to objects in the response body, and a Delta Sync link to follow.</span></span>

<span data-ttu-id="d8456-132">`deltaLink` Если вызывающий абонент использует неправильный формат, эта конечная точка возвратит HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="d8456-132">If the `deltaLink` that the caller uses is malformed, this endpoint will return HTTP 400.</span></span>

<span data-ttu-id="d8456-133">Если абонент `deltaLink` использует слишком старое значение, эта конечная точка возвратит HTTP 410.</span><span class="sxs-lookup"><span data-stu-id="d8456-133">If the `deltaLink` that the caller uses is too old, this endpoint will return HTTP 410.</span></span>

<span data-ttu-id="d8456-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="d8456-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="d8456-137">Пример</span><span class="sxs-lookup"><span data-stu-id="d8456-137">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d8456-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="d8456-138">Request</span></span>

<span data-ttu-id="d8456-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d8456-139">Here is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d8456-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8456-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/planner/all/delta
```
# <a name="c"></a>[<span data-ttu-id="d8456-141">C#</span><span class="sxs-lookup"><span data-stu-id="d8456-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8456-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8456-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8456-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8456-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d8456-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="d8456-144">Response</span></span>
<span data-ttu-id="d8456-145">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d8456-145">Here is an example of the response.</span></span>

><span data-ttu-id="d8456-146">**Примечание.** Показанный объект ответа может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d8456-146">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="d8456-147">При фактическом вызове будут возвращены все измененные свойства.</span><span class="sxs-lookup"><span data-stu-id="d8456-147">All the changed properties will be returned from an actual call.</span></span>

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
