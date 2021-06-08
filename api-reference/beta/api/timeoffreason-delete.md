---
title: Удаление timeOffReason
description: Пометить timeOffReason как неактивное, задав свойство isActive.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 48c39c0b371a6feafb7c89868903b60c8bb4ea63
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787347"
---
# <a name="delete-timeoffreason"></a><span data-ttu-id="e5fec-103">Удаление timeOffReason</span><span class="sxs-lookup"><span data-stu-id="e5fec-103">Delete timeOffReason</span></span>

<span data-ttu-id="e5fec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5fec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e5fec-105">[Пометить timeOffReason](../resources/timeoffreason.md) как неактивное, задав **свойство isActive.**</span><span class="sxs-lookup"><span data-stu-id="e5fec-105">Mark a [timeOffReason](../resources/timeoffreason.md) as inactive by setting the **isActive** property.</span></span> <span data-ttu-id="e5fec-106">Каждая команда должна включать по крайней мере один **разOffReason**.</span><span class="sxs-lookup"><span data-stu-id="e5fec-106">Every team must include at least one **timeOffReason**.</span></span>

<span data-ttu-id="e5fec-107">Этот метод не удаляет указанный экземпляр **timeOffReason.**</span><span class="sxs-lookup"><span data-stu-id="e5fec-107">This method does not remove the specified **timeOffReason** instance.</span></span> <span data-ttu-id="e5fec-108">[Экземпляры timeOffItem,](../resources/timeoffitem.md) которые были назначены по этой причине, остаются назначены по этой причине.</span><span class="sxs-lookup"><span data-stu-id="e5fec-108">[timeOffItem](../resources/timeoffitem.md) instances that have been assigned this reason remain assigned to this reason.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5fec-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e5fec-109">Permissions</span></span>

<span data-ttu-id="e5fec-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5fec-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5fec-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e5fec-112">Permission type</span></span>      | <span data-ttu-id="e5fec-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e5fec-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5fec-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e5fec-114">Delegated (work or school account)</span></span> | <span data-ttu-id="e5fec-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5fec-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e5fec-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e5fec-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5fec-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e5fec-117">Not supported.</span></span>    |
|<span data-ttu-id="e5fec-118">Приложение</span><span class="sxs-lookup"><span data-stu-id="e5fec-118">Application</span></span> | <span data-ttu-id="e5fec-119">Schedule.ReadWrite.All\*</span><span class="sxs-lookup"><span data-stu-id="e5fec-119">Schedule.ReadWrite.All\*</span></span> |

><span data-ttu-id="e5fec-120">\***Важно:** Разрешения приложения в настоящее время доступны только в закрытом режиме и недоступны для общего пользования.</span><span class="sxs-lookup"><span data-stu-id="e5fec-120">\* **Important:** Application permissions are currently in private preview only and are not available for public use.</span></span>

> <span data-ttu-id="e5fec-121">**Примечание**. Этот API поддерживает разрешения администратора.</span><span class="sxs-lookup"><span data-stu-id="e5fec-121">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e5fec-122">Глобальные администраторы могут получать доступ к группам, в которых они не являются членами.</span><span class="sxs-lookup"><span data-stu-id="e5fec-122">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e5fec-123">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e5fec-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```

## <a name="request-headers"></a><span data-ttu-id="e5fec-124">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e5fec-124">Request headers</span></span>

| <span data-ttu-id="e5fec-125">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e5fec-125">Header</span></span>       | <span data-ttu-id="e5fec-126">Значение</span><span class="sxs-lookup"><span data-stu-id="e5fec-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e5fec-127">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e5fec-127">Authorization</span></span>  | <span data-ttu-id="e5fec-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e5fec-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e5fec-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e5fec-130">Request body</span></span>
<span data-ttu-id="e5fec-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e5fec-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5fec-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5fec-132">Response</span></span>

<span data-ttu-id="e5fec-p106">При успешном выполнении этот метод возвращает код отклика `204 No Content`. Метод не возвращает данные в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="e5fec-p106">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5fec-135">Пример</span><span class="sxs-lookup"><span data-stu-id="e5fec-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5fec-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="e5fec-136">Request</span></span>

<span data-ttu-id="e5fec-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e5fec-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e5fec-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5fec-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoffreason-delete"
}-->
```http
DELETE https://graph.microsoft.com/beta/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}
```
# <a name="c"></a>[<span data-ttu-id="e5fec-139">C#</span><span class="sxs-lookup"><span data-stu-id="e5fec-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoffreason-delete-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5fec-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5fec-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoffreason-delete-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5fec-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5fec-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoffreason-delete-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5fec-142">Java</span><span class="sxs-lookup"><span data-stu-id="e5fec-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoffreason-delete-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e5fec-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e5fec-143">Response</span></span>

<span data-ttu-id="e5fec-144">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="e5fec-144">The following is an example of the response.</span></span> 

><span data-ttu-id="e5fec-145">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e5fec-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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
  "description": "Marks a timeOffReason as inactive",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


