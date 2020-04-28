---
title: Удаление смены
description: Удаляет смену из расписания.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c0ee4a22d2fc4d206e9ded8419c7fb3317255ece
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453328"
---
# <a name="delete-shift"></a><span data-ttu-id="2a97e-103">Удаление смены</span><span class="sxs-lookup"><span data-stu-id="2a97e-103">Delete shift</span></span>

<span data-ttu-id="2a97e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a97e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a97e-105">Удаляет [смену](../resources/shift.md) из расписания.</span><span class="sxs-lookup"><span data-stu-id="2a97e-105">Deletes a [shift](../resources/shift.md) from the schedule.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a97e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2a97e-106">Permissions</span></span>

<span data-ttu-id="2a97e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a97e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a97e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2a97e-109">Permission type</span></span>      | <span data-ttu-id="2a97e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2a97e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2a97e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2a97e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2a97e-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a97e-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="2a97e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2a97e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a97e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2a97e-114">Not supported.</span></span>    |
|<span data-ttu-id="2a97e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2a97e-115">Application</span></span> | <span data-ttu-id="2a97e-116">Schedule. Read. All *, Schedule. ReadWrite. ALL*</span><span class="sxs-lookup"><span data-stu-id="2a97e-116">Schedule.Read.All *, Schedule.ReadWrite.All*</span></span> |

><span data-ttu-id="2a97e-117">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="2a97e-117">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="2a97e-118">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="2a97e-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="2a97e-119">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="2a97e-119">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="2a97e-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2a97e-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="2a97e-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2a97e-121">Request headers</span></span>

| <span data-ttu-id="2a97e-122">Заголовок</span><span class="sxs-lookup"><span data-stu-id="2a97e-122">Header</span></span>       | <span data-ttu-id="2a97e-123">Значение</span><span class="sxs-lookup"><span data-stu-id="2a97e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2a97e-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2a97e-124">Authorization</span></span>  | <span data-ttu-id="2a97e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2a97e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2a97e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2a97e-127">Request body</span></span>
<span data-ttu-id="2a97e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2a97e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a97e-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a97e-129">Response</span></span>

<span data-ttu-id="2a97e-p104">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="2a97e-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a97e-132">Пример</span><span class="sxs-lookup"><span data-stu-id="2a97e-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="2a97e-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="2a97e-133">Request</span></span>

<span data-ttu-id="2a97e-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2a97e-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2a97e-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="2a97e-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="c"></a>[<span data-ttu-id="2a97e-136">C#</span><span class="sxs-lookup"><span data-stu-id="2a97e-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2a97e-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2a97e-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2a97e-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2a97e-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2a97e-139">Ответ</span><span class="sxs-lookup"><span data-stu-id="2a97e-139">Response</span></span>

<span data-ttu-id="2a97e-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2a97e-140">The following is an example of the response.</span></span> 

><span data-ttu-id="2a97e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="2a97e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
