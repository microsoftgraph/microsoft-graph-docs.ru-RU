---
title: Удаление Тимеофф
description: Удаление экземпляра Тимеофф по расписанию.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d9c3269db1b211a5188beb458f0f94aa209439d3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055750"
---
# <a name="delete-timeoff"></a><span data-ttu-id="038f5-103">Удаление Тимеофф</span><span class="sxs-lookup"><span data-stu-id="038f5-103">Delete timeOff</span></span>

<span data-ttu-id="038f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="038f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="038f5-105">Удаление экземпляра [тимеофф](../resources/timeoff.md) по [расписанию](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="038f5-105">Delete a [timeOff](../resources/timeoff.md) instance from a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="038f5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="038f5-106">Permissions</span></span>

<span data-ttu-id="038f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="038f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="038f5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="038f5-109">Permission type</span></span>      | <span data-ttu-id="038f5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="038f5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="038f5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="038f5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="038f5-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="038f5-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="038f5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="038f5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="038f5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="038f5-114">Not supported.</span></span>    |
|<span data-ttu-id="038f5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="038f5-115">Application</span></span> | <span data-ttu-id="038f5-116">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="038f5-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="038f5-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="038f5-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="038f5-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="038f5-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="038f5-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="038f5-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="038f5-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="038f5-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="038f5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="038f5-121">Request headers</span></span>

| <span data-ttu-id="038f5-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="038f5-122">Header</span></span>       | <span data-ttu-id="038f5-123">Значение</span><span class="sxs-lookup"><span data-stu-id="038f5-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="038f5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="038f5-124">Authorization</span></span>  | <span data-ttu-id="038f5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="038f5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="038f5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="038f5-127">Request body</span></span>
<span data-ttu-id="038f5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="038f5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="038f5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="038f5-129">Response</span></span>

<span data-ttu-id="038f5-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="038f5-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="038f5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="038f5-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="038f5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="038f5-133">Request</span></span>

<span data-ttu-id="038f5-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="038f5-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="038f5-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="038f5-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```
# <a name="c"></a>[<span data-ttu-id="038f5-136">C#</span><span class="sxs-lookup"><span data-stu-id="038f5-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="038f5-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="038f5-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="038f5-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="038f5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="038f5-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="038f5-139">Response</span></span>

<span data-ttu-id="038f5-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="038f5-140">The following is an example of the response.</span></span> 

><span data-ttu-id="038f5-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="038f5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Deletes a timeOff from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


