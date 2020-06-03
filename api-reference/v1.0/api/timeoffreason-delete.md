---
title: Удаление Тимеоффреасон
description: Помечайте Тимеоффреасон как неактивную, устанавливая свойство.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 5d6cc11350b48924ed9aba7a4395a4fa707fe7f3
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44217498"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="e748c-103">Удаление Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="e748c-103">Delete timeOffReason</span></span>

<span data-ttu-id="e748c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e748c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e748c-105">Помечайте Тимеоффреасон как неактивную **isActive** , устанавливая свойство [timeOffReason](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="e748c-105">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span> <span data-ttu-id="e748c-106">Каждая команда должна включать по крайней мере одну причину тимеофф.</span><span class="sxs-lookup"><span data-stu-id="e748c-106">Every team must include at least one timeoff reason.</span></span>

<span data-ttu-id="e748c-107">Этот метод не удаляет указанный экземпляр [тимеоффреасон](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="e748c-107">This method does not remove the specified [timeOffReason](../resources/timeoffreason.md) instance.</span></span> <span data-ttu-id="e748c-108">экземпляры [тимеоффитем](../resources/timeoffitem.md) , которым назначена эта причина, остались назначенными по этой причине.</span><span class="sxs-lookup"><span data-stu-id="e748c-108">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="e748c-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e748c-109">Permissions</span></span>

<span data-ttu-id="e748c-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e748c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e748c-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e748c-112">Permission type</span></span>      | <span data-ttu-id="e748c-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e748c-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e748c-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e748c-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e748c-115">Запланируйте. ReadWrite. ALL, Group. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="e748c-115">Schedule.ReadWrite.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e748c-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e748c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e748c-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e748c-117">Not supported.</span></span>    |
|<span data-ttu-id="e748c-118">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="e748c-118">Application</span></span> | <span data-ttu-id="e748c-119">Schedule.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e748c-119">Schedule.ReadWrite.All</span></span> |

> <span data-ttu-id="e748c-120">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="e748c-120">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e748c-121">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="e748c-121">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e748c-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e748c-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="e748c-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e748c-123">Request headers</span></span>

| <span data-ttu-id="e748c-124">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e748c-124">Header</span></span>       | <span data-ttu-id="e748c-125">Значение</span><span class="sxs-lookup"><span data-stu-id="e748c-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e748c-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e748c-126">Authorization</span></span>  | <span data-ttu-id="e748c-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e748c-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e748c-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e748c-129">Request body</span></span>
<span data-ttu-id="e748c-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e748c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e748c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="e748c-131">Response</span></span>

<span data-ttu-id="e748c-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e748c-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e748c-134">Пример</span><span class="sxs-lookup"><span data-stu-id="e748c-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="e748c-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="e748c-135">Request</span></span>

<span data-ttu-id="e748c-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e748c-136">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="e748c-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="e748c-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="c"></a>[<span data-ttu-id="e748c-138">C#</span><span class="sxs-lookup"><span data-stu-id="e748c-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e748c-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e748c-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e748c-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e748c-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e748c-141">Java</span><span class="sxs-lookup"><span data-stu-id="e748c-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffreason-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---


### <a name="response"></a><span data-ttu-id="e748c-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="e748c-142">Response</span></span>

<span data-ttu-id="e748c-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e748c-143">The following is an example of the response.</span></span> 

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
