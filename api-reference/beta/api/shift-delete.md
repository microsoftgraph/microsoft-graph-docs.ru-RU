---
title: Удаление смены
description: Удаляет смену из расписания.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 0643a262971127eafc6b940c27f6bac7bee4a7e6
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314281"
---
# <a name="delete-shift"></a><span data-ttu-id="65077-103">Удаление смены</span><span class="sxs-lookup"><span data-stu-id="65077-103">Delete shift</span></span>

<span data-ttu-id="65077-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65077-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65077-105">Удаляет [смену](../resources/shift.md) из расписания.</span><span class="sxs-lookup"><span data-stu-id="65077-105">Deletes a [shift](../resources/shift.md) from the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="65077-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="65077-106">Permissions</span></span>

<span data-ttu-id="65077-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65077-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65077-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="65077-109">Permission type</span></span>      | <span data-ttu-id="65077-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="65077-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65077-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="65077-111">Delegated (work or school account)</span></span> | <span data-ttu-id="65077-112">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="65077-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="65077-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="65077-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65077-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65077-114">Not supported.</span></span>    |
|<span data-ttu-id="65077-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="65077-115">Application</span></span> | <span data-ttu-id="65077-116">Schedule. Read. ALL, Schedule. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="65077-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="65077-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="65077-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="65077-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="65077-118">Request headers</span></span>

| <span data-ttu-id="65077-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="65077-119">Header</span></span>       | <span data-ttu-id="65077-120">Значение</span><span class="sxs-lookup"><span data-stu-id="65077-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="65077-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="65077-121">Authorization</span></span>  | <span data-ttu-id="65077-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="65077-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="65077-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="65077-124">Request body</span></span>
<span data-ttu-id="65077-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="65077-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65077-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="65077-126">Response</span></span>

<span data-ttu-id="65077-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="65077-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65077-129">Пример</span><span class="sxs-lookup"><span data-stu-id="65077-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="65077-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="65077-130">Request</span></span>

<span data-ttu-id="65077-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="65077-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="65077-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="65077-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="65077-133">C#</span><span class="sxs-lookup"><span data-stu-id="65077-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65077-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65077-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65077-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65077-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="65077-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="65077-136">Response</span></span>

<span data-ttu-id="65077-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="65077-137">The following is an example of the response.</span></span> 

><span data-ttu-id="65077-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="65077-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Deletes a shift from the schedule",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


