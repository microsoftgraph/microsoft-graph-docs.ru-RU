---
title: Список recentPlans
description: Получение списка plannerPlans недавно просмотре пользователем. Недавно просматриваемые планы можно обновить, изменив plannerUser ресурсов.
author: TarkanSevilmis
ms.openlocfilehash: 68ed0cf626207e0cf02b6d32187598c3cf68d9d1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322510"
---
# <a name="list-recentplans"></a><span data-ttu-id="46cb8-104">Список recentPlans</span><span class="sxs-lookup"><span data-stu-id="46cb8-104">List recentPlans</span></span>

> <span data-ttu-id="46cb8-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="46cb8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="46cb8-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46cb8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="46cb8-107">Получение списка [plannerPlans](../resources/plannerplan.md) недавно просмотре пользователем.</span><span class="sxs-lookup"><span data-stu-id="46cb8-107">Retrieve a list of [plannerPlans](../resources/plannerplan.md) recently viewed by a user.</span></span> <span data-ttu-id="46cb8-108">Недавно просматриваемые планы можно обновить, [изменив plannerUser ресурсов](planneruser-update.md).</span><span class="sxs-lookup"><span data-stu-id="46cb8-108">You can update recently viewed plans by [updating the plannerUser resource](planneruser-update.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="46cb8-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="46cb8-109">Permissions</span></span>
<span data-ttu-id="46cb8-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="46cb8-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46cb8-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="46cb8-112">Permission type</span></span>      | <span data-ttu-id="46cb8-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="46cb8-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="46cb8-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="46cb8-114">Delegated (work or school account)</span></span> | <span data-ttu-id="46cb8-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="46cb8-115">Group.Read.All</span></span>    |
|<span data-ttu-id="46cb8-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="46cb8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="46cb8-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46cb8-117">Not supported.</span></span>    |
|<span data-ttu-id="46cb8-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="46cb8-118">Application</span></span> | <span data-ttu-id="46cb8-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="46cb8-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="46cb8-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="46cb8-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/recentPlans
GET /users/<id>/planner/recentPlans
```

## <a name="request-headers"></a><span data-ttu-id="46cb8-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="46cb8-121">Request headers</span></span>
| <span data-ttu-id="46cb8-122">Имя</span><span class="sxs-lookup"><span data-stu-id="46cb8-122">Name</span></span>      |<span data-ttu-id="46cb8-123">Описание</span><span class="sxs-lookup"><span data-stu-id="46cb8-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="46cb8-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="46cb8-124">Authorization</span></span>  | <span data-ttu-id="46cb8-p105">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="46cb8-p105">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46cb8-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="46cb8-127">Request body</span></span>
<span data-ttu-id="46cb8-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="46cb8-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="46cb8-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="46cb8-129">Response</span></span>
<span data-ttu-id="46cb8-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [plannerPlan](../resources/plannerplan.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="46cb8-130">If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="46cb8-131">Пример</span><span class="sxs-lookup"><span data-stu-id="46cb8-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="46cb8-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="46cb8-132">Request</span></span>
<span data-ttu-id="46cb8-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="46cb8-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_recentplans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/recentPlans
```
##### <a name="response"></a><span data-ttu-id="46cb8-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="46cb8-134">Response</span></span>
<span data-ttu-id="46cb8-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="46cb8-135">The following is an example of the response.</span></span> 

><span data-ttu-id="46cb8-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="46cb8-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List recentPlans",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
