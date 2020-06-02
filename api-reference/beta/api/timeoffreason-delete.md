---
title: Удаление Тимеоффреасон
description: Помечайте Тимеоффреасон как неактивную, устанавливая свойство.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1e71e976167b94d144037d93bf9bb3dff59cc5b7
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44154425"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="f1a9e-103">Удаление Тимеоффреасон</span><span class="sxs-lookup"><span data-stu-id="f1a9e-103">Delete timeOffReason</span></span>

<span data-ttu-id="f1a9e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1a9e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1a9e-105">Помечайте Тимеоффреасон как неактивную **isActive** , устанавливая свойство [timeOffReason](../resources/timeoffreason.md) .</span><span class="sxs-lookup"><span data-stu-id="f1a9e-105">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span> <span data-ttu-id="f1a9e-106">Каждая команда должна включать по крайней мере один **тимеоффреасон**.</span><span class="sxs-lookup"><span data-stu-id="f1a9e-106">Every team must include at least one **timeOffReason**.</span></span>

<span data-ttu-id="f1a9e-107">Этот метод не удаляет указанный экземпляр **тимеоффреасон** .</span><span class="sxs-lookup"><span data-stu-id="f1a9e-107">This method does not remove the specified **timeOffReason** instance.</span></span> <span data-ttu-id="f1a9e-108">экземпляры [тимеоффитем](../resources/timeoffitem.md) , которым назначена эта причина, остались назначенными по этой причине.</span><span class="sxs-lookup"><span data-stu-id="f1a9e-108">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="f1a9e-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f1a9e-109">Permissions</span></span>

<span data-ttu-id="f1a9e-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1a9e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1a9e-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f1a9e-112">Permission type</span></span>      | <span data-ttu-id="f1a9e-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f1a9e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1a9e-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f1a9e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f1a9e-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1a9e-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f1a9e-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f1a9e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1a9e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f1a9e-117">Not supported.</span></span>    |
|<span data-ttu-id="f1a9e-118">Сервер приложений</span><span class="sxs-lookup"><span data-stu-id="f1a9e-118">Application</span></span> | <span data-ttu-id="f1a9e-119">Schedule. ReadWrite. ALL \*</span><span class="sxs-lookup"><span data-stu-id="f1a9e-119">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="f1a9e-120">\***Важно!** Разрешения на доступ к приложениям в настоящее время доступны только для частного просмотра и недоступны для использования в общедоступном режиме.</span><span class="sxs-lookup"><span data-stu-id="f1a9e-120">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="f1a9e-121">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="f1a9e-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f1a9e-122">Глобальные администраторы могут получать доступ к группам, которые не являются участниками.</span><span class="sxs-lookup"><span data-stu-id="f1a9e-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f1a9e-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f1a9e-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="f1a9e-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f1a9e-124">Request headers</span></span>

| <span data-ttu-id="f1a9e-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="f1a9e-125">Header</span></span>       | <span data-ttu-id="f1a9e-126">Значение</span><span class="sxs-lookup"><span data-stu-id="f1a9e-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f1a9e-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f1a9e-127">Authorization</span></span>  | <span data-ttu-id="f1a9e-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="f1a9e-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f1a9e-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f1a9e-130">Request body</span></span>
<span data-ttu-id="f1a9e-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="f1a9e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f1a9e-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1a9e-132">Response</span></span>

<span data-ttu-id="f1a9e-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="f1a9e-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1a9e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="f1a9e-135">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f1a9e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="f1a9e-136">Request</span></span>

<span data-ttu-id="f1a9e-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f1a9e-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f1a9e-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="f1a9e-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="c"></a>[<span data-ttu-id="f1a9e-139">C#</span><span class="sxs-lookup"><span data-stu-id="f1a9e-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f1a9e-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f1a9e-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f1a9e-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f1a9e-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f1a9e-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="f1a9e-142">Response</span></span>

<span data-ttu-id="f1a9e-143">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="f1a9e-143">The following is an example of the response.</span></span> 

><span data-ttu-id="f1a9e-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f1a9e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
