---
title: Удаление Тимеоффреасон
description: Пометка Тимеоффреасон как неактивной с помощью задания свойства GetProperty
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 25e07aa77790b38da5c19922060ac93490166fd3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457935"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="ba9ad-103">Удаление Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="ba9ad-103">Delete timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba9ad-104">Помечайте Тимеоффреасон как неактивную \*\*\*\* , устанавливая свойство [](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="ba9ad-104">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span>

<span data-ttu-id="ba9ad-105">Этот метод не удаляет указанный экземпляр [тимеоффреасон](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="ba9ad-105">This method does not remove the specified [timeOffReason](../resources/timeoffreason.md) instance.</span></span> <span data-ttu-id="ba9ad-106">экземпляры [тимеоффитем](../resources/timeoffitem.md) , которым назначена эта причина, остались назначенными по этой причине.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-106">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba9ad-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba9ad-107">Permissions</span></span>

<span data-ttu-id="ba9ad-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba9ad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba9ad-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba9ad-110">Permission type</span></span>      | <span data-ttu-id="ba9ad-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba9ad-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba9ad-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba9ad-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ba9ad-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba9ad-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ba9ad-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba9ad-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba9ad-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-115">Not supported.</span></span>    |
|<span data-ttu-id="ba9ad-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba9ad-116">Application</span></span> | <span data-ttu-id="ba9ad-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-117">Not supported.</span></span> |

> <span data-ttu-id="ba9ad-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ba9ad-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ba9ad-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba9ad-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="ba9ad-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba9ad-121">Request headers</span></span>

| <span data-ttu-id="ba9ad-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="ba9ad-122">Header</span></span>       | <span data-ttu-id="ba9ad-123">Значение</span><span class="sxs-lookup"><span data-stu-id="ba9ad-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ba9ad-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="ba9ad-124">Authorization</span></span>  | <span data-ttu-id="ba9ad-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ba9ad-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ba9ad-127">Content-Type</span></span>  | <span data-ttu-id="ba9ad-128">application/json</span><span class="sxs-lookup"><span data-stu-id="ba9ad-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ba9ad-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ba9ad-129">Request body</span></span>
<span data-ttu-id="ba9ad-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba9ad-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba9ad-131">Response</span></span>

<span data-ttu-id="ba9ad-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba9ad-134">Пример</span><span class="sxs-lookup"><span data-stu-id="ba9ad-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ba9ad-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba9ad-135">Request</span></span>

<span data-ttu-id="ba9ad-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ba9ad-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="ba9ad-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ba9ad-138">C#</span><span class="sxs-lookup"><span data-stu-id="ba9ad-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ba9ad-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="ba9ad-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ba9ad-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="ba9ad-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ba9ad-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba9ad-141">Response</span></span>

<span data-ttu-id="ba9ad-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-142">The following is an example of the response.</span></span> 

><span data-ttu-id="ba9ad-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ba9ad-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "Marks a timeOffReason as inactive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
