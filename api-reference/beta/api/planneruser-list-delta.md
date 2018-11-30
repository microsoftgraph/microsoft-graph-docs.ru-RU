---
title: 'Планировщик работы: дельты'
description: Извлекает изменения объектов, на которые подписан пользователь.
ms.openlocfilehash: 7c866946f0c9a873b99ee4efd6d9e2c7ce646be3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080160"
---
# <a name="planner-delta"></a><span data-ttu-id="d7f5a-103">Планировщик работы: дельты</span><span class="sxs-lookup"><span data-stu-id="d7f5a-103">Planner: delta</span></span>

> <span data-ttu-id="d7f5a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7f5a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d7f5a-106">Извлекает изменения объектов, которые пользователь является [на рассылку](../resources/planner-overview.md#track-changes-using-delta-query) .</span><span class="sxs-lookup"><span data-stu-id="d7f5a-106">Retrieves changes to objects that the user is [subscribed](../resources/planner-overview.md#track-changes-using-delta-query) to.</span></span>

<span data-ttu-id="d7f5a-107">Этот метод позволяет приложению для отслеживания изменений объектов, которые пользователь может получить доступ из в пределах планировщик работы со временем.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-107">This method allows your application to track changes to objects that the user can access from within Planner over time.</span></span>

<span data-ttu-id="d7f5a-108">Возвращаемое значение этого метода может содержать гетерогенной типы объектов из планировщика.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-108">The return value of this method might contain hetergenous types of objects from Planner.</span></span>

<span data-ttu-id="d7f5a-109">Дополнительные сведения о отслеживание изменений в данных Microsoft Graph можно [запроса дельты используется для отслеживания изменений в данных Microsoft Graph](/graph/delta-query-overview).</span><span class="sxs-lookup"><span data-stu-id="d7f5a-109">For more information about tracking changes in Microsoft Graph data, see [Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="d7f5a-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d7f5a-110">Permissions</span></span>

<span data-ttu-id="d7f5a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d7f5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7f5a-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d7f5a-113">Permission type</span></span>      | <span data-ttu-id="d7f5a-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d7f5a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7f5a-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d7f5a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="d7f5a-116">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7f5a-116">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d7f5a-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d7f5a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7f5a-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-118">Not supported.</span></span>    |
|<span data-ttu-id="d7f5a-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d7f5a-119">Application</span></span> | <span data-ttu-id="d7f5a-120">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7f5a-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d7f5a-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/planner/all/delta
GET /users/<id>/planner/all/delta
```

<span data-ttu-id="d7f5a-122">Без параметров дополнительных запросов (например, `$select`, `$expand`, или `$filter`) в настоящее время поддерживаются на планировщик работы по реализации дельты запросов.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-122">No additional query parameters (such as `$select`, `$expand`, or `$filter`) are currently supported on Planner's implementation of delta queries.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7f5a-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d7f5a-123">Request headers</span></span>

| <span data-ttu-id="d7f5a-124">Имя</span><span class="sxs-lookup"><span data-stu-id="d7f5a-124">Name</span></span>           |<span data-ttu-id="d7f5a-125">Описание</span><span class="sxs-lookup"><span data-stu-id="d7f5a-125">Description</span></span>                |
|:---------------|:--------------------------|
| <span data-ttu-id="d7f5a-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d7f5a-126">Authorization</span></span>  | <span data-ttu-id="d7f5a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7f5a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d7f5a-129">Request body</span></span>

<span data-ttu-id="d7f5a-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7f5a-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7f5a-131">Response</span></span>

<span data-ttu-id="d7f5a-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию изменения, примененные к объектам в основной части ответа и следуйте ссылку разностная синхронизация.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-132">If successful, this method returns a `200 OK` response code and a collection of changes to be applied to objects in the response body, and a Delta Sync link to follow.</span></span>

<span data-ttu-id="d7f5a-133">Если `deltaLink` неверно сформированные использует вызывающего абонента, эту конечную точку возвращает HTTP 400.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-133">If the `deltaLink` that the caller uses is malformed, this endpoint will return HTTP 400.</span></span>

<span data-ttu-id="d7f5a-134">Если `deltaLink` слишком старый использует вызывающего абонента, возвращает HTTP 410 эту конечную точку.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-134">If the `deltaLink` that the caller uses is too old, this endpoint will return HTTP 410.</span></span>

<span data-ttu-id="d7f5a-p104">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="d7f5a-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="d7f5a-138">Пример</span><span class="sxs-lookup"><span data-stu-id="d7f5a-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d7f5a-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="d7f5a-139">Request</span></span>

<span data-ttu-id="d7f5a-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-140">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_delta"
}-->

```http
GET https://graph.microsoft.com/beta/me/planner/all/delta
```

##### <a name="response"></a><span data-ttu-id="d7f5a-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="d7f5a-141">Response</span></span>
<span data-ttu-id="d7f5a-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-142">Here is an example of the response.</span></span>

><span data-ttu-id="d7f5a-143">**Примечание:** Объект ответа может сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-143">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="d7f5a-144">Будут возвращены все измененные свойства из фактический вызов.</span><span class="sxs-lookup"><span data-stu-id="d7f5a-144">All the changed properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List changes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
