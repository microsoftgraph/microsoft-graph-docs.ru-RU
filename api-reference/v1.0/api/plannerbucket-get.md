---
title: Получение объекта plannerBucket
description: Получение свойств и связей объекта **plannerBucket**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: d331523ad2d205f2e01431f943da6095ecd667f8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953762"
---
# <a name="get-plannerbucket"></a><span data-ttu-id="339e1-103">Получение объекта plannerBucket</span><span class="sxs-lookup"><span data-stu-id="339e1-103">Get plannerBucket</span></span>

<span data-ttu-id="339e1-104">Получение свойств и связей объекта **plannerBucket**.</span><span class="sxs-lookup"><span data-stu-id="339e1-104">Retrieve the properties and relationships of **plannerBucket** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="339e1-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="339e1-105">Permissions</span></span>
<span data-ttu-id="339e1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="339e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="339e1-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="339e1-108">Permission type</span></span>      | <span data-ttu-id="339e1-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="339e1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="339e1-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="339e1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="339e1-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="339e1-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="339e1-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="339e1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="339e1-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="339e1-113">Not supported.</span></span>    |
|<span data-ttu-id="339e1-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="339e1-114">Application</span></span> | <span data-ttu-id="339e1-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="339e1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="339e1-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="339e1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets/{id}
```

## <a name="request-headers"></a><span data-ttu-id="339e1-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="339e1-117">Request headers</span></span>
| <span data-ttu-id="339e1-118">Имя</span><span class="sxs-lookup"><span data-stu-id="339e1-118">Name</span></span>      |<span data-ttu-id="339e1-119">Описание</span><span class="sxs-lookup"><span data-stu-id="339e1-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="339e1-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="339e1-120">Authorization</span></span>  | <span data-ttu-id="339e1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="339e1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="339e1-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="339e1-123">Request body</span></span>
<span data-ttu-id="339e1-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="339e1-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="339e1-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="339e1-125">Response</span></span>

<span data-ttu-id="339e1-126">В случае успеха этот метод возвращает код ответа `200 OK` и объект [plannerBucket](../resources/plannerbucket.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="339e1-126">If successful, this method returns a `200 OK` response code and [plannerBucket](../resources/plannerbucket.md) object in the response body.</span></span>

<span data-ttu-id="339e1-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="339e1-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="339e1-130">Пример</span><span class="sxs-lookup"><span data-stu-id="339e1-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="339e1-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="339e1-131">Request</span></span>
<span data-ttu-id="339e1-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="339e1-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerbucket"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/buckets/{bucket-id}
```
##### <a name="response"></a><span data-ttu-id="339e1-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="339e1-133">Response</span></span>
<span data-ttu-id="339e1-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="339e1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 245

{
  "name": "Advertising",
  "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
  "orderHint": "85752723360752+",
  "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
