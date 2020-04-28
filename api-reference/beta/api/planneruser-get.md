---
title: Получение объекта plannerUser
description: 'Получение свойств и связей объекта plannerUser. Возвращаемые свойства включают в себя избранные планы и недавно просмотренные планы пользователя. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: apiPageType
ms.openlocfilehash: f87a84d9297fbbde1d5fb9d6045dadae10e6bd72
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455580"
---
# <a name="get-planneruser"></a><span data-ttu-id="9510c-104">Получение объекта plannerUser</span><span class="sxs-lookup"><span data-stu-id="9510c-104">Get plannerUser</span></span>

<span data-ttu-id="9510c-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9510c-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9510c-106">Получение свойств и связей объекта [plannerUser](../resources/planneruser.md) .</span><span class="sxs-lookup"><span data-stu-id="9510c-106">Retrieve the properties and relationships of a [plannerUser](../resources/planneruser.md) object.</span></span> <span data-ttu-id="9510c-107">Возвращаемые свойства включают в себя избранные планы и недавно просмотренные планы пользователя.</span><span class="sxs-lookup"><span data-stu-id="9510c-107">The returned properties include the user's favorite plans and recently viewed plans.</span></span> 
## <a name="permissions"></a><span data-ttu-id="9510c-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9510c-108">Permissions</span></span>
<span data-ttu-id="9510c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9510c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9510c-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9510c-111">Permission type</span></span>      | <span data-ttu-id="9510c-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9510c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9510c-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9510c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9510c-114">Group.Read.All</span><span class="sxs-lookup"><span data-stu-id="9510c-114">Group.Read.All</span></span>    |
|<span data-ttu-id="9510c-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9510c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9510c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9510c-116">Not supported.</span></span>    |
|<span data-ttu-id="9510c-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9510c-117">Application</span></span> | <span data-ttu-id="9510c-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9510c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9510c-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9510c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner
GET /users/{id}/planner
```

## <a name="request-headers"></a><span data-ttu-id="9510c-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9510c-120">Request headers</span></span>
| <span data-ttu-id="9510c-121">Имя</span><span class="sxs-lookup"><span data-stu-id="9510c-121">Name</span></span>      |<span data-ttu-id="9510c-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9510c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9510c-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9510c-123">Authorization</span></span>  | <span data-ttu-id="9510c-124">Bearer {код}.</span><span class="sxs-lookup"><span data-stu-id="9510c-124">Bearer {code}.</span></span> <span data-ttu-id="9510c-125">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="9510c-125">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9510c-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9510c-126">Request body</span></span>
<span data-ttu-id="9510c-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9510c-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="9510c-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="9510c-128">Response</span></span>
<span data-ttu-id="9510c-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [plannerUser](../resources/planneruser.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="9510c-129">If successful, this method returns a `200 OK` response code and a [plannerUser](../resources/planneruser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9510c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9510c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9510c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9510c-131">Request</span></span>
<span data-ttu-id="9510c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9510c-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_planneruser"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner
```
##### <a name="response"></a><span data-ttu-id="9510c-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="9510c-133">Response</span></span>
<span data-ttu-id="9510c-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9510c-134">The following is an example of the response.</span></span> 

><span data-ttu-id="9510c-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9510c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
