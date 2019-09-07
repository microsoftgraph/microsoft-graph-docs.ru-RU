---
title: 'Call: Упдатеметадата'
description: Обновление метаданных апплиатион, связанных с вызовом.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e777dccdb1eb1925c1c8961c00efe79396f293fd
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/07/2019
ms.locfileid: "36792278"
---
# <a name="call-updatemetadata"></a><span data-ttu-id="b03e4-103">Call: Упдатеметадата</span><span class="sxs-lookup"><span data-stu-id="b03e4-103">call: updateMetadata</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b03e4-104">Обновление метаданных апплиатион, связанных с вызовом.</span><span class="sxs-lookup"><span data-stu-id="b03e4-104">Update the appliation's metadata associated with a call.</span></span>

## <a name="permissions"></a><span data-ttu-id="b03e4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b03e4-105">Permissions</span></span>
<span data-ttu-id="b03e4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b03e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b03e4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b03e4-108">Permission type</span></span>                        | <span data-ttu-id="b03e4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b03e4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b03e4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b03e4-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="b03e4-111">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b03e4-111">Not Supported</span></span>                               |
| <span data-ttu-id="b03e4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b03e4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b03e4-113">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="b03e4-113">Not Supported</span></span>                               |
| <span data-ttu-id="b03e4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b03e4-114">Application</span></span>     | <span data-ttu-id="b03e4-115">Calls. Жоинграупкаллсасгуест. ALL, Calls. Жоинграупкаллс. ALL, Calls. Инитиатеграупкаллс. ALL</span><span class="sxs-lookup"><span data-stu-id="b03e4-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.InitiateGroupCalls.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b03e4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b03e4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /app/calls/{id}/updateMetadata
```

## <a name="request-headers"></a><span data-ttu-id="b03e4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b03e4-117">Request headers</span></span>
| <span data-ttu-id="b03e4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b03e4-118">Name</span></span>          | <span data-ttu-id="b03e4-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b03e4-119">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b03e4-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b03e4-120">Authorization</span></span> | <span data-ttu-id="b03e4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b03e4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b03e4-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b03e4-123">Request body</span></span>
<span data-ttu-id="b03e4-124">В тексте запроса предоставьте JSON-объект с указанными ниже параметрами.</span><span class="sxs-lookup"><span data-stu-id="b03e4-124">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b03e4-125">Параметр</span><span class="sxs-lookup"><span data-stu-id="b03e4-125">Parameter</span></span>      | <span data-ttu-id="b03e4-126">Тип</span><span class="sxs-lookup"><span data-stu-id="b03e4-126">Type</span></span>    |<span data-ttu-id="b03e4-127">Описание</span><span class="sxs-lookup"><span data-stu-id="b03e4-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b03e4-128">метаданных</span><span class="sxs-lookup"><span data-stu-id="b03e4-128">metadata</span></span>|<span data-ttu-id="b03e4-129">String.</span><span class="sxs-lookup"><span data-stu-id="b03e4-129">String</span></span>|<span data-ttu-id="b03e4-130">Большой двоичный объект данных, предоставляемый участником в списке.</span><span class="sxs-lookup"><span data-stu-id="b03e4-130">A blob of data provided by the participant in the roster.</span></span>|
|<span data-ttu-id="b03e4-131">Контекст</span><span class="sxs-lookup"><span data-stu-id="b03e4-131">clientContext</span></span>|<span data-ttu-id="b03e4-132">String.</span><span class="sxs-lookup"><span data-stu-id="b03e4-132">String</span></span>|<span data-ttu-id="b03e4-133">Контекст клиента.</span><span class="sxs-lookup"><span data-stu-id="b03e4-133">The client context.</span></span>|

## <a name="response"></a><span data-ttu-id="b03e4-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="b03e4-134">Response</span></span>
<span data-ttu-id="b03e4-135">Возвращает `202 Accepted` код отклика и заголовок Location с URI для [коммсоператион](../resources/commsoperation.md) , созданного для этого запроса.</span><span class="sxs-lookup"><span data-stu-id="b03e4-135">Returns `202 Accepted` response code and a Location header with a uri to the [commsOperation](../resources/commsoperation.md) created for this request.</span></span>

## <a name="example"></a><span data-ttu-id="b03e4-136">Пример</span><span class="sxs-lookup"><span data-stu-id="b03e4-136">Example</span></span>
<span data-ttu-id="b03e4-137">В приведенном ниже примере показано, как вызывать этот API.</span><span class="sxs-lookup"><span data-stu-id="b03e4-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b03e4-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b03e4-138">Request</span></span>
<span data-ttu-id="b03e4-139">Ниже показан пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b03e4-139">The following example shows the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b03e4-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="b03e4-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "call-updateMetadata"
}-->
```http
POST https://graph.microsoft.com/beta/app/calls/{id}/updateMetadata
Content-Type: application/json
Content-Length: 79

{
  "metadata": "metadata-value",
  "clientContext": "clientContext-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b03e4-141">C#</span><span class="sxs-lookup"><span data-stu-id="b03e4-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/call-updatemetadata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b03e4-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b03e4-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/call-updatemetadata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b03e4-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="b03e4-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/call-updatemetadata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b03e4-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="b03e4-144">Response</span></span>

> <span data-ttu-id="b03e4-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b03e4-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.commsOperation"
} -->
```http
HTTP/1.1 202 Accepted
Location: https://graph.microsoft.com/beta/app/calls/57dab8b1-894c-409a-b240-bd8beae78896/operations/0fe0623f-d628-42ed-b4bd-8ac290072cc5
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "call: updateMetadata",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
