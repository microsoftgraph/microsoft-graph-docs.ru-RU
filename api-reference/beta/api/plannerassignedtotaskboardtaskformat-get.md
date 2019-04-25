---
title: Получение объекта plannerAssignedToTaskBoardTaskFormat
description: Получение свойств и связей объекта **plannerAssignedToTaskBoardTaskFormat**.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 86cacbbab4a0c96c444400d0369cafd49f685554
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32539008"
---
# <a name="get-plannerassignedtotaskboardtaskformat"></a><span data-ttu-id="cee9e-103">Получение объекта plannerAssignedToTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="cee9e-103">Get plannerAssignedToTaskBoardTaskFormat</span></span>

<span data-ttu-id="cee9e-104">Получение свойств и связей объекта **plannerAssignedToTaskBoardTaskFormat**.</span><span class="sxs-lookup"><span data-stu-id="cee9e-104">Retrieve the properties and relationships of **plannerAssignedToTaskBoardTaskFormat** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cee9e-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cee9e-105">Permissions</span></span>
<span data-ttu-id="cee9e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cee9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cee9e-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cee9e-108">Permission type</span></span>      | <span data-ttu-id="cee9e-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cee9e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cee9e-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cee9e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cee9e-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cee9e-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cee9e-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cee9e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cee9e-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cee9e-113">Not supported.</span></span>    |
|<span data-ttu-id="cee9e-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cee9e-114">Application</span></span> | <span data-ttu-id="cee9e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cee9e-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cee9e-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cee9e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/assignedToTaskBoardFormat
```
## <a name="request-headers"></a><span data-ttu-id="cee9e-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cee9e-117">Request headers</span></span>
| <span data-ttu-id="cee9e-118">Имя</span><span class="sxs-lookup"><span data-stu-id="cee9e-118">Name</span></span>      |<span data-ttu-id="cee9e-119">Описание</span><span class="sxs-lookup"><span data-stu-id="cee9e-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="cee9e-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cee9e-120">Authorization</span></span>  | <span data-ttu-id="cee9e-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cee9e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cee9e-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cee9e-123">Request body</span></span>
<span data-ttu-id="cee9e-124">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cee9e-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cee9e-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="cee9e-125">Response</span></span>

<span data-ttu-id="cee9e-126">В случае успеха этот метод возвращает код ответа `200 OK` и объект [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="cee9e-126">If successful, this method returns a `200 OK` response code and [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.</span></span>

<span data-ttu-id="cee9e-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="cee9e-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="cee9e-130">Пример</span><span class="sxs-lookup"><span data-stu-id="cee9e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cee9e-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="cee9e-131">Request</span></span>
<span data-ttu-id="cee9e-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cee9e-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannerassignedtotaskboardtaskformat"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/assignedToTaskBoardFormat
```
##### <a name="response"></a><span data-ttu-id="cee9e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="cee9e-133">Response</span></span>
<span data-ttu-id="cee9e-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cee9e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerAssignedToTaskBoardTaskFormat"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "unassignedOrderHint": "RWk1",
  "orderHintsByAssignee": {
    "6463a5ce-2119-4198-9f2a-628761df4a62":"85752723360752+",
    "aaa27244-1db4-476a-a5cb-004607466324":"90057581;"
  },
  "id": "01gzSlKkIUSUl6DF_EilrmQAKDhh"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerAssignedToTaskBoardTaskFormat",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
