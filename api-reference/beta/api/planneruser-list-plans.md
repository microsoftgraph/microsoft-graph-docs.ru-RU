---
title: Перечисление планов
description: Получение списка объектов **plannerplan**, к которым есть доступ у объекта user.
localization_priority: Normal
ms.openlocfilehash: b64bae15222a42153ee5731b2ed0c4e623a6386a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875350"
---
# <a name="list-plans"></a><span data-ttu-id="758e5-103">Перечисление планов</span><span class="sxs-lookup"><span data-stu-id="758e5-103">List plans</span></span>

> <span data-ttu-id="758e5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="758e5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="758e5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="758e5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="758e5-106">Получение списка объектов **plannerplan**, к которым есть доступ у объекта [user](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="758e5-106">Retrieve a list of **plannerplan** objects shared with a [user](../resources/user.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="758e5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="758e5-107">Permissions</span></span>
<span data-ttu-id="758e5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="758e5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="758e5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="758e5-110">Permission type</span></span>      | <span data-ttu-id="758e5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="758e5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="758e5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="758e5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="758e5-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="758e5-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="758e5-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="758e5-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="758e5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="758e5-115">Not supported.</span></span>    |
|<span data-ttu-id="758e5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="758e5-116">Application</span></span> | <span data-ttu-id="758e5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="758e5-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="758e5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="758e5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/plans
GET /users/<id>/planner/plans
GET /drive/root/createdByUser/planner/plans
```

## <a name="request-headers"></a><span data-ttu-id="758e5-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="758e5-119">Request headers</span></span>
| <span data-ttu-id="758e5-120">Имя</span><span class="sxs-lookup"><span data-stu-id="758e5-120">Name</span></span>      |<span data-ttu-id="758e5-121">Описание</span><span class="sxs-lookup"><span data-stu-id="758e5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="758e5-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="758e5-122">Authorization</span></span>  | <span data-ttu-id="758e5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="758e5-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="758e5-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="758e5-125">Request body</span></span>
<span data-ttu-id="758e5-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="758e5-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="758e5-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="758e5-127">Response</span></span>

<span data-ttu-id="758e5-128">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [plannerPlan](../resources/plannerplan.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="758e5-128">If successful, this method returns a `200 OK` response code and collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.</span></span>

<span data-ttu-id="758e5-p104">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="758e5-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="758e5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="758e5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="758e5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="758e5-133">Request</span></span>
<span data-ttu-id="758e5-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="758e5-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plans"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/plans
```
##### <a name="response"></a><span data-ttu-id="758e5-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="758e5-135">Response</span></span>
<span data-ttu-id="758e5-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="758e5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlan",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 438

{
  "value": [
    {
      "createdBy": {
        "application": {
          "id": "95e27074-6c4a-447a-aa24-9d718a0b86fa"
        },
        "user": {
          "id": "ebf3b108-5234-4e22-b93d-656d7dae5874"
        }
      },
      "createdDateTime": "2015-03-30T18:36:49.2407981Z",
      "owner": "ebf3b108-5234-4e22-b93d-656d7dae5874",
      "title": "title-value",
      "id": "xqQg5FS2LkCp935s-FIFm2QAFkHM"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List plans",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
