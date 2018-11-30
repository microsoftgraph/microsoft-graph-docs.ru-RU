---
title: Получение объекта plannerTaskDetails
description: Получение свойств и связей объекта **plannertaskdetails**.
ms.openlocfilehash: f0d0ad060d8cc43f72aaa6373429edf2f95bb1b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025496"
---
# <a name="get-plannertaskdetails"></a><span data-ttu-id="ac5fc-103">Получение объекта plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="ac5fc-103">Get plannerTaskDetails</span></span>

<span data-ttu-id="ac5fc-104">Получение свойств и связей объекта **plannertaskdetails**.</span><span class="sxs-lookup"><span data-stu-id="ac5fc-104">Retrieve the properties and relationships of **plannertaskdetails** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ac5fc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ac5fc-105">Permissions</span></span>
<span data-ttu-id="ac5fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac5fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac5fc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ac5fc-108">Permission type</span></span>      | <span data-ttu-id="ac5fc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ac5fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ac5fc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ac5fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ac5fc-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac5fc-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ac5fc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ac5fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ac5fc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac5fc-113">Not supported.</span></span>    |
|<span data-ttu-id="ac5fc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ac5fc-114">Application</span></span> | <span data-ttu-id="ac5fc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ac5fc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac5fc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ac5fc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/tasks/{id}/details
```

## <a name="request-headers"></a><span data-ttu-id="ac5fc-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ac5fc-117">Request headers</span></span>
| <span data-ttu-id="ac5fc-118">Имя</span><span class="sxs-lookup"><span data-stu-id="ac5fc-118">Name</span></span>      |<span data-ttu-id="ac5fc-119">Описание</span><span class="sxs-lookup"><span data-stu-id="ac5fc-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ac5fc-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ac5fc-120">Authorization</span></span>  | <span data-ttu-id="ac5fc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ac5fc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ac5fc-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ac5fc-123">Request body</span></span>
<span data-ttu-id="ac5fc-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ac5fc-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ac5fc-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="ac5fc-125">Response</span></span>

<span data-ttu-id="ac5fc-126">В случае успеха этот метод возвращает код ответа `200 OK` и объект [plannerTaskDetails](../resources/plannertaskdetails.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="ac5fc-126">If successful, this method returns a `200 OK` response code and [plannerTaskDetails](../resources/plannertaskdetails.md) object in the response body.</span></span>

<span data-ttu-id="ac5fc-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="ac5fc-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="ac5fc-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ac5fc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ac5fc-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="ac5fc-131">Request</span></span>
<span data-ttu-id="ac5fc-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ac5fc-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_plannertaskdetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/tasks/{task-id}/details
```
##### <a name="response"></a><span data-ttu-id="ac5fc-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="ac5fc-133">Response</span></span>
<span data-ttu-id="ac5fc-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="ac5fc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTaskDetails"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1036

{
  "description": "Task details properties:\nchecklist:Sub items\nreferences:Related links",
  "previewType": "automatic",
  "references": {
    "https%3A//developer%2Emicrosoft%2Ecom/en-us/graph/graph-explorer": {
      "@odata.type": "#microsoft.graph.plannerExternalReference",
      "alias": "Graph Explorer",
      "type": "Other",
      "previewPriority": "0009005706180391122",
      "lastModifiedBy": {
        "user": {
          "id": "fbab97d0-4932-4511-b675-204639209557"
        }
      },
      "lastModifiedDateTime": "2017-04-24T22:52:29.814Z"
    }
  },
  "checklist": {
    "d280ed1a-9f6b-4f9c-a962-fb4d00dc50ff": {
      "@odata.type": "#microsoft.graph.plannerChecklistItem",
      "isChecked": false,
      "title": "Try reading task details",
      "orderHint": "8587094707721254251P]",
      "lastModifiedBy": {
        "user": {
          "id": "e396de0e-4812-4fcb-9f9e-0358744df343"
        }
      },
      "lastModifiedDateTime": "2017-04-14T02:16:14.866Z"
    }
  },
  "id": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get plannerTaskDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->