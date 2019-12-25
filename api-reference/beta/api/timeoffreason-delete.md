---
title: Удаление Тимеоффреасон
description: Пометка Тимеоффреасон как неактивной с помощью задания свойства GetProperty
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: a3c8b5618aa0582668ffb262404ba678bbbcf61d
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863661"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="d3e27-103">Удаление Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="d3e27-103">Delete timeOffReason</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3e27-104">Помечайте Тимеоффреасон как неактивную \*\*\*\* , устанавливая свойство [](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="d3e27-104">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span>

<span data-ttu-id="d3e27-105">Этот метод не удаляет указанный экземпляр [тимеоффреасон](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="d3e27-105">This method does not remove the specified [timeOffReason](../resources/timeoffreason.md) instance.</span></span> <span data-ttu-id="d3e27-106">экземпляры [тимеоффитем](../resources/timeoffitem.md) , которым назначена эта причина, остались назначенными по этой причине.</span><span class="sxs-lookup"><span data-stu-id="d3e27-106">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="d3e27-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d3e27-107">Permissions</span></span>

<span data-ttu-id="d3e27-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d3e27-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3e27-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d3e27-110">Permission type</span></span>      | <span data-ttu-id="d3e27-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d3e27-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d3e27-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d3e27-112">Delegated (work or school account)</span></span> | <span data-ttu-id="d3e27-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3e27-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="d3e27-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d3e27-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d3e27-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d3e27-115">Not supported.</span></span>    |
|<span data-ttu-id="d3e27-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="d3e27-116">Application</span></span> | <span data-ttu-id="d3e27-117">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="d3e27-117">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="d3e27-118">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="d3e27-118">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="d3e27-119">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="d3e27-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="d3e27-120">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="d3e27-120">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="d3e27-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d3e27-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="d3e27-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d3e27-122">Request headers</span></span>

| <span data-ttu-id="d3e27-123">Заголовок</span><span class="sxs-lookup"><span data-stu-id="d3e27-123">Header</span></span>       | <span data-ttu-id="d3e27-124">Значение</span><span class="sxs-lookup"><span data-stu-id="d3e27-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d3e27-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d3e27-125">Authorization</span></span>  | <span data-ttu-id="d3e27-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d3e27-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d3e27-128">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="d3e27-128">Request body</span></span>
<span data-ttu-id="d3e27-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d3e27-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3e27-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="d3e27-130">Response</span></span>

<span data-ttu-id="d3e27-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="d3e27-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d3e27-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d3e27-133">Example</span></span>

#### <a name="request"></a><span data-ttu-id="d3e27-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d3e27-134">Request</span></span>

<span data-ttu-id="d3e27-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d3e27-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d3e27-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="d3e27-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d3e27-137">C#</span><span class="sxs-lookup"><span data-stu-id="d3e27-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d3e27-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d3e27-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d3e27-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d3e27-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d3e27-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="d3e27-140">Response</span></span>

<span data-ttu-id="d3e27-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="d3e27-141">The following is an example of the response.</span></span> 

><span data-ttu-id="d3e27-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d3e27-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
