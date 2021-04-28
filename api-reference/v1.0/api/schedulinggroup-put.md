---
title: Замена объекта schedulingGroup
description: Замените существующую группу планирования.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f6dd53bea34e39200bdc4a75d1013fc7537e203c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038994"
---
# <a name="replace-schedulinggroup"></a><span data-ttu-id="d0772-103">Замена объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="d0772-103">Replace schedulingGroup</span></span>

<span data-ttu-id="d0772-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0772-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d0772-105">Замените [существующую группу планирования](../resources/schedulinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="d0772-105">Replace an existing [schedulingGroup](../resources/schedulinggroup.md).</span></span>

<span data-ttu-id="d0772-106">Если указанной [schedulingGroup](../resources/schedulinggroup.md) не существует, этот метод `404 Not found` возвращается.</span><span class="sxs-lookup"><span data-stu-id="d0772-106">If the specified [schedulingGroup](../resources/schedulinggroup.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0772-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d0772-107">Permissions</span></span>

<span data-ttu-id="d0772-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d0772-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0772-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d0772-110">Permission type</span></span>      | <span data-ttu-id="d0772-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d0772-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0772-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d0772-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d0772-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0772-113">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d0772-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d0772-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0772-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d0772-115">Not supported.</span></span>    |
|<span data-ttu-id="d0772-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d0772-116">Application</span></span> | <span data-ttu-id="d0772-117">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0772-117">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0772-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d0772-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="d0772-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d0772-119">Request headers</span></span>

| <span data-ttu-id="d0772-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d0772-120">Header</span></span>       | <span data-ttu-id="d0772-121">Значение</span><span class="sxs-lookup"><span data-stu-id="d0772-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d0772-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d0772-122">Authorization</span></span>  | <span data-ttu-id="d0772-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0772-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d0772-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0772-125">Content-Type</span></span>  | <span data-ttu-id="d0772-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d0772-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d0772-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d0772-128">Request body</span></span>

<span data-ttu-id="d0772-129">В теле запроса поставляем представление JSON объекта [schedulingGroup.](../resources/schedulinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="d0772-129">In the request body, supply a JSON representation of a [schedulingGroup](../resources/schedulinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d0772-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0772-130">Response</span></span>

<span data-ttu-id="d0772-131">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект schedulingGroup](../resources/schedulinggroup.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="d0772-131">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0772-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d0772-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0772-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="d0772-133">Request</span></span>

<span data-ttu-id="d0772-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d0772-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d0772-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d0772-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-put-schedulinggroups"
}-->
```http
PUT https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
Content-type: application/json
Prefer: return=representation

{
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="d0772-136">C#</span><span class="sxs-lookup"><span data-stu-id="d0772-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-put-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d0772-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d0772-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-put-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d0772-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d0772-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-put-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d0772-139">Java</span><span class="sxs-lookup"><span data-stu-id="d0772-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-put-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="d0772-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="d0772-140">Response</span></span>

<span data-ttu-id="d0772-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="d0772-141">The following is an example of the response.</span></span> 

><span data-ttu-id="d0772-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="d0772-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

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
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing schedulingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

