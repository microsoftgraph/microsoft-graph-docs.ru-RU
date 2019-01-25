---
title: Перечисление задач
description: Получение списка объектов **plannertask**, назначенных объекту User.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 1f2f1e9378971cef887214b2a4992198d9e797bb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520146"
---
# <a name="list-tasks"></a><span data-ttu-id="8ed53-103">Перечисление задач</span><span class="sxs-lookup"><span data-stu-id="8ed53-103">List tasks</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ed53-104">Получение списка объектов **plannertask**, назначенных объекту User.</span><span class="sxs-lookup"><span data-stu-id="8ed53-104">Retrieve a list of **plannertask** objects assigned to a User.</span></span>

## <a name="permissions"></a><span data-ttu-id="8ed53-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8ed53-105">Permissions</span></span>
<span data-ttu-id="8ed53-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8ed53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8ed53-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8ed53-108">Permission type</span></span>      | <span data-ttu-id="8ed53-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8ed53-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8ed53-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8ed53-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8ed53-111">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8ed53-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="8ed53-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8ed53-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8ed53-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ed53-113">Not supported.</span></span>    |
|<span data-ttu-id="8ed53-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8ed53-114">Application</span></span> | <span data-ttu-id="8ed53-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8ed53-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="8ed53-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8ed53-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/planner/tasks
GET /users/<id>/planner/tasks
```

## <a name="request-headers"></a><span data-ttu-id="8ed53-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8ed53-117">Request headers</span></span>
| <span data-ttu-id="8ed53-118">Имя</span><span class="sxs-lookup"><span data-stu-id="8ed53-118">Name</span></span>      |<span data-ttu-id="8ed53-119">Описание</span><span class="sxs-lookup"><span data-stu-id="8ed53-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8ed53-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8ed53-120">Authorization</span></span>  | <span data-ttu-id="8ed53-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8ed53-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8ed53-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8ed53-123">Request body</span></span>
<span data-ttu-id="8ed53-124">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="8ed53-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8ed53-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="8ed53-125">Response</span></span>

<span data-ttu-id="8ed53-126">В случае успеха этот метод возвращает код ответа `200 OK` и коллекцию объектов [plannerTask](../resources/plannertask.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="8ed53-126">If successful, this method returns a `200 OK` response code and collection of [plannerTask](../resources/plannertask.md) objects in the response body.</span></span>

<span data-ttu-id="8ed53-p103">Этот метод может возвращать любые [коды состояния HTTP](/graph/errors). Приложения должны обрабатывать ошибки 403 и 404, которые возникают чаще всего. Дополнительные сведения об этих ошибках см. в разделе [Основные ошибки Планировщика](../resources/planner-overview.md#common-planner-error-conditions).</span><span class="sxs-lookup"><span data-stu-id="8ed53-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="8ed53-130">Пример</span><span class="sxs-lookup"><span data-stu-id="8ed53-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8ed53-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="8ed53-131">Request</span></span>
<span data-ttu-id="8ed53-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8ed53-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_tasks"
}-->
```http
GET https://graph.microsoft.com/beta/me/planner/tasks
```
##### <a name="response"></a><span data-ttu-id="8ed53-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="8ed53-133">Response</span></span>
<span data-ttu-id="8ed53-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="8ed53-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
          "@odata.type": "#microsoft.graph.plannerAssignment",
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
<!--
{
  "type": "#page.annotation",
  "description": "List tasks",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-list-tasks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
