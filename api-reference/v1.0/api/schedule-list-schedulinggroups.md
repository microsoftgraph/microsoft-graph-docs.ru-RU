---
title: Список объектов schedulingGroup
description: Получение списка Счедулингграуп в этом расписании.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7628c20df5e72e5c780361e3c858648b586d7c8d
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315093"
---
# <a name="list-schedulegroups"></a><span data-ttu-id="239f6-103">Список Счедулеграупс</span><span class="sxs-lookup"><span data-stu-id="239f6-103">List scheduleGroups</span></span>

<span data-ttu-id="239f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="239f6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="239f6-105">Получение списка [счедулингграупс](../resources/schedulinggroup.md) в этом [расписании](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="239f6-105">Get the list of [schedulingGroups](../resources/schedulinggroup.md) in this [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="239f6-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="239f6-106">Permissions</span></span>

<span data-ttu-id="239f6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="239f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="239f6-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="239f6-109">Permission type</span></span>      | <span data-ttu-id="239f6-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="239f6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="239f6-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="239f6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="239f6-112">Schedule. Read. ALL, Group. Read. ALL, Schedule. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="239f6-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="239f6-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="239f6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="239f6-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="239f6-114">Not supported.</span></span>    |
|<span data-ttu-id="239f6-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="239f6-115">Application</span></span> | <span data-ttu-id="239f6-116">Schedule. Read. ALL, Schedule. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="239f6-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="239f6-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="239f6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="239f6-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="239f6-118">Request headers</span></span>

| <span data-ttu-id="239f6-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="239f6-119">Header</span></span>       | <span data-ttu-id="239f6-120">Значение</span><span class="sxs-lookup"><span data-stu-id="239f6-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="239f6-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="239f6-121">Authorization</span></span>  | <span data-ttu-id="239f6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="239f6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="239f6-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="239f6-124">Request body</span></span>
<span data-ttu-id="239f6-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="239f6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="239f6-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="239f6-126">Response</span></span>

<span data-ttu-id="239f6-127">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [счедулингграуп](../resources/schedulinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="239f6-127">If successful, this method returns a `200 OK` response code and a collection of [schedulingGroup](../resources/schedulinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="239f6-128">Пример</span><span class="sxs-lookup"><span data-stu-id="239f6-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="239f6-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="239f6-129">Request</span></span>

<span data-ttu-id="239f6-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="239f6-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="239f6-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="239f6-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-schedulinggroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups
```
# <a name="c"></a>[<span data-ttu-id="239f6-132">C#</span><span class="sxs-lookup"><span data-stu-id="239f6-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="239f6-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="239f6-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="239f6-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="239f6-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="239f6-135">Java</span><span class="sxs-lookup"><span data-stu-id="239f6-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-list-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a><span data-ttu-id="239f6-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="239f6-136">Response</span></span>

<span data-ttu-id="239f6-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="239f6-137">The following is an example of the response.</span></span> 

><span data-ttu-id="239f6-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="239f6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "value": [
    {
      "id": "TAG_f914d037-00a3-4ba4-b712-ef178cbea263",
      "createdDateTime": "2019-03-12T22:10:38.242Z",
      "lastModifiedDateTime": "2019-03-12T22:10:38.242Z",
      "displayName": "Cashiers",
      "isActive": true,
      "userIds": [
        "c5d0c76b-80c4-481c-be50-923cd8d680a1",
        "2a4296b3-a28a-44ba-bc66-0274b9b95851"
      ],
      "lastModifiedBy": {
        "@odata.type":"microsoft.graph.identitySet",
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
          "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
          "displayName": "John Doe"
        }
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get the list of schedulingGroup in this schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

