---
title: Удаление смены
description: Удаляет сдвиг из расписания.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: fb3ea22816f288d4834ce720ebc5e1478da2d7b2
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786110"
---
# <a name="delete-shift"></a><span data-ttu-id="3f396-103">Удаление смены</span><span class="sxs-lookup"><span data-stu-id="3f396-103">Delete shift</span></span>

<span data-ttu-id="3f396-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f396-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f396-105">Удаляет сдвиг [из](../resources/shift.md) расписания.</span><span class="sxs-lookup"><span data-stu-id="3f396-105">Deletes a [shift](../resources/shift.md) from the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f396-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3f396-106">Permissions</span></span>

<span data-ttu-id="3f396-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3f396-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3f396-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3f396-109">Permission type</span></span>      | <span data-ttu-id="3f396-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3f396-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f396-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3f396-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3f396-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f396-112">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3f396-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3f396-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f396-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f396-114">Not supported.</span></span>    |
|<span data-ttu-id="3f396-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3f396-115">Application</span></span> | <span data-ttu-id="3f396-116">Schedule.Read.All, Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f396-116">Schedule.Read.All, Schedule.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f396-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3f396-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="3f396-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3f396-118">Request headers</span></span>

| <span data-ttu-id="3f396-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="3f396-119">Header</span></span>       | <span data-ttu-id="3f396-120">Значение</span><span class="sxs-lookup"><span data-stu-id="3f396-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3f396-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3f396-121">Authorization</span></span>  | <span data-ttu-id="3f396-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3f396-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3f396-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3f396-124">Request body</span></span>
<span data-ttu-id="3f396-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3f396-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3f396-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f396-126">Response</span></span>

<span data-ttu-id="3f396-p103">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="3f396-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f396-129">Пример</span><span class="sxs-lookup"><span data-stu-id="3f396-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3f396-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="3f396-130">Request</span></span>

<span data-ttu-id="3f396-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3f396-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3f396-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f396-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="3f396-133">C#</span><span class="sxs-lookup"><span data-stu-id="3f396-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f396-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f396-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f396-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f396-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3f396-136">Java</span><span class="sxs-lookup"><span data-stu-id="3f396-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3f396-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="3f396-137">Response</span></span>

<span data-ttu-id="3f396-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="3f396-138">The following is an example of the response.</span></span> 

><span data-ttu-id="3f396-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3f396-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response"
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


