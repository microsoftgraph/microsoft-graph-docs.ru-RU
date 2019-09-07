---
title: 'Call: Чанжескриншарингроле'
description: Начало и прекращение демонстрации экрана в звонке. Этот API используется, чтобы разрешить приложениям совместно использовать содержимое экрана с участниками звонка или собрания.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 969dd84b7262dc2495c7990b39af5a593a245808
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792445"
---
# <a name="call-changescreensharingrole"></a><span data-ttu-id="45ba2-104">Call: Чанжескриншарингроле</span><span class="sxs-lookup"><span data-stu-id="45ba2-104">call: changeScreenSharingRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45ba2-105">Начало и прекращение демонстрации экрана в звонке.</span><span class="sxs-lookup"><span data-stu-id="45ba2-105">Start and stop sharing screen in the call.</span></span> <span data-ttu-id="45ba2-106">Этот API используется, чтобы разрешить приложениям совместно использовать содержимое экрана с участниками звонка или собрания.</span><span class="sxs-lookup"><span data-stu-id="45ba2-106">This API is used to allow applications to share screen content with the participants of a call or meeting.</span></span>

## <a name="permissions"></a><span data-ttu-id="45ba2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="45ba2-107">Permissions</span></span>
<span data-ttu-id="45ba2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45ba2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="45ba2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="45ba2-110">Permission type</span></span>                        | <span data-ttu-id="45ba2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="45ba2-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="45ba2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="45ba2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="45ba2-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="45ba2-113">Not Supported</span></span>                               |
| <span data-ttu-id="45ba2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="45ba2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45ba2-115">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="45ba2-115">Not Supported</span></span>                               |
| <span data-ttu-id="45ba2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="45ba2-116">Application</span></span>                            | <span data-ttu-id="45ba2-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="45ba2-117">Calls.AccessMedia.All</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="45ba2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="45ba2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/changeScreenSharingRole
```

## <a name="request-headers"></a><span data-ttu-id="45ba2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="45ba2-119">Request headers</span></span>
| <span data-ttu-id="45ba2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="45ba2-120">Name</span></span>          | <span data-ttu-id="45ba2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="45ba2-121">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="45ba2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="45ba2-122">Authorization</span></span> | <span data-ttu-id="45ba2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="45ba2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="45ba2-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="45ba2-125">Request body</span></span>
<span data-ttu-id="45ba2-126">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="45ba2-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="45ba2-127">Параметр</span><span class="sxs-lookup"><span data-stu-id="45ba2-127">Parameter</span></span>      | <span data-ttu-id="45ba2-128">Тип</span><span class="sxs-lookup"><span data-stu-id="45ba2-128">Type</span></span>    |<span data-ttu-id="45ba2-129">Описание</span><span class="sxs-lookup"><span data-stu-id="45ba2-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45ba2-130">role</span><span class="sxs-lookup"><span data-stu-id="45ba2-130">role</span></span>|<span data-ttu-id="45ba2-131">String.</span><span class="sxs-lookup"><span data-stu-id="45ba2-131">String</span></span>|<span data-ttu-id="45ba2-132">Возможные значения: "средство просмотра", "общий доступ"</span><span class="sxs-lookup"><span data-stu-id="45ba2-132">Possible values are: 'Viewer', 'Sharer'</span></span>|

## <a name="response"></a><span data-ttu-id="45ba2-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="45ba2-133">Response</span></span>
<span data-ttu-id="45ba2-134">Возвращает `202 Accepted` код отклика.</span><span class="sxs-lookup"><span data-stu-id="45ba2-134">Returns `202 Accepted` response code.</span></span>

## <a name="example"></a><span data-ttu-id="45ba2-135">Пример</span><span class="sxs-lookup"><span data-stu-id="45ba2-135">Example</span></span>
<span data-ttu-id="45ba2-136">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="45ba2-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="45ba2-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="45ba2-137">Request</span></span>
<span data-ttu-id="45ba2-138">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="45ba2-138">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="45ba2-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="45ba2-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-changeScreenSharingRole"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/changeScreenSharingRole
Content-Type: application/json
Content-Length: 24

{
  "role": "viewer"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="45ba2-140">C#</span><span class="sxs-lookup"><span data-stu-id="45ba2-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-changescreensharingrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="45ba2-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45ba2-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-changescreensharingrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="45ba2-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="45ba2-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-changescreensharingrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="45ba2-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="45ba2-143">Response</span></span>
<span data-ttu-id="45ba2-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="45ba2-144">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 202 Accepted
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: changeScreenSharingRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
