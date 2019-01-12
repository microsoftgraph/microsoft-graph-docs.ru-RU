---
title: Перечисление сегментов
description: Получение списка объектов **plannerbucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: c0648d659dbb33c3e7d51b38999648637721ca7b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928733"
---
# <a name="list-buckets"></a><span data-ttu-id="cb37a-103">Перечисление сегментов</span><span class="sxs-lookup"><span data-stu-id="cb37a-103">List buckets</span></span>

> <span data-ttu-id="cb37a-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cb37a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb37a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb37a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cb37a-106">Получение списка объектов **plannerbucket**.</span><span class="sxs-lookup"><span data-stu-id="cb37a-106">Retrieve a list of **plannerbucket** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb37a-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb37a-107">Permissions</span></span>
<span data-ttu-id="cb37a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb37a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb37a-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb37a-110">Permission type</span></span>      | <span data-ttu-id="cb37a-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cb37a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cb37a-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb37a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cb37a-113">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb37a-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cb37a-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb37a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cb37a-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb37a-115">Not supported.</span></span>    |
|<span data-ttu-id="cb37a-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb37a-116">Application</span></span> | <span data-ttu-id="cb37a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb37a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cb37a-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb37a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cb37a-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="cb37a-119">Optional query parameters</span></span>
<span data-ttu-id="cb37a-120">Этот метод требует указания [фильтра](https://developer.microsoft.com/graph/docs/concepts/query_parameters) по идентификатору плана.</span><span class="sxs-lookup"><span data-stu-id="cb37a-120">This method requires planId [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cb37a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb37a-121">Request headers</span></span>
| <span data-ttu-id="cb37a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="cb37a-122">Name</span></span>      |<span data-ttu-id="cb37a-123">Описание</span><span class="sxs-lookup"><span data-stu-id="cb37a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cb37a-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cb37a-124">Authorization</span></span>  | <span data-ttu-id="cb37a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb37a-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb37a-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="cb37a-127">Request body</span></span>
<span data-ttu-id="cb37a-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cb37a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cb37a-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb37a-129">Response</span></span>

<span data-ttu-id="cb37a-130">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [plannerBucket](../resources/plannerbucket.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cb37a-130">If successful, this method returns a `200 OK` response code and collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="cb37a-p104">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="cb37a-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="cb37a-134">Пример</span><span class="sxs-lookup"><span data-stu-id="cb37a-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cb37a-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb37a-135">Request</span></span>
<span data-ttu-id="cb37a-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb37a-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/beta/planner/buckets
```
##### <a name="response"></a><span data-ttu-id="cb37a-137">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb37a-137">Response</span></span>
<span data-ttu-id="cb37a-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="cb37a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtQnVja2V0QEBAQEBAQEBAQEBAQEBARCc=\"",
      "name": "To do",
      "planId": "2txjA-BMZEq-bKi6Wfj5aGQAB1OJ",
      "orderHint": "85752723360752+",
      "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
