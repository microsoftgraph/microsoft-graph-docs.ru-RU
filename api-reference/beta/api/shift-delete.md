---
title: Удаление смены
description: Удаляет смену из расписания.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: debaeead3ba2506d9dbe62fec46d569532332a4c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363860"
---
# <a name="delete-shift"></a><span data-ttu-id="2edae-103">Удаление смены</span><span class="sxs-lookup"><span data-stu-id="2edae-103">Delete shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2edae-104">Удаляет [смену](../resources/shift.md) из расписания.</span><span class="sxs-lookup"><span data-stu-id="2edae-104">Deletes a [shift](../resources/shift.md) from the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="2edae-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2edae-105">Permissions</span></span>

<span data-ttu-id="2edae-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2edae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2edae-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2edae-108">Permission type</span></span>      | <span data-ttu-id="2edae-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2edae-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2edae-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2edae-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2edae-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2edae-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2edae-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2edae-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2edae-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2edae-113">Not supported.</span></span>    |
|<span data-ttu-id="2edae-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2edae-114">Application</span></span> | <span data-ttu-id="2edae-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2edae-115">Not supported.</span></span> |

> <span data-ttu-id="2edae-116">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="2edae-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2edae-117">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="2edae-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2edae-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2edae-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="2edae-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2edae-119">Request headers</span></span>

| <span data-ttu-id="2edae-120">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2edae-120">Header</span></span>       | <span data-ttu-id="2edae-121">Значение</span><span class="sxs-lookup"><span data-stu-id="2edae-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2edae-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2edae-122">Authorization</span></span>  | <span data-ttu-id="2edae-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2edae-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2edae-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2edae-125">Content-Type</span></span>  | <span data-ttu-id="2edae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2edae-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2edae-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2edae-127">Request body</span></span>
<span data-ttu-id="2edae-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2edae-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2edae-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2edae-129">Response</span></span>

<span data-ttu-id="2edae-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2edae-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2edae-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2edae-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2edae-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2edae-133">Request</span></span>

<span data-ttu-id="2edae-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2edae-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2edae-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2edae-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2edae-136">C#</span><span class="sxs-lookup"><span data-stu-id="2edae-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2edae-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2edae-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2edae-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="2edae-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2edae-139">Java</span><span class="sxs-lookup"><span data-stu-id="2edae-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2edae-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="2edae-140">Response</span></span>

<span data-ttu-id="2edae-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2edae-141">The following is an example of the response.</span></span> 

><span data-ttu-id="2edae-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2edae-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
