---
title: Получение объекта plannerBucketTaskBoardTaskFormat
description: Получение свойств и связей объекта **plannerBucketTaskBoardTaskFormat**.
ms.openlocfilehash: 8172c8afeb04613276d9b11ee532b36ef1709e87
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026951"
---
# <a name="get-plannerbuckettaskboardtaskformat"></a><span data-ttu-id="5fd3c-103">Получение объекта plannerBucketTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="5fd3c-103">Get plannerBucketTaskBoardTaskFormat</span></span>

<span data-ttu-id="5fd3c-104">Получение свойств и связей объекта **plannerBucketTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="5fd3c-104">Retrieve the properties and relationships of **plannerBucketTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="5fd3c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5fd3c-105">Permissions</span></span>
<span data-ttu-id="5fd3c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fd3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fd3c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5fd3c-108">Permission type</span></span>      | <span data-ttu-id="5fd3c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5fd3c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5fd3c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5fd3c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="5fd3c-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fd3c-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5fd3c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5fd3c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fd3c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fd3c-113">Not supported.</span></span>    |
|<span data-ttu-id="5fd3c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5fd3c-114">Application</span></span> | <span data-ttu-id="5fd3c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5fd3c-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5fd3c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5fd3c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/bucketTaskBoardFormat
```

## <a name="request-headers"></a><span data-ttu-id="5fd3c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5fd3c-117">Request headers</span></span>
| <span data-ttu-id="5fd3c-118">Имя</span><span class="sxs-lookup"><span data-stu-id="5fd3c-118">Name</span></span>      |<span data-ttu-id="5fd3c-119">Описание</span><span class="sxs-lookup"><span data-stu-id="5fd3c-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5fd3c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5fd3c-120">Authorization</span></span>  | <span data-ttu-id="5fd3c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5fd3c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5fd3c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5fd3c-123">Request body</span></span>
<span data-ttu-id="5fd3c-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5fd3c-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fd3c-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="5fd3c-125">Response</span></span>

<span data-ttu-id="5fd3c-126">В случае успеха этот метод возвращает код ответа `200 OK` и объект [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5fd3c-126">If successful, this method returns a `200 OK` response code and [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="5fd3c-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="5fd3c-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="5fd3c-130">Пример</span><span class="sxs-lookup"><span data-stu-id="5fd3c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5fd3c-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="5fd3c-131">Request</span></span>
<span data-ttu-id="5fd3c-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5fd3c-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerbuckettaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/bucketTaskBoardFormat
```
##### <a name="response"></a><span data-ttu-id="5fd3c-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="5fd3c-133">Response</span></span>
<span data-ttu-id="5fd3c-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="5fd3c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucketTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 76

{
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh",
  "orderHint": "85752723360752+"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerBucketTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->