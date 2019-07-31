---
title: Получение plannerUser
description: 'Получение свойств и связей объекта plannerUser. Возвращаемые свойства включают в себя избранные планы и недавно просмотренные планы пользователя. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: 4bc0bf1ddd07a1f03baa871bd96bf2193fae9e4c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992208"
---
# <a name="get-planneruser"></a><span data-ttu-id="36915-104">Получение plannerUser</span><span class="sxs-lookup"><span data-stu-id="36915-104">Get plannerUser</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36915-105">Получение свойств и связей объекта [plannerUser](../resources/planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="36915-105">Retrieve the properties and relationships of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="36915-106">Возвращаемые свойства включают в себя избранные планы и недавно просмотренные планы пользователя.</span><span class="sxs-lookup"><span data-stu-id="36915-106">The returned properties include the user's favorite plans and recently viewed plans.</span></span> 
## <a name="permissions"></a><span data-ttu-id="36915-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="36915-107">Permissions</span></span>
<span data-ttu-id="36915-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="36915-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="36915-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="36915-110">Permission type</span></span>      | <span data-ttu-id="36915-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="36915-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="36915-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="36915-112">Delegated (work or school account)</span></span> | <span data-ttu-id="36915-113">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="36915-113">Group.Read.All</span></span>    |
|<span data-ttu-id="36915-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="36915-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="36915-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36915-115">Not supported.</span></span>    |
|<span data-ttu-id="36915-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="36915-116">Application</span></span> | <span data-ttu-id="36915-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="36915-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="36915-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="36915-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner
GET /users/<id>/planner
```

## <a name="request-headers"></a><span data-ttu-id="36915-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="36915-119">Request headers</span></span>
| <span data-ttu-id="36915-120">Имя</span><span class="sxs-lookup"><span data-stu-id="36915-120">Name</span></span>      |<span data-ttu-id="36915-121">Описание</span><span class="sxs-lookup"><span data-stu-id="36915-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="36915-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="36915-122">Authorization</span></span>  | <span data-ttu-id="36915-123">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="36915-123">Bearer {code}.</span></span> <span data-ttu-id="36915-124">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="36915-124">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="36915-125">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="36915-125">Request body</span></span>
<span data-ttu-id="36915-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="36915-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="36915-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="36915-127">Response</span></span>
<span data-ttu-id="36915-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [plannerUser](../resources/planneruser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="36915-128">If successful, this method returns a `200 OK` response code and a [plannerUser](../resources/planneruser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="36915-129">Пример</span><span class="sxs-lookup"><span data-stu-id="36915-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="36915-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="36915-130">Request</span></span>
<span data-ttu-id="36915-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="36915-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_planneruser"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner
```
##### <a name="response"></a><span data-ttu-id="36915-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="36915-132">Response</span></span>
<span data-ttu-id="36915-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="36915-133">The following is an example of the response.</span></span> 

><span data-ttu-id="36915-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="36915-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Get plannerUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
