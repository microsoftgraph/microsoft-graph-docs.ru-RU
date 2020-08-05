---
title: Удаление Тимеофф
description: Удаление экземпляра Тимеофф по расписанию.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 68c26aafd2dcf5f7c4755117587267e9c03e3eaf
ms.sourcegitcommit: 29135eaeff6b2e963b9b5a8b41c207f044dce0fd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/04/2020
ms.locfileid: "44218064"
---
# <a name="delete-timeoff"></a><span data-ttu-id="a18ed-103">Удаление Тимеофф</span><span class="sxs-lookup"><span data-stu-id="a18ed-103">Delete timeOff</span></span>

<span data-ttu-id="a18ed-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a18ed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a18ed-105">Удаление экземпляра [тимеофф](../resources/timeoff.md) по [расписанию](../resources/schedule.md).</span><span class="sxs-lookup"><span data-stu-id="a18ed-105">Delete a [timeOff](../resources/timeoff.md) instance from a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a18ed-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a18ed-106">Permissions</span></span>

<span data-ttu-id="a18ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a18ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a18ed-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a18ed-109">Permission type</span></span>      | <span data-ttu-id="a18ed-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a18ed-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a18ed-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a18ed-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a18ed-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a18ed-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a18ed-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a18ed-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a18ed-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a18ed-114">Not supported.</span></span>    |
|<span data-ttu-id="a18ed-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a18ed-115">Application</span></span> | <span data-ttu-id="a18ed-116">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a18ed-116">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="a18ed-117">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="a18ed-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a18ed-118">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="a18ed-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a18ed-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a18ed-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="a18ed-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a18ed-120">Request headers</span></span>

| <span data-ttu-id="a18ed-121">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a18ed-121">Header</span></span>       | <span data-ttu-id="a18ed-122">Значение</span><span class="sxs-lookup"><span data-stu-id="a18ed-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a18ed-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a18ed-123">Authorization</span></span>  | <span data-ttu-id="a18ed-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a18ed-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a18ed-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a18ed-126">Request body</span></span>
<span data-ttu-id="a18ed-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a18ed-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a18ed-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="a18ed-128">Response</span></span>

<span data-ttu-id="a18ed-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a18ed-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a18ed-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a18ed-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="a18ed-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a18ed-132">Request</span></span>

<span data-ttu-id="a18ed-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a18ed-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a18ed-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a18ed-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timesOff/{timeOffId}
```
# <a name="c"></a>[<span data-ttu-id="a18ed-135">C#</span><span class="sxs-lookup"><span data-stu-id="a18ed-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a18ed-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a18ed-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a18ed-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a18ed-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a18ed-138">Java</span><span class="sxs-lookup"><span data-stu-id="a18ed-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


#### <a name="response"></a><span data-ttu-id="a18ed-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a18ed-139">Response</span></span>

<span data-ttu-id="a18ed-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a18ed-140">The following is an example of the response.</span></span> 

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
