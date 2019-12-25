---
title: Удаление Тимеофф
description: Удаление экземпляра Тимеофф по расписанию.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5e5108b7fe46c1bcf7699e9216a5a3228f77d438
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40864917"
---
# <a name="delete-timeoff"></a><span data-ttu-id="784fc-103">Удаление Тимеофф</span><span class="sxs-lookup"><span data-stu-id="784fc-103">Delete timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="784fc-104">Удаление экземпляра [тимеофф](../resources/timeoff.md) по [расписанию](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="784fc-104">Delete a [timeOff](../resources/timeoff.md) instance from a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="784fc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="784fc-105">Permissions</span></span>

<span data-ttu-id="784fc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="784fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="784fc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="784fc-108">Permission type</span></span>      | <span data-ttu-id="784fc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="784fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="784fc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="784fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="784fc-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="784fc-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="784fc-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="784fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="784fc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="784fc-113">Not supported.</span></span>    |
|<span data-ttu-id="784fc-114">Приложение</span><span class="sxs-lookup"><span data-stu-id="784fc-114">Application</span></span> | <span data-ttu-id="784fc-115">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="784fc-115">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="784fc-116">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="784fc-116">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="784fc-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="784fc-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="784fc-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="784fc-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="784fc-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="784fc-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="784fc-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="784fc-120">Request headers</span></span>

| <span data-ttu-id="784fc-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="784fc-121">Header</span></span>       | <span data-ttu-id="784fc-122">Значение</span><span class="sxs-lookup"><span data-stu-id="784fc-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="784fc-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="784fc-123">Authorization</span></span>  | <span data-ttu-id="784fc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="784fc-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="784fc-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="784fc-126">Request body</span></span>
<span data-ttu-id="784fc-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="784fc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="784fc-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="784fc-128">Response</span></span>

<span data-ttu-id="784fc-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="784fc-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="784fc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="784fc-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="784fc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="784fc-132">Request</span></span>

<span data-ttu-id="784fc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="784fc-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="784fc-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="784fc-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="784fc-135">C#</span><span class="sxs-lookup"><span data-stu-id="784fc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="784fc-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="784fc-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="784fc-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="784fc-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="784fc-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="784fc-138">Response</span></span>

<span data-ttu-id="784fc-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="784fc-139">The following is an example of the response.</span></span> 

><span data-ttu-id="784fc-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="784fc-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
