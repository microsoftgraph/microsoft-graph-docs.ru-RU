---
title: Перечисление задач
description: Получение списка объектов **plannerTask**, связанных с объектом plannerBucket.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: bcebc3c9188ad4e93272964674483ef898f4def4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981611"
---
# <a name="list-tasks"></a><span data-ttu-id="56dbf-103">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="56dbf-103">List tasks</span></span>

<span data-ttu-id="56dbf-104">Получение списка объектов **plannerTask**, связанных с объектом [plannerBucket](../resources/plannerbucket.md).</span><span class="sxs-lookup"><span data-stu-id="56dbf-104">Retrieve a list of **plannerTask** objects associated to a [plannerBucket](../resources/plannerbucket.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="56dbf-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="56dbf-105">Permissions</span></span>
<span data-ttu-id="56dbf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="56dbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56dbf-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="56dbf-108">Permission type</span></span>      | <span data-ttu-id="56dbf-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="56dbf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="56dbf-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="56dbf-110">Delegated (work or school account)</span></span> | <span data-ttu-id="56dbf-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56dbf-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="56dbf-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="56dbf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="56dbf-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56dbf-113">Not supported.</span></span>    |
|<span data-ttu-id="56dbf-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="56dbf-114">Application</span></span> | <span data-ttu-id="56dbf-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="56dbf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="56dbf-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="56dbf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets/{id}/tasks
```

## <a name="request-headers"></a><span data-ttu-id="56dbf-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="56dbf-117">Request headers</span></span>
| <span data-ttu-id="56dbf-118">Имя</span><span class="sxs-lookup"><span data-stu-id="56dbf-118">Name</span></span>      |<span data-ttu-id="56dbf-119">Описание</span><span class="sxs-lookup"><span data-stu-id="56dbf-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="56dbf-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="56dbf-120">Authorization</span></span>  | <span data-ttu-id="56dbf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="56dbf-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56dbf-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="56dbf-123">Request body</span></span>
<span data-ttu-id="56dbf-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="56dbf-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56dbf-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="56dbf-125">Response</span></span>

<span data-ttu-id="56dbf-126">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [plannerTask](../resources/plannertask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="56dbf-126">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="56dbf-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="56dbf-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="56dbf-130">Пример</span><span class="sxs-lookup"><span data-stu-id="56dbf-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="56dbf-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="56dbf-131">Request</span></span>
<span data-ttu-id="56dbf-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="56dbf-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/v1.0/planner/buckets/{task-id}/tasks
```
##### <a name="response"></a><span data-ttu-id="56dbf-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="56dbf-133">Response</span></span>
<span data-ttu-id="56dbf-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="56dbf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 833

{
  "value": [
    {
      "createdBy": {
        "user": {
          "id": "6463a5ce-2119-4198-9f2a-628761df4a62"
        }
      },
      "planId": "xqQg5FS2LkCp935s-FIFm2QAFkHM",
      "bucketId": "gcrYAaAkgU2EQUvpkNNXLGQAGTtu",
      "title": "title-value",
      "orderHint": "9223370609546166567W",
      "assigneePriority": "90057581\"",
      "createdDateTime": "2015-03-25T18:36:49.2407981Z",
      "assignments": {
        "fbab97d0-4932-4511-b675-204639209557": {
          "@odata.type": "#microsoft.graph.plannerassignment",
          "assignedBy": {
            "user": {
              "id": "1e9955d2-6acd-45bf-86d3-b546fdc795eb"
            }
          },
          "assignedDateTime": "2015-03-25T18:38:21.956Z",
          "orderHint": "RWk1"
         }
      },
      "id":"01gzSlKkIUSUl6DF_EilrmQAKDhh"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
