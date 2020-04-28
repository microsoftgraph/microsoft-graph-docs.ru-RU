---
title: Удаление Тимеоффреасон
description: Пометка Тимеоффреасон как неактивной с помощью задания свойства GetProperty
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: b33b6ff6b91923e6821f9e4ae8a0aa8043373f4a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42452304"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="67ffc-103">Удаление Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="67ffc-103">Delete timeOffReason</span></span>

<span data-ttu-id="67ffc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67ffc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67ffc-105">Помечайте Тимеоффреасон как неактивную **isActive** , устанавливая свойство [timeOffReason](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="67ffc-105">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span>

<span data-ttu-id="67ffc-106">Этот метод не удаляет указанный экземпляр [тимеоффреасон](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="67ffc-106">This method does not remove the specified [timeOffReason](../resources/timeoffreason.md) instance.</span></span> <span data-ttu-id="67ffc-107">экземпляры [тимеоффитем](../resources/timeoffitem.md) , которым назначена эта причина, остались назначенными по этой причине.</span><span class="sxs-lookup"><span data-stu-id="67ffc-107">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="67ffc-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="67ffc-108">Permissions</span></span>

<span data-ttu-id="67ffc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67ffc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67ffc-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="67ffc-111">Permission type</span></span>      | <span data-ttu-id="67ffc-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="67ffc-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="67ffc-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="67ffc-113">Delegated (work or school account)</span></span> | <span data-ttu-id="67ffc-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67ffc-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="67ffc-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="67ffc-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67ffc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="67ffc-116">Not supported.</span></span>    |
|<span data-ttu-id="67ffc-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="67ffc-117">Application</span></span> | <span data-ttu-id="67ffc-118">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="67ffc-118">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="67ffc-119">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="67ffc-119">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="67ffc-120">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="67ffc-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="67ffc-121">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="67ffc-121">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="67ffc-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="67ffc-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="67ffc-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="67ffc-123">Request headers</span></span>

| <span data-ttu-id="67ffc-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="67ffc-124">Header</span></span>       | <span data-ttu-id="67ffc-125">Значение</span><span class="sxs-lookup"><span data-stu-id="67ffc-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="67ffc-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="67ffc-126">Authorization</span></span>  | <span data-ttu-id="67ffc-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="67ffc-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="67ffc-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="67ffc-129">Request body</span></span>
<span data-ttu-id="67ffc-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="67ffc-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="67ffc-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="67ffc-131">Response</span></span>

<span data-ttu-id="67ffc-p105">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="67ffc-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67ffc-134">Пример</span><span class="sxs-lookup"><span data-stu-id="67ffc-134">Example</span></span>

#### <a name="request"></a><span data-ttu-id="67ffc-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="67ffc-135">Request</span></span>

<span data-ttu-id="67ffc-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="67ffc-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="67ffc-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="67ffc-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="c"></a>[<span data-ttu-id="67ffc-138">C#</span><span class="sxs-lookup"><span data-stu-id="67ffc-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67ffc-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67ffc-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67ffc-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67ffc-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="67ffc-141">Ответ</span><span class="sxs-lookup"><span data-stu-id="67ffc-141">Response</span></span>

<span data-ttu-id="67ffc-142">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="67ffc-142">The following is an example of the response.</span></span> 

><span data-ttu-id="67ffc-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="67ffc-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
