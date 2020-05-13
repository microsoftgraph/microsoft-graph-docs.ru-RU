---
title: Замена объекта schedulingGroup
description: Замена существующего Счедулингграуп.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b9bc875b3bd01cc2083f7726a1c0abb42c0bb316
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2020
ms.locfileid: "42453784"
---
# <a name="replace-schedulinggroup"></a><span data-ttu-id="a12a9-103">Замена объекта schedulingGroup</span><span class="sxs-lookup"><span data-stu-id="a12a9-103">Replace schedulingGroup</span></span>

<span data-ttu-id="a12a9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a12a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a12a9-105">Замена существующего [счедулингграуп](../resources/schedulinggroup.md).</span><span class="sxs-lookup"><span data-stu-id="a12a9-105">Replace an existing [schedulingGroup](../resources/schedulinggroup.md).</span></span>

<span data-ttu-id="a12a9-106">Если указанный [счедулингграуп](../resources/schedulinggroup.md) не существует, этот метод возвращает значение `404 Not found` .</span><span class="sxs-lookup"><span data-stu-id="a12a9-106">If the specified [schedulingGroup](../resources/schedulinggroup.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="a12a9-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a12a9-107">Permissions</span></span>

<span data-ttu-id="a12a9-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a12a9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a12a9-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a12a9-110">Permission type</span></span>      | <span data-ttu-id="a12a9-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a12a9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a12a9-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a12a9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a12a9-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a12a9-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a12a9-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a12a9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a12a9-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a12a9-115">Not supported.</span></span>    |
|<span data-ttu-id="a12a9-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a12a9-116">Application</span></span> | <span data-ttu-id="a12a9-117">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="a12a9-117">Schedule.ReadWrite.All\*</span></span>  |

><span data-ttu-id="a12a9-118">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="a12a9-118">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="a12a9-119">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="a12a9-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a12a9-120">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="a12a9-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a12a9-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a12a9-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/schedulingGroups/{schedulingGroupId}
```

## <a name="request-headers"></a><span data-ttu-id="a12a9-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a12a9-122">Request headers</span></span>

| <span data-ttu-id="a12a9-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a12a9-123">Header</span></span>       | <span data-ttu-id="a12a9-124">Значение</span><span class="sxs-lookup"><span data-stu-id="a12a9-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a12a9-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a12a9-125">Authorization</span></span>  | <span data-ttu-id="a12a9-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a12a9-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a12a9-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a12a9-128">Content-Type</span></span>  | <span data-ttu-id="a12a9-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a12a9-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a12a9-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a12a9-131">Request body</span></span>

<span data-ttu-id="a12a9-132">В тексте запроса добавьте представление объекта [счедулингграуп](../resources/schedulinggroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a12a9-132">In the request body, supply a JSON representation of a [schedulingGroup](../resources/schedulinggroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a12a9-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="a12a9-133">Response</span></span>

<span data-ttu-id="a12a9-134">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [счедулингграуп](../resources/schedulinggroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a12a9-134">If successful, this method returns a `200 OK` response code and a [schedulingGroup](../resources/schedulinggroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a12a9-135">Пример</span><span class="sxs-lookup"><span data-stu-id="a12a9-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a12a9-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a12a9-136">Request</span></span>

<span data-ttu-id="a12a9-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a12a9-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a12a9-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="a12a9-138">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a12a9-139">C#</span><span class="sxs-lookup"><span data-stu-id="a12a9-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-put-schedulinggroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a12a9-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a12a9-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-put-schedulinggroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a12a9-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a12a9-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-put-schedulinggroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a12a9-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="a12a9-142">Response</span></span>

<span data-ttu-id="a12a9-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a12a9-143">The following is an example of the response.</span></span> 

><span data-ttu-id="a12a9-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a12a9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
