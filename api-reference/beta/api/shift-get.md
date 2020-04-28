---
title: Получение смены
description: Получение сдвига по ИДЕНТИФИКАТОРу.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1074150b77b8608a158a25db2224bd913f8cd157
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453305"
---
# <a name="get-shift"></a><span data-ttu-id="7ca73-103">Получение смены</span><span class="sxs-lookup"><span data-stu-id="7ca73-103">Get shift</span></span>

<span data-ttu-id="7ca73-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ca73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ca73-105">Получение свойств и связей объекта [SHIFT](../resources/shift.md) по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="7ca73-105">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="7ca73-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7ca73-106">Permissions</span></span>

<span data-ttu-id="7ca73-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7ca73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ca73-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7ca73-109">Permission type</span></span>      | <span data-ttu-id="7ca73-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7ca73-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7ca73-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7ca73-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7ca73-112">Group.Read.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ca73-112">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7ca73-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7ca73-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ca73-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7ca73-114">Not supported.</span></span>    |<span data-ttu-id="7ca73-115">s</span><span class="sxs-lookup"><span data-stu-id="7ca73-115">s</span></span>
|<span data-ttu-id="7ca73-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7ca73-116">Application</span></span> | <span data-ttu-id="7ca73-117">Schedule. Read. All *, Schedule. ReadWrite. ALL*</span><span class="sxs-lookup"><span data-stu-id="7ca73-117">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="7ca73-118">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="7ca73-118">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="7ca73-119">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="7ca73-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="7ca73-120">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="7ca73-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="7ca73-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7ca73-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="7ca73-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7ca73-122">Request headers</span></span>

| <span data-ttu-id="7ca73-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7ca73-123">Header</span></span>       | <span data-ttu-id="7ca73-124">Значение</span><span class="sxs-lookup"><span data-stu-id="7ca73-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7ca73-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7ca73-125">Authorization</span></span>  | <span data-ttu-id="7ca73-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7ca73-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7ca73-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7ca73-128">Request body</span></span>
<span data-ttu-id="7ca73-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="7ca73-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ca73-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="7ca73-130">Response</span></span>

<span data-ttu-id="7ca73-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [сдвига](../resources/shift.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="7ca73-131">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ca73-132">Пример</span><span class="sxs-lookup"><span data-stu-id="7ca73-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="7ca73-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="7ca73-133">Request</span></span>

<span data-ttu-id="7ca73-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7ca73-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7ca73-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ca73-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="7ca73-136">C#</span><span class="sxs-lookup"><span data-stu-id="7ca73-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ca73-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ca73-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ca73-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ca73-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="7ca73-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="7ca73-139">Response</span></span>

<span data-ttu-id="7ca73-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7ca73-140">The following is an example of the response.</span></span> 

><span data-ttu-id="7ca73-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="7ca73-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
    "id": "SHFT_ca485cdd-a42c-4b93-9e6a-6fa54fd45fe1",
    "createdDateTime": "2019-06-06T20:15:38.9Z",
    "lastModifiedDateTime": "2019-11-18T01:12:08.318Z",
    "schedulingGroupId": "TAG_d18fd675-3ac8-41b2-8038-d17fdac8b0d3",
    "userId": "a7b0c8c4-3f5c-492f-ab13-40f0e0f0ffa8",
    "draftShift": null,
    "lastModifiedBy": {
        "application": null,
        "device": null,
        "conversation": null,
        "user": {
            "id": "1c717a55-febd-4850-b5f6-101f3a29972c",
            "displayName": "Sumanth Lingom"
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a shift by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
