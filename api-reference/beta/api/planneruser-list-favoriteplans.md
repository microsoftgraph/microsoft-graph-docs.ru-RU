---
title: Список favoritePlans
description: Получение списка plannerPlans, помеченные как избранные пользователем. План в Избранное можно пометить, изменив plannerUser ресурсов.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: c189b3a3a7ed6d36272c05e9614fd6d0327600d4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519124"
---
# <a name="list-favoriteplans"></a><span data-ttu-id="67657-104">Список favoritePlans</span><span class="sxs-lookup"><span data-stu-id="67657-104">List favoritePlans</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67657-105">Получение списка [plannerPlans](../resources/plannerplan.md) , помеченные как избранные пользователем.</span><span class="sxs-lookup"><span data-stu-id="67657-105">Retrieve a list of [plannerPlans](../resources/plannerplan.md) that are marked as favorite by a user.</span></span> <span data-ttu-id="67657-106">План в Избранное можно пометить, [изменив plannerUser ресурсов](planneruser-update.md).</span><span class="sxs-lookup"><span data-stu-id="67657-106">You can mark a plan as favorite by [updating the plannerUser resource](planneruser-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="67657-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67657-107">Permissions</span></span>
<span data-ttu-id="67657-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67657-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67657-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67657-110">Permission type</span></span>      | <span data-ttu-id="67657-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67657-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67657-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67657-112">Delegated (work or school account)</span></span> | <span data-ttu-id="67657-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="67657-113">Group.Read.All</span></span>    |
|<span data-ttu-id="67657-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67657-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67657-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67657-115">Not supported.</span></span>    |
|<span data-ttu-id="67657-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67657-116">Application</span></span> | <span data-ttu-id="67657-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67657-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="67657-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67657-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/favoritePlans
GET /users/<id>/planner/favoritePlans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="67657-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="67657-119">Optional query parameters</span></span>
<span data-ttu-id="67657-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="67657-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="67657-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67657-121">Request headers</span></span>
| <span data-ttu-id="67657-122">Имя</span><span class="sxs-lookup"><span data-stu-id="67657-122">Name</span></span>      |<span data-ttu-id="67657-123">Описание</span><span class="sxs-lookup"><span data-stu-id="67657-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="67657-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="67657-124">Authorization</span></span>  | <span data-ttu-id="67657-p104">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67657-p104">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="67657-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="67657-127">Request body</span></span>
<span data-ttu-id="67657-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="67657-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="67657-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="67657-129">Response</span></span>
<span data-ttu-id="67657-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [plannerPlan](../resources/plannerplan.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="67657-130">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="67657-131">Пример</span><span class="sxs-lookup"><span data-stu-id="67657-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67657-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="67657-132">Request</span></span>
<span data-ttu-id="67657-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67657-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_favoriteplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/favoritePlans
```
##### <a name="response"></a><span data-ttu-id="67657-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="67657-134">Response</span></span>
<span data-ttu-id="67657-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="67657-135">The following is an example of the response.</span></span> 

><span data-ttu-id="67657-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67657-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List favoritePlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-list-favoriteplans.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
