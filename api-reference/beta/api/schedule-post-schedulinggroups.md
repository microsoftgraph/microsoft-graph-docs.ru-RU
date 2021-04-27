---
title: Создание объекта schedulingGroup
description: Создание нового объекта schedulingGroup
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ef8ae3c8f878d6414929997e75e5ece29434a09d
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052728"
---
# <a name="create-schedulinggroup"></a><span data-ttu-id="6672f-103">Создание объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="6672f-103">Create schedulingGroup</span></span>

<span data-ttu-id="6672f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6672f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6672f-105">Создание нового объекта [schedulingGroup](../resources/schedulinggroup.md)</span><span class="sxs-lookup"><span data-stu-id="6672f-105">Create a new [schedulingGroup](../resources/schedulinggroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6672f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6672f-106">Permissions</span></span>

<span data-ttu-id="6672f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6672f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6672f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6672f-109">Permission type</span></span>      | <span data-ttu-id="6672f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6672f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6672f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6672f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6672f-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6672f-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6672f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6672f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6672f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6672f-114">Not supported.</span></span>    |
|<span data-ttu-id="6672f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="6672f-115">Application</span></span> |<span data-ttu-id="6672f-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6672f-116">Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6672f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6672f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/schedulingGroups
```

## <a name="request-headers"></a><span data-ttu-id="6672f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6672f-118">Request headers</span></span>

| <span data-ttu-id="6672f-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="6672f-119">Header</span></span>       | <span data-ttu-id="6672f-120">Значение</span><span class="sxs-lookup"><span data-stu-id="6672f-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6672f-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6672f-121">Authorization</span></span>  | <span data-ttu-id="6672f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6672f-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6672f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6672f-124">Content-Type</span></span>  | <span data-ttu-id="6672f-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="6672f-p103">application/json. Required.</span></span>  |

## <a name="response"></a><span data-ttu-id="6672f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="6672f-127">Response</span></span>

<span data-ttu-id="6672f-128">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект schedulingGroup](../resources/schedulinggroup.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="6672f-128">If successful, this method returns a `201 Created` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6672f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="6672f-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6672f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="6672f-130">Request</span></span>

<span data-ttu-id="6672f-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6672f-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6672f-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="6672f-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-post-schedulinggroups"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups
Content-type: application/json

{
  "displayName": "Cashiers",
  "isActive": true,
  "userIds": [
    "c5d0c76b-80c4-481c-be50-923cd8d680a1",
    "2a4296b3-a28a-44ba-bc66-0274b9b95851"
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="6672f-133">C#</span><span class="sxs-lookup"><span data-stu-id="6672f-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6672f-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6672f-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6672f-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6672f-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6672f-136">Java</span><span class="sxs-lookup"><span data-stu-id="6672f-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-post-schedulinggroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6672f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="6672f-137">Response</span></span>

<span data-ttu-id="6672f-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="6672f-138">The following is an example of the response.</span></span> 

><span data-ttu-id="6672f-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="6672f-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.schedulingGroup"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "Creates a new schedulingGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


