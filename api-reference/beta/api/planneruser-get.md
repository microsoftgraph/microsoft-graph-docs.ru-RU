---
title: Получение plannerUser
description: 'Извлечение свойств и связи объекта plannerUser. Возвращаемых свойств включают пользователя избранные планы и планы, которые были открыты. '
localization_priority: Normal
ms.openlocfilehash: 1abffddb2ddbefdcd0aaeddedffe94ae8ad605d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810642"
---
# <a name="get-planneruser"></a><span data-ttu-id="9e6e2-104">Получение plannerUser</span><span class="sxs-lookup"><span data-stu-id="9e6e2-104">Get plannerUser</span></span>

> <span data-ttu-id="9e6e2-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9e6e2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e6e2-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e6e2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9e6e2-107">Извлечение свойств и связи объекта [plannerUser](../resources/planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="9e6e2-107">Retrieve the properties and relationships of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="9e6e2-108">Возвращаемых свойств включают пользователя избранные планы и планы, которые были открыты.</span><span class="sxs-lookup"><span data-stu-id="9e6e2-108">The returned properties include the user's favorite plans and recently viewed plans.</span></span> 
## <a name="permissions"></a><span data-ttu-id="9e6e2-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9e6e2-109">Permissions</span></span>
<span data-ttu-id="9e6e2-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9e6e2-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e6e2-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9e6e2-112">Permission type</span></span>      | <span data-ttu-id="9e6e2-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9e6e2-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9e6e2-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9e6e2-114">Delegated (work or school account)</span></span> | <span data-ttu-id="9e6e2-115">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e6e2-115">Group.Read.All</span></span>    |
|<span data-ttu-id="9e6e2-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9e6e2-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e6e2-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e6e2-117">Not supported.</span></span>    |
|<span data-ttu-id="9e6e2-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9e6e2-118">Application</span></span> | <span data-ttu-id="9e6e2-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9e6e2-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e6e2-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9e6e2-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner
GET /users/<id>/planner
```

## <a name="request-headers"></a><span data-ttu-id="9e6e2-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9e6e2-121">Request headers</span></span>
| <span data-ttu-id="9e6e2-122">Имя</span><span class="sxs-lookup"><span data-stu-id="9e6e2-122">Name</span></span>      |<span data-ttu-id="9e6e2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="9e6e2-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9e6e2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e6e2-124">Authorization</span></span>  | <span data-ttu-id="9e6e2-p105">В заголовке указывается "Bearer {код}". Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9e6e2-p105">Bearer {code}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e6e2-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9e6e2-127">Request body</span></span>
<span data-ttu-id="9e6e2-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9e6e2-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9e6e2-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="9e6e2-129">Response</span></span>
<span data-ttu-id="9e6e2-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [plannerUser](../resources/planneruser.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9e6e2-130">If successful, this method returns a `200 OK` response code and a [plannerUser](../resources/planneruser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9e6e2-131">Пример</span><span class="sxs-lookup"><span data-stu-id="9e6e2-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9e6e2-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="9e6e2-132">Request</span></span>
<span data-ttu-id="9e6e2-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9e6e2-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_planneruser"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner
```
##### <a name="response"></a><span data-ttu-id="9e6e2-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="9e6e2-134">Response</span></span>
<span data-ttu-id="9e6e2-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9e6e2-135">The following is an example of the response.</span></span> 

><span data-ttu-id="9e6e2-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9e6e2-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 979

{
  "favoritePlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586866870001551087",
      "planTitle": "Next Release Discussion"
    },
    "uZWtCtli30CGoWLIWSat1mQAC0ai": {
      "@odata.type": "#microsoft.graph.plannerFavoritePlanReference",
      "orderHint": "8586888705198093378",
      "planTitle": "Product Support"
    }
  },
  "recentPlanReferences": {
    "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-02T22:49:46.155Z",
      "planTitle": "Next Release Discussion"
    },
    "XYE5pqNJu0uuRC2PM4ZQrmQAF2Pn": {
      "@odata.type": "#microsoft.graph.plannerRecentPlanReference",
      "lastAccessedDateTime": "2018-01-01T19:39:17.57Z",
      "planTitle": "Success Metrics"
    }
  },
  "id": "-YPnMJRiIUSKFyaVjYEkBWQAAc47"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
