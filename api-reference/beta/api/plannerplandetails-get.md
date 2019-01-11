---
title: Получение объекта plannerPlanDetails
description: Получение свойств и связей объекта **plannerplandetails**.
localization_priority: Normal
ms.openlocfilehash: 096e2092a71545c5008d82305f7c137a911db419
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871997"
---
# <a name="get-plannerplandetails"></a><span data-ttu-id="41a03-103">Получение объекта plannerPlanDetails</span><span class="sxs-lookup"><span data-stu-id="41a03-103">Get plannerPlanDetails</span></span>

> <span data-ttu-id="41a03-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="41a03-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41a03-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41a03-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="41a03-106">Получение свойств и связей объекта **plannerplandetails**.</span><span class="sxs-lookup"><span data-stu-id="41a03-106">Retrieve the properties and relationships of **plannerplandetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="41a03-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="41a03-107">Permissions</span></span>
<span data-ttu-id="41a03-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41a03-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41a03-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="41a03-110">Permission type</span></span>      | <span data-ttu-id="41a03-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="41a03-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41a03-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="41a03-112">Delegated (work or school account)</span></span> | <span data-ttu-id="41a03-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41a03-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="41a03-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="41a03-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41a03-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41a03-115">Not supported.</span></span>    |
|<span data-ttu-id="41a03-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="41a03-116">Application</span></span> | <span data-ttu-id="41a03-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="41a03-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="41a03-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="41a03-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/plans/<id>/details
```

## <a name="request-headers"></a><span data-ttu-id="41a03-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="41a03-119">Request headers</span></span>
| <span data-ttu-id="41a03-120">Имя</span><span class="sxs-lookup"><span data-stu-id="41a03-120">Name</span></span>      |<span data-ttu-id="41a03-121">Описание</span><span class="sxs-lookup"><span data-stu-id="41a03-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="41a03-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41a03-122">Authorization</span></span>  | <span data-ttu-id="41a03-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="41a03-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="41a03-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="41a03-125">Request body</span></span>
<span data-ttu-id="41a03-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="41a03-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41a03-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="41a03-127">Response</span></span>

<span data-ttu-id="41a03-128">В случае успеха этот метод возвращает код ответа `200 OK` и объект [plannerPlanDetails](../resources/plannerplandetails.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="41a03-128">If successful, this method returns a `200 OK` response code and [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.</span></span>

<span data-ttu-id="41a03-p104">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="41a03-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="41a03-132">Пример</span><span class="sxs-lookup"><span data-stu-id="41a03-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41a03-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="41a03-133">Request</span></span>
<span data-ttu-id="41a03-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="41a03-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerplandetails"
}-->
```http
GET https://graph.microsoft.com/beta/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details
```
##### <a name="response"></a><span data-ttu-id="41a03-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="41a03-135">Response</span></span>
<span data-ttu-id="41a03-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="41a03-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlanDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 373

{
  "sharedWith": {
    "aaa27244-1db4-476a-a5cb-004607466324" : true,
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true
  },
  "categoryDescriptions": {
    "category1": "Indoors",
    "category2": "Outdoors",
    "category3": null,
    "category4": null,
    "category5": "Needs materials",
    "category6": "Needs equipment"
  },
  "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerPlanDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
