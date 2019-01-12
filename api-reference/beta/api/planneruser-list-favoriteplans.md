---
title: Список favoritePlans
description: Получение списка plannerPlans, помеченные как избранные пользователем. План в Избранное можно пометить, изменив plannerUser ресурсов.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: 15938b2ed3acc9a944d775dc19211745c52ca2fa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931316"
---
# <a name="list-favoriteplans"></a><span data-ttu-id="926a1-104">Список favoritePlans</span><span class="sxs-lookup"><span data-stu-id="926a1-104">List favoritePlans</span></span>

> <span data-ttu-id="926a1-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="926a1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="926a1-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="926a1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="926a1-107">Получение списка [plannerPlans](../resources/plannerplan.md) , помеченные как избранные пользователем.</span><span class="sxs-lookup"><span data-stu-id="926a1-107">Retrieve a list of [plannerPlans](../resources/plannerplan.md) that are marked as favorite by a user.</span></span> <span data-ttu-id="926a1-108">План в Избранное можно пометить, [изменив plannerUser ресурсов](planneruser-update.md).</span><span class="sxs-lookup"><span data-stu-id="926a1-108">You can mark a plan as favorite by [updating the plannerUser resource](planneruser-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="926a1-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="926a1-109">Permissions</span></span>
<span data-ttu-id="926a1-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="926a1-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="926a1-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="926a1-112">Permission type</span></span>      | <span data-ttu-id="926a1-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="926a1-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="926a1-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="926a1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="926a1-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="926a1-115">Group.Read.All</span></span>    |
|<span data-ttu-id="926a1-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="926a1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="926a1-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="926a1-117">Not supported.</span></span>    |
|<span data-ttu-id="926a1-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="926a1-118">Application</span></span> | <span data-ttu-id="926a1-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="926a1-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="926a1-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="926a1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/favoritePlans
GET /users/<id>/planner/favoritePlans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="926a1-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="926a1-121">Optional query parameters</span></span>
<span data-ttu-id="926a1-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="926a1-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="926a1-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="926a1-123">Request headers</span></span>
| <span data-ttu-id="926a1-124">Имя</span><span class="sxs-lookup"><span data-stu-id="926a1-124">Name</span></span>      |<span data-ttu-id="926a1-125">Описание</span><span class="sxs-lookup"><span data-stu-id="926a1-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="926a1-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="926a1-126">Authorization</span></span>  | <span data-ttu-id="926a1-p105">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="926a1-p105">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="926a1-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="926a1-129">Request body</span></span>
<span data-ttu-id="926a1-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="926a1-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="926a1-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="926a1-131">Response</span></span>
<span data-ttu-id="926a1-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [plannerPlan](../resources/plannerplan.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="926a1-132">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="926a1-133">Пример</span><span class="sxs-lookup"><span data-stu-id="926a1-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="926a1-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="926a1-134">Request</span></span>
<span data-ttu-id="926a1-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="926a1-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_favoriteplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/favoritePlans
```
##### <a name="response"></a><span data-ttu-id="926a1-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="926a1-136">Response</span></span>
<span data-ttu-id="926a1-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="926a1-137">The following is an example of the response.</span></span> 

><span data-ttu-id="926a1-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="926a1-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtUGxhbiAgQEBAQEBAQEBAQEBAQEBDXCc=\"",
      "createdBy": {
        "user": {
          "id": "dd8a8379-1ac1-4eee-861d-ec15f6fa3611"
        },
        "application": {
          "id": "09abbdfd-ed23-44ee-a2d9-a627aa1c90f3"
        }
      },
      "createdDateTime": "2015-10-14T00:57:28.4698344Z",
      "owner": "eacd01dd-84cc-4c12-bd8a-9a33e5aeed11",
      "title": "Budget Planning (2016)",
      "id": "uZWtCtli30CGoWLIWSat1mQAC0ai"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List favoritePlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
