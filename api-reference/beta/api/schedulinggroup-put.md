---
title: Замена объекта schedulingGroup
description: Замена существующего Счедулингграуп.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a073667569fbe9a9e2a62c8ec03dd555e3a7bba8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055822"
---
# <a name="replace-schedulinggroup"></a><span data-ttu-id="91c5e-103">Замена объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="91c5e-103">Replace schedulingGroup</span></span>

<span data-ttu-id="91c5e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91c5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91c5e-105">Замена существующего [счедулингграуп](../resources/schedulinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="91c5e-105">Replace an existing [schedulingGroup](../resources/schedulinggroup.md).</span></span>

<span data-ttu-id="91c5e-106">Если указанный [счедулингграуп](../resources/schedulinggroup.md) не существует, этот метод возвращает значение `404 Not found` .</span><span class="sxs-lookup"><span data-stu-id="91c5e-106">If the specified [schedulingGroup](../resources/schedulinggroup.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="91c5e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91c5e-107">Permissions</span></span>

<span data-ttu-id="91c5e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91c5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91c5e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91c5e-110">Permission type</span></span>      | <span data-ttu-id="91c5e-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91c5e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91c5e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91c5e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="91c5e-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91c5e-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="91c5e-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91c5e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91c5e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91c5e-115">Not supported.</span></span>    |
|<span data-ttu-id="91c5e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91c5e-116">Application</span></span> | <span data-ttu-id="91c5e-117">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="91c5e-117">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="91c5e-118">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="91c5e-118">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="91c5e-119">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="91c5e-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="91c5e-120">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="91c5e-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="91c5e-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91c5e-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="91c5e-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91c5e-122">Request headers</span></span>

| <span data-ttu-id="91c5e-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="91c5e-123">Header</span></span>       | <span data-ttu-id="91c5e-124">Значение</span><span class="sxs-lookup"><span data-stu-id="91c5e-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="91c5e-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="91c5e-125">Authorization</span></span>  | <span data-ttu-id="91c5e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91c5e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="91c5e-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91c5e-128">Content-Type</span></span>  | <span data-ttu-id="91c5e-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91c5e-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="91c5e-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91c5e-131">Request body</span></span>

<span data-ttu-id="91c5e-132">В тексте запроса добавьте представление объекта [счедулингграуп](../resources/schedulinggroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91c5e-132">In the request body, supply a JSON representation of a [schedulingGroup](../resources/schedulinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="91c5e-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="91c5e-133">Response</span></span>

<span data-ttu-id="91c5e-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [счедулингграуп](../resources/schedulinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="91c5e-134">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91c5e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="91c5e-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="91c5e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="91c5e-136">Request</span></span>

<span data-ttu-id="91c5e-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91c5e-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91c5e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="91c5e-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="91c5e-139">C#</span><span class="sxs-lookup"><span data-stu-id="91c5e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-put-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91c5e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91c5e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-put-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91c5e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91c5e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-put-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="91c5e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="91c5e-142">Response</span></span>

<span data-ttu-id="91c5e-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="91c5e-143">The following is an example of the response.</span></span> 

><span data-ttu-id="91c5e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="91c5e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


