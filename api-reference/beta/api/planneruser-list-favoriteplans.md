---
title: Список Фаворитепланс
description: Получение списка планов, помеченных пользователем как избранный. Вы можете пометить план как избранный, обновив ресурс plannerUser.
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: c189b3a3a7ed6d36272c05e9614fd6d0327600d4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538724"
---
# <a name="list-favoriteplans"></a><span data-ttu-id="2419f-104">Список Фаворитепланс</span><span class="sxs-lookup"><span data-stu-id="2419f-104">List favoritePlans</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2419f-105">Получение списка [планов](../resources/plannerplan.md) , помеченных пользователем как избранный.</span><span class="sxs-lookup"><span data-stu-id="2419f-105">Retrieve a list of [plannerPlans](../resources/plannerplan.md) that are marked as favorite by a user.</span></span> <span data-ttu-id="2419f-106">Вы можете пометить план как избранный, [обновив ресурс plannerUser](planneruser-update.md).</span><span class="sxs-lookup"><span data-stu-id="2419f-106">You can mark a plan as favorite by [updating the plannerUser resource](planneruser-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2419f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2419f-107">Permissions</span></span>
<span data-ttu-id="2419f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2419f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2419f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2419f-110">Permission type</span></span>      | <span data-ttu-id="2419f-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2419f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2419f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2419f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2419f-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="2419f-113">Group.Read.All</span></span>    |
|<span data-ttu-id="2419f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2419f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2419f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2419f-115">Not supported.</span></span>    |
|<span data-ttu-id="2419f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2419f-116">Application</span></span> | <span data-ttu-id="2419f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2419f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2419f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2419f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/favoritePlans
GET /users/<id>/planner/favoritePlans
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2419f-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="2419f-119">Optional query parameters</span></span>
<span data-ttu-id="2419f-120">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="2419f-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2419f-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2419f-121">Request headers</span></span>
| <span data-ttu-id="2419f-122">Имя</span><span class="sxs-lookup"><span data-stu-id="2419f-122">Name</span></span>      |<span data-ttu-id="2419f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2419f-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2419f-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2419f-124">Authorization</span></span>  | <span data-ttu-id="2419f-125">Bearer {Code}.</span><span class="sxs-lookup"><span data-stu-id="2419f-125">Bearer {code}.</span></span> <span data-ttu-id="2419f-126">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2419f-126">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2419f-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2419f-127">Request body</span></span>
<span data-ttu-id="2419f-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2419f-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="2419f-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2419f-129">Response</span></span>
<span data-ttu-id="2419f-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [plannerPlan](../resources/plannerplan.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="2419f-130">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2419f-131">Пример</span><span class="sxs-lookup"><span data-stu-id="2419f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2419f-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="2419f-132">Request</span></span>
<span data-ttu-id="2419f-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2419f-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_favoriteplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/favoritePlans
```
##### <a name="response"></a><span data-ttu-id="2419f-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="2419f-134">Response</span></span>
<span data-ttu-id="2419f-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2419f-135">The following is an example of the response.</span></span> 

><span data-ttu-id="2419f-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2419f-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
