---
title: Список объектов schedulingGroup
description: Получите список schedulingGroup в этом расписании.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e4d45bb7b3948a6e8626299fd35adc1308a33a6c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053512"
---
# <a name="list-schedulegroups"></a><span data-ttu-id="54113-103">Расписание списковGroups</span><span class="sxs-lookup"><span data-stu-id="54113-103">List scheduleGroups</span></span>

<span data-ttu-id="54113-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="54113-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54113-105">Получите список [schedulingGroups в](../resources/schedulinggroup.md) этом [расписании.](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="54113-105">Get the list of [schedulingGroups](../resources/schedulinggroup.md) in this [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="54113-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="54113-106">Permissions</span></span>

<span data-ttu-id="54113-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="54113-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="54113-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="54113-109">Permission type</span></span>      | <span data-ttu-id="54113-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="54113-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="54113-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="54113-111">Delegated (work or school account)</span></span> | <span data-ttu-id="54113-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54113-112">Schedule.Read.All, Group.Read.All, Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="54113-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="54113-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="54113-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54113-114">Not supported.</span></span>    |
|<span data-ttu-id="54113-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="54113-115">Application</span></span> | <span data-ttu-id="54113-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54113-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="54113-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="54113-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="54113-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="54113-118">Request headers</span></span>

| <span data-ttu-id="54113-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="54113-119">Header</span></span>       | <span data-ttu-id="54113-120">Значение</span><span class="sxs-lookup"><span data-stu-id="54113-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="54113-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="54113-121">Authorization</span></span>  | <span data-ttu-id="54113-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="54113-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="54113-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="54113-124">Request body</span></span>
<span data-ttu-id="54113-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="54113-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54113-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="54113-126">Response</span></span>

<span data-ttu-id="54113-127">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [schedulingGroup](../resources/schedulinggroup.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="54113-127">If successful, this method returns a `200 OK` response code and a collection of [schedulingGroup](../resources/schedulinggroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54113-128">Пример</span><span class="sxs-lookup"><span data-stu-id="54113-128">Example</span></span>

#### <a name="request"></a><span data-ttu-id="54113-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="54113-129">Request</span></span>

<span data-ttu-id="54113-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="54113-130">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="54113-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="54113-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-list-schedulinggroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups
```
# <a name="c"></a>[<span data-ttu-id="54113-132">C#</span><span class="sxs-lookup"><span data-stu-id="54113-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-list-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="54113-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="54113-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-list-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="54113-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="54113-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-list-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="54113-135">Java</span><span class="sxs-lookup"><span data-stu-id="54113-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-list-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="54113-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="54113-136">Response</span></span>

<span data-ttu-id="54113-137">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="54113-137">The following is an example of the response.</span></span> 

><span data-ttu-id="54113-138">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="54113-138">**Note:** The response object shown here might be shortened for readability.</span></span>
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


