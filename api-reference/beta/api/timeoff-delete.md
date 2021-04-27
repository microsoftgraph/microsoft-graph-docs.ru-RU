---
title: Удаление timeOff
description: Удаление экземпляра timeOff из расписания.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 459cf68eb91f47b5c5ffaec965ebbe605a8d783b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050754"
---
# <a name="delete-timeoff"></a><span data-ttu-id="b95d0-103">Удаление timeOff</span><span class="sxs-lookup"><span data-stu-id="b95d0-103">Delete timeOff</span></span>

<span data-ttu-id="b95d0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b95d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b95d0-105">Удаление [экземпляра timeOff](../resources/timeoff.md) из [расписания.](../resources/schedule.md)</span><span class="sxs-lookup"><span data-stu-id="b95d0-105">Delete a [timeOff](../resources/timeoff.md) instance from a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="b95d0-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b95d0-106">Permissions</span></span>

<span data-ttu-id="b95d0-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b95d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b95d0-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b95d0-109">Permission type</span></span>      | <span data-ttu-id="b95d0-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b95d0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b95d0-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b95d0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b95d0-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b95d0-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b95d0-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b95d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b95d0-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b95d0-114">Not supported.</span></span>    |
|<span data-ttu-id="b95d0-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="b95d0-115">Application</span></span> | <span data-ttu-id="b95d0-116">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="b95d0-116">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="b95d0-117">\***Важно:** Разрешения приложения в настоящее время доступны только в закрытом режиме и недоступны для общего пользования.</span><span class="sxs-lookup"><span data-stu-id="b95d0-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="b95d0-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="b95d0-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="b95d0-119">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="b95d0-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="b95d0-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b95d0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="b95d0-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b95d0-121">Request headers</span></span>

| <span data-ttu-id="b95d0-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="b95d0-122">Header</span></span>       | <span data-ttu-id="b95d0-123">Значение</span><span class="sxs-lookup"><span data-stu-id="b95d0-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b95d0-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b95d0-124">Authorization</span></span>  | <span data-ttu-id="b95d0-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b95d0-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b95d0-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b95d0-127">Request body</span></span>
<span data-ttu-id="b95d0-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b95d0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b95d0-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="b95d0-129">Response</span></span>

<span data-ttu-id="b95d0-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="b95d0-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b95d0-132">Пример</span><span class="sxs-lookup"><span data-stu-id="b95d0-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="b95d0-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="b95d0-133">Request</span></span>

<span data-ttu-id="b95d0-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b95d0-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b95d0-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="b95d0-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```
# <a name="c"></a>[<span data-ttu-id="b95d0-136">C#</span><span class="sxs-lookup"><span data-stu-id="b95d0-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b95d0-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b95d0-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b95d0-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b95d0-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b95d0-139">Java</span><span class="sxs-lookup"><span data-stu-id="b95d0-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b95d0-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="b95d0-140">Response</span></span>

<span data-ttu-id="b95d0-141">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b95d0-141">The following is an example of the response.</span></span> 

><span data-ttu-id="b95d0-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b95d0-142">**Note:** The response object shown here might be shortened for readability.</span></span>
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


