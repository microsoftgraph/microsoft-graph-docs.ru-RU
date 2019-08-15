---
title: Замена объекта schedulingGroup
description: Замена существующего Счедулингграуп.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 2cc22b11fdba3f4b0dfdf7d3e0289e1a9fbcc161
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410649"
---
# <a name="replace-schedulinggroup"></a><span data-ttu-id="b90de-103">Замена объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="b90de-103">Replace schedulingGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b90de-104">Замена существующего [счедулингграуп](../resources/schedulinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="b90de-104">Replace an existing [schedulingGroup](../resources/schedulinggroup.md).</span></span>

<span data-ttu-id="b90de-105">Если указанный [счедулингграуп](../resources/schedulinggroup.md) не существует, этот метод возвращает значение `404 Not found`.</span><span class="sxs-lookup"><span data-stu-id="b90de-105">If the specified [schedulingGroup](../resources/schedulinggroup.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="b90de-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b90de-106">Permissions</span></span>

<span data-ttu-id="b90de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b90de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b90de-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b90de-109">Permission type</span></span>      | <span data-ttu-id="b90de-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b90de-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b90de-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b90de-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b90de-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b90de-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b90de-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b90de-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b90de-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b90de-114">Not supported.</span></span>    |
|<span data-ttu-id="b90de-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b90de-115">Application</span></span> | <span data-ttu-id="b90de-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b90de-116">Not supported.</span></span> |

> <span data-ttu-id="b90de-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="b90de-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b90de-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="b90de-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b90de-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b90de-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="b90de-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b90de-120">Request headers</span></span>

| <span data-ttu-id="b90de-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b90de-121">Header</span></span>       | <span data-ttu-id="b90de-122">Значение</span><span class="sxs-lookup"><span data-stu-id="b90de-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b90de-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b90de-123">Authorization</span></span>  | <span data-ttu-id="b90de-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b90de-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b90de-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b90de-126">Content-Type</span></span>  | <span data-ttu-id="b90de-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b90de-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b90de-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b90de-128">Request body</span></span>

<span data-ttu-id="b90de-129">В тексте запроса добавьте представление объекта [счедулингграуп](../resources/schedulinggroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b90de-129">In the request body, supply a JSON representation of a [schedulingGroup](../resources/schedulinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b90de-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b90de-130">Response</span></span>

<span data-ttu-id="b90de-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [счедулингграуп](../resources/schedulinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="b90de-131">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b90de-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b90de-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b90de-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b90de-133">Request</span></span>

<span data-ttu-id="b90de-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b90de-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b90de-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b90de-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-put-schedulinggroups"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b90de-136">C#</span><span class="sxs-lookup"><span data-stu-id="b90de-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-put-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b90de-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b90de-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-put-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b90de-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b90de-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-put-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b90de-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="b90de-139">Response</span></span>

<span data-ttu-id="b90de-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b90de-140">The following is an example of the response.</span></span> 

><span data-ttu-id="b90de-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b90de-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
